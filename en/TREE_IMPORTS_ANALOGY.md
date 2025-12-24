# Tree Imports Analogy

**Author:** Josué Amaral  
**Date:** December 24, 2025  
**Context:** Phase 3.0 - Refactoring Architecture  
**Applicable to:** All programming languages

---

## 📚 Overview

This document describes the **Tree Imports Analogy**, a mental model for understanding and organizing the dependency architecture in software projects. This analogy is applicable to any programming language that supports module importing/inclusion.

---

## 🌳 The Imports Tree

### Fundamental Concept

A project's import structure can be visualized as a **hierarchical tree**, where:

```
                    📦 A (Root)
                   /           \
              📦 B              📦 C
             / | \               |
        📦 D 📦 E 📦 F         📦 G
         |    |    |            |
      [libs] [libs] [libs]   [libs]
```

### Tree Elements

#### 🌲 **Root**
- **Main File** (e.g., `app.py`, `main.py`, `index.js`)
- **Characteristics:**
  - Most complex and encapsulated
  - System orchestrator
  - Imports multiple project modules
  - Contains coordination logic between components
  - Decides "what" to do, delegating "how" to do it

#### 🌿 **Branches**
- **Intermediate Modules** (e.g., `gui/`, `core/`, `utils/`)
- **Characteristics:**
  - Medium complexity
  - Import other project modules
  - Provide specialized functionality
  - Abstract implementation details

#### 🍃 **Leaves**
- **Terminal Modules** (e.g., `button.py`, `validator.py`, `helpers.py`)
- **Characteristics:**
  - Simpler and more specific
  - **DO NOT import** files from the project itself
  - **DO import** external libraries (Numpy, Pandas, etc.)
  - Provide atomic functionality
  - Are reusable and independently testable

---

## 📊 Practical Example

### Hierarchical Structure

```python
# A.py (ROOT) - Main file
from B import feature_x
from C import feature_y

def main():
    """Orchestrator - coordinates B and C"""
    result_x = feature_x.process()
    result_y = feature_y.process()
    combine(result_x, result_y)
```

```python
# B.py (BRANCH) - Intermediate module
from D import validator
from E import transformer
from F import calculator

def feature_x():
    """Specialist - coordinates D, E, F"""
    data = validator.validate_input()
    transformed = transformer.transform(data)
    return calculator.compute(transformed)
```

```python
# D.py (LEAF) - Terminal module
import re  # Standard library
import numpy as np  # External library

def validate_input(data):
    """Atomic function - doesn't import project files"""
    pattern = re.compile(r'^\d+$')
    return np.array([x for x in data if pattern.match(x)])
```

### Characteristics by Level

| Level | File | Imports Project | Imports External | Complexity | Role |
|-------|------|-----------------|------------------|------------|------|
| 0 (Root) | A | B, C | Rarely | High | Orchestrator |
| 1 (Branch) | B, C | D, E, F, G | Sometimes | Medium | Coordinator |
| 2 (Leaf) | D, E, F, G | ❌ Never | ✅ Always | Low | Executor |

---

## 🔄 Development Approaches

### 🔽 Top-Down (From Top to Bottom)

**Starts from the root and descends to the leaves**

```
Process:
1. Define A (what the system does)
2. Identify needs (B, C)
3. Decompose B into (D, E, F)
4. Implement leaves (D, E, F, G)
```

**Advantages:**
- ✅ Clear architecture from the start
- ✅ Facilitates high-level planning
- ✅ Identifies dependencies early

**Disadvantages:**
- ❌ May create interfaces without implementation
- ❌ Makes initial testing difficult
- ❌ Risk of over-engineering

**Application Example:**
- Phase 3.0 refactoring followed top-down
- Started with `app.py` (root)
- Extracted specialized modules (branches/leaves)

---

### 🔼 Bottom-Up (From Bottom to Top)

**Starts from the leaves and rises to the root**

```
Process:
1. Implement D, E, F, G (basic components)
2. Combine into B, C (functionalities)
3. Orchestrate in A (complete system)
```

**Advantages:**
- ✅ Testable components from the start
- ✅ Natural reusability
- ✅ Less code waste

**Disadvantages:**
- ❌ Architecture emerges late
- ❌ Risk of non-integrable components
- ❌ Difficulty visualizing the whole

**Application Example:**
- Initial development of docks (leaves)
- Creation of utilities (`utils/`)
- Later integration in `MainWindow` (root)

---

### ↔️ Middle-Out (From Middle Outward)

**Starts from the branches and expands in both directions**

```
Process:
1. Identify central functionality (B)
2. ↓ Implement necessary components (D, E, F)
3. ↑ Create orchestrator (A)
4. Repeat for other functionalities (C, G)
```

**Advantages:**
- ✅ Balances overview and details
- ✅ Iterative and adaptable
- ✅ Reduces risk of both extreme approaches

**Disadvantages:**
- ❌ Requires experience to identify "the middle"
- ❌ Can create inconsistencies
- ❌ Requires frequent refactoring

**Application Example:**
- **Ideal phase for new modules**
- Start with functionality (e.g., `TranslatorDock`)
- Extract helpers as needed
- Integrate in `MainWindow` when stable

---

## 🎯 Design Principles

### 1. **Depth Principle**

> "The closer to the root, the more complex and orchestrating.  
> The closer to the leaves, the simpler and executing."

```
Root (A):     if condition: B.do() else: C.do()  ← Decision
Branch (B):   return D.compute(E.prepare(data))  ← Coordination
Leaf (D):     return sum(numbers) / len(numbers) ← Execution
```

### 2. **Independence Principle**

> "Leaves don't depend on other project leaves.  
> Leaves can only depend on external libraries."

❌ **Wrong:**
```python
# D.py (leaf)
from E import helper  # Dependency between leaves!
```

✅ **Correct:**
```python
# B.py (branch)
from D import function_d
from E import helper

def feature():
    return function_d(helper.prepare())  # Branch coordinates leaves
```

### 3. **Single Responsibility Principle**

> "Each level has its distinct role."

| Level | Responsibility | Question it Answers |
|-------|----------------|---------------------|
| Root | Orchestration | "What does the system do?" |
| Branch | Coordination | "How do the parts connect?" |
| Leaf | Execution | "How to do X specifically?" |

---

## 📏 Quality Metrics

### Good Architecture Indicators

✅ **Balanced Tree:**
- Depth of 2-4 levels
- Width proportional to complexity
- No leaves importing other leaves

✅ **Clear Separation:**
```
Root:  High complexity + Low execution
Leaf:  Low complexity + High execution
```

✅ **Ease of Testing:**
- Leaves testable in isolation
- Branches testable with mocks
- Root testable with integration

### Problem Indicators

❌ **Degenerate Tree (Linear):**
```
A → B → C → D → E → F  # Too deep!
```

❌ **Fat Leaves:**
```python
# D.py - 500 lines, imports E, F, G  # It's a branch, not a leaf!
```

❌ **Thin Root:**
```python
# A.py - 10 lines  # Should orchestrate more!
```

---

## 🔧 Practical Application Example

### Current State of a Project

```
app.py (2636 lines)
├── MainWindow (Root - 1555 lines)
│   ├── gui/preferences_dialog.py (Leaf)
│   ├── gui/settings_dialog.py (Leaf)
│   ├── gui/plugin_manager_dialog.py (Leaf)
│   ├── gui/layout_manager_dialog.py (Leaf)
│   ├── gui/ui_builder.py (Branch)
│   ├── gui/menu_builder.py (Branch)
│   ├── gui/initialization_manager.py (Branch)
│   └── gui/tab_manager.py (Branch)
├── DataView (330 lines - should be leaf)
└── DataProcessor (370 lines - should be leaf)
```

### Improvement Opportunities

**Extract to leaves:**
1. `DataView` → `gui/data_view.py`
2. `DataProcessor` → `processors/data_processor.py`

**Expected result:**
```
app.py (~1900 lines)
└── MainWindow (Root - adequate for orchestrator)
```

---

## 🌍 Universal Application

### Python
```python
# Root
from module import Class
# Branch
from .submodule import Helper
# Leaf
import numpy as np
```

### JavaScript
```javascript
// Root
import { Feature } from './feature';
// Branch
import { Component } from './components/component';
// Leaf
import React from 'react';
```

### Java
```java
// Root
import com.project.Module;
// Branch
import com.project.utils.Helper;
// Leaf
import java.util.ArrayList;
```

### C++
```cpp
// Root
#include "module.h"
// Branch
#include "utils/helper.h"
// Leaf
#include <vector>
```

---

## 📖 Conclusion

The **Tree Imports Analogy** provides a powerful mental model for:

1. **Understanding** existing architecture
2. **Planning** new modules
3. **Refactoring** code organically
4. **Communicating** design decisions

### Golden Rule

> **"The main file (root) should be the orchestrator, not the executor.  
> The simpler the leaf, the more reusable the code."**

---

## 🔗 References

- **Clean Architecture:** Robert C. Martin
- **Domain-Driven Design:** Eric Evans
- **Design Patterns:** Gang of Four
- **Refactoring:** Martin Fowler

---

**Living document:** This document should be updated as the architecture evolves.
