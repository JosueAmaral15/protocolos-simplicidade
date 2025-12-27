# Ordinal Task Organization - Simplicity Protocols

**Version**: 1.0  
**Creation Date**: December 27, 2025  
**Author**: Josué Amaral  
**Status**: ACTIVE

---

## 🎯 Objective

This document defines the **Ordinal Task Organization** system for the Simplicity Protocols, allowing human developers and artificial intelligences to quickly identify:

- ✅ **Execution order** of tasks (from simplest to most complex)
- ✅ **Dependencies** between tasks (which must be done first)
- ✅ **Parallelization** (which can be executed simultaneously)
- ✅ **Hierarchical organization** (tree/graph structure)

---

## 📊 Ordinal Prefix System

### Level 1: Simple Numbering (Independent Tasks)

For **independent** tasks that have **no dependencies** between them:

```markdown
1. Task A - Set up development environment
2. Task B - Create initial documentation
3. Task C - Define system architecture
```

**Characteristics**:
- ✅ Can be executed in **any order**
- ✅ Can be done **in parallel** in separate branches
- ✅ No dependency conflicts
- ✅ Sequential ascending numbering (1, 2, 3...)

---

### Level 2: Hierarchy with Letters (Task Groups)

To organize tasks into **logical groups** with **subgroups**:

```markdown
🔴 MUST HAVE - Release v1.0.0

A. Infrastructure and Configuration
   A.1. Create directory structure
   A.2. Configure project dependencies
   
B. Core - Data Structures
   B.1. Implement Node class
   B.2. Implement ExpressionTree
   
C. Core - Conversions
   C.1. Implement number → tree conversion
   C.2. Implement tree → RPN conversion
```

**Characteristics**:
- ✅ **Capital letter** = Group/Category
- ✅ **Number after letter** = Subtask within group
- ✅ Tasks from **different groups** (A, B, C) are **parallel**
- ✅ Tasks within the **same group** may have dependencies

---

### Level 3: Deep Hierarchy (Complex Dependencies)

For tasks with **explicit dependencies** in a **tree/graph** structure:

```markdown
A.C.1. Implement number → tree conversion
   ├─ Must be done AFTER A.1, A.2, C.1
   └─ Structure: A (root) → C (intermediate) → 1 (leaf)

B.C.2. Implement tree → RPN conversion
   B.C.2.1. RPN Parser (leaf - do FIRST)
   B.C.2.2. RPN Serializer (leaf - do FIRST)
   B.C.2. Implement conversion (parent - do AFTER 2.1 and 2.2)
```

**Reading the hierarchy** (⭐ CRITICAL):

The hierarchy should be read from **RIGHT to LEFT** (reverse order):

```
C.B.1.D.1
   │  │ │ └─ 1: Execute LAST (tree root)
   │  │ └─── D: Execute THIRD
   │  └───── 1: Execute SECOND
   └──────── B: Execute FIRST (tree leaf)

Execution order: B → 1 → D → 1 (right to left)
```

**Interpretation**:
- ✅ **Rightmost** = Ancestors (execute LAST)
- ✅ **Leftmost** = Descendants (execute FIRST)
- ✅ **Bottom-up organization**: Base → Top

**Practical Example**:

```markdown
C.B.1.D.1 - Integrate Dash with Cytoscape

Execution order (right → left):
1. FIRST:  Task D.1 (create basic Cytoscape component)
2. SECOND: Task 1.D (configure layout)
3. THIRD:  Task B.1 (implement data structure)
4. FOURTH: Task C (final Dash + Cytoscape integration)
```

---

## 🌳 Tree/Graph Structure

### Fundamental Concepts

#### 1. **Parent and Child Nodes**

```
B.C.2 (PARENT - execute AFTER)
   ├── B.C.2.1 (CHILD - execute BEFORE)
   └── B.C.2.2 (CHILD - execute BEFORE)
```

**Rule**: 
- ✅ **Children must be completed BEFORE parent**
- ✅ Children are **prerequisites** for parent
- ✅ Parent **depends** on children

#### 2. **Siblings (Parallel)**

```
B.C.2.1 (sibling)
B.C.2.2 (sibling)
```

**Rule**:
- ✅ Siblings can be executed **in parallel**
- ✅ No dependency between them
- ✅ Can be in **separate branches**

#### 3. **Cousins, Uncles, Grandparents (Parallel vs Serial)**

```
A. Group A
   A.1. Task A1
   A.2. Task A2
   
B. Group B
   B.1. Task B1
   B.2. Task B2
```

**Rule**:
- ✅ **Different groups** (A, B) = **PARALLEL** (execute simultaneously)
- ✅ **Cousins** (A.1 and B.1) = **PARALLEL**
- ✅ **Uncles/Nephews** (A and B.1) = **Evaluate explicit dependencies**

---

## 🔄 Parallelization vs Serialization

### PARALLEL Tasks (can be simultaneous)

✅ **When to parallelize**:
- Tasks from **different groups** (A.x, B.x, C.x)
- **Siblings** at the same level (X.1, X.2, X.3)
- **Cousins** (A.1 and B.1)
- Tasks **without explicit dependencies**

**Example**:
```markdown
✅ PARALLEL:
   A.1 (Create User model)
   B.1 (Create Product model)
   C.1 (Create graphical interface)
   
→ Can be done in 3 simultaneous branches
→ Zero conflicts
```

---

### SERIAL Tasks (must be sequential)

❌ **When to serialize**:
- Tasks with **parent-child relationship**
- Tasks with **explicit dependencies**
- When one task **uses the result** of another

**Example**:
```markdown
❌ SERIAL:
   B.C.2.1 (RPN Parser) ─┐
   B.C.2.2 (Serializer)  ├─→ B.C.2 (Complete conversion)
                         ┘
   
→ B.C.2.1 and B.C.2.2 MUST be completed BEFORE B.C.2
→ B.C.2 depends on results from 2.1 and 2.2
```

---

## 🎨 Practical Examples

### Example 1: Simple Project (Flat)

```markdown
# TASKS.md - Blog Project

## 🔴 MUST HAVE

1. 🔴🟢 [ ] Create Post model (Simple, 1h)
2. 🔴🟢 [ ] Create Comment model (Simple, 1h)
3. 🔴🟡 [ ] Implement Posts CRUD (Medium, 2h)
4. 🔴🟡 [ ] Implement Comments CRUD (Medium, 2h)

**Analysis**:
- Tasks 1 and 2 are PARALLEL (independent models)
- Task 3 depends on 1 (SERIAL)
- Task 4 depends on 2 (SERIAL)
- Tasks 3 and 4 are PARALLEL with each other

**Branch Strategy**:
- Branch 1: Implement 1 → 3
- Branch 2: Implement 2 → 4
```

---

### Example 2: Medium Project (Hierarchical)

```markdown
# TASKS.md - E-commerce System

## 🔴 MUST HAVE - Release v1.0.0

A. Authentication
   🔴🟡 [ ] A.1. Implement User model (Medium, 1.5h)
   🔴🟡 [ ] A.2. Implement JWT login (Medium, 2h)
   🔴🔴 [ ] A.3. Implement 2FA (Complex, 3h)

B. Product Catalog
   🔴🟢 [ ] B.1. Product model (Simple, 1h)
   🔴🟡 [ ] B.2. Products CRUD (Medium, 2h)
   🔴🟡 [ ] B.3. Search and filters (Medium, 2.5h)

C. Shopping Cart
   🔴🟢 [ ] C.1. Cart model (Simple, 1h)
   🔴🟡 [ ] C.2. Add/remove items (Medium, 1.5h)
   🔴🔴 [ ] C.3. Checkout (Complex, 4h)

**Dependency Analysis**:
- A.2 depends on A.1 (SERIAL: A.1 → A.2)
- A.3 depends on A.2 (SERIAL: A.2 → A.3)
- B.2 depends on B.1 (SERIAL: B.1 → B.2)
- B.3 depends on B.2 (SERIAL: B.2 → B.3)
- C.2 depends on C.1 (SERIAL: C.1 → C.2)
- C.3 depends on C.2 and A.2 (SERIAL: C.2, A.2 → C.3)

**Groups A, B, C are PARALLEL** (until C.3 which needs A.2)

**Branch Strategy**:
- Branch feat/auth: A.1 → A.2 → A.3
- Branch feat/catalog: B.1 → B.2 → B.3
- Branch feat/cart: C.1 → C.2
- Branch feat/checkout: C.3 (after merging auth and cart)
```

---

### Example 3: Complex Project (Deep Graph)

```markdown
# TASKS.md - Data Visualization Platform

## 🔴 MUST HAVE - Release v1.0.0

A. Infrastructure
   🔴🟢 [ ] A.1. Directory structure (Simple, 0.5h)
   🔴🟢 [ ] A.2. Dependencies (Simple, 0.5h)

B. Core - Structures
   🔴🟡 [ ] B.1. Node class (Medium, 1h)
       Depends: A.1, A.2
   🔴🟡 [ ] B.2. ExpressionTree (Medium, 1.5h)
       Depends: B.1

C. Conversions
   🔴🔴 [ ] A.C.1. Number → Tree (Complex, 2h)
       Depends: A.1, A.2, B.1, B.2
       Notation: A (infra) → C (conversion) → 1 (specific)
       
   🔴🟡 [ ] B.C.2. Tree → RPN (Medium, 2.5h)
       🔴🟡 [ ] B.C.2.1. RPN Parser (Medium, 1h)
           Depends: B.1, B.2
       🔴🟡 [ ] B.C.2.2. RPN Serializer (Medium, 1h)
           Depends: B.1, B.2
       🔴🟡 [ ] B.C.2. Complete conversion (Medium, 0.5h)
           Depends: B.C.2.1, B.C.2.2

D. Graphical Interface
   🔴🔴 [ ] C.B.1.D.1. Integrate Dash with Cytoscape (Complex, 2.5h)
       Reading right→left: D.1 → 1 → B → C
       Depends: B.1, B.2, C (conversions)
       
   🔴🔴 [ ] D.2. Drag-and-drop (Complex, 2h)
       Depends: C.B.1.D.1

**Recommended Execution Order**:

1. **Sprint 1** (PARALLEL - 3 branches):
   - Branch infra: A.1, A.2
   - Wait for merge

2. **Sprint 2** (PARALLEL - 2 branches):
   - Branch core: B.1 → B.2
   - Wait for merge

3. **Sprint 3** (PARALLEL - 3 branches):
   - Branch conversion-num: A.C.1
   - Branch parser: B.C.2.1
   - Branch serializer: B.C.2.2
   - Wait for merge of all 3

4. **Sprint 4** (SERIAL):
   - Branch conversion-rpn: B.C.2 (merge 2.1 and 2.2 first)

5. **Sprint 5** (SERIAL):
   - Branch gui-integration: C.B.1.D.1
   - Branch gui-drag: D.2 (after C.B.1.D.1)
```

---

## 📋 How to Decide Organization

### Decision Flowchart

```
┌─────────────────────────────────────┐
│ Does the task have dependencies?    │
└─────────────┬───────────────────────┘
              │
        ┌─────┴─────┐
        │           │
       YES         NO
        │           │
        │           ▼
        │     ┌───────────────────────┐
        │     │ Use simple numbering  │
        │     │ 1., 2., 3., ...       │
        │     │ (PARALLEL)            │
        │     └───────────────────────┘
        │
        ▼
  ┌─────────────────────────────┐
  │ Multiple complex            │
  │ dependencies?               │
  └─────────────┬───────────────┘
                │
          ┌─────┴─────┐
          │           │
         YES         NO
          │           │
          │           ▼
          │     ┌────────────────────────┐
          │     │ Use simple hierarchy   │
          │     │ A.1, A.2, B.1, B.2     │
          │     │ (PARALLEL GROUPS)      │
          │     └────────────────────────┘
          │
          ▼
    ┌──────────────────────────────┐
    │ Use deep hierarchy           │
    │ A.C.1, B.C.2.1, C.B.1.D.1    │
    │ (GRAPH - reading ←)          │
    └──────────────────────────────┘
```

---

## 🎯 Integration with Existing Classification System

The ordinal system **complements** (does not replace) existing classifications:

```markdown
🔴🟡 [ ] #3 B.1. Implement Node class (1h)
 │  │  │  │ └─ Ordinal prefix (dependencies)
 │  │  │  └─── Issue ID (#3)
 │  │  └────── Hierarchy (B = Group, 1 = Subtask)
 │  └───────── Complexity (🟡 Medium)
 └──────────── Priority (🔴 Must Have)

Reason: Base for all tree manipulation
Features: Binary tree node with operator/value
Tests: Unit tests for node creation
```

**Complete Legend**:
- **MoSCoW Priority**: 🔴 Must | 🟡 Should | 🟢 Could | ⚪ Won't
- **Complexity**: 🟢 Simple (0-1h) | 🟡 Medium (1-2h) | 🔴 Complex (>2h)
- **Status**: 🔴 Not Started | 🟡 In Progress | 🟢 Done | 🔵 Blocked
- **Ordinal Prefix**: Identifies execution order and dependencies

---

## ✅ Developer Checklist

When organizing tasks with ordinal system:

```markdown
- [ ] Identify independent tasks (simple numbering: 1, 2, 3)
- [ ] Group related tasks (hierarchy: A.1, A.2, B.1)
- [ ] Map explicit dependencies (graph: A.C.1, B.C.2.1)
- [ ] Define execution order (leaves → root, bottom-up)
- [ ] Identify parallelization opportunities (siblings, cousins)
- [ ] Plan branch strategy (1 branch per parallel group)
- [ ] Document complex dependencies (comments in TASKS.md)
- [ ] Validate that order is correct (children before parents)
- [ ] Communicate clearly to team members
- [ ] Update as dependencies change
```

---

## 🤖 Instructions for Artificial Intelligences

### When to Suggest Ordinal Organization

AI should suggest ordinal organization when:

✅ **Project has >10 tasks** with interdependencies
✅ **Multiple developers** working simultaneously
✅ **Blocking tasks** (one depends on another)
✅ **Risk of conflicts** in version control
✅ **Need for parallelization** to speed up development

### How AI Should Apply

1. **Analyze dependencies**:
   ```python
   # Pseudo-code
   tasks = read_tasks_md()
   graph = build_dependency_graph(tasks)
   order = topological_sort(graph)  # Bottom-up
   ```

2. **Identify parallel groups**:
   ```python
   parallel_groups = identify_independent_components(graph)
   ```

3. **Assign ordinal prefixes**:
   ```python
   for group in parallel_groups:
       letter = next_letter()  # A, B, C...
       for task in group:
           task.prefix = f"{letter}.{task.index}"
   ```

4. **Suggest branch strategy**:
   ```markdown
   Branch recommendation:
   - Branch feat/auth: A.1 → A.2 → A.3
   - Branch feat/api: B.1 → B.2 (parallel with auth)
   - Branch feat/ui: C.1 (wait for auth merge)
   ```

### Example AI Suggestion

```markdown
💡 **AI Suggestion**: I organized tasks with ordinal prefixes

Dependency analysis:
- Group A (Authentication): 3 SERIAL tasks
- Group B (API): 2 SERIAL tasks
- Group C (UI): 1 task, depends on A

Parallelization opportunities:
✅ Groups A and B can be developed simultaneously
✅ Total of 2 parallel branches → 40% time reduction

Recommended strategy:
1. Sprint 1 (parallel): Start A.1 and B.1
2. Sprint 2 (parallel): Continue A.2 and B.2
3. Sprint 3 (serial): A.3 (no parallel available)
4. Sprint 4 (serial): C.1 (waits for A)

Do you prefer this organization or would you like adjustments?
```

---

## 📖 References and Inspiration

This system was inspired by:

- ✅ **Dewey Decimal Notation** (libraries)
- ✅ **Topological Ordering** (graph algorithm)
- ✅ **Work Breakdown Structure (WBS)** (project management)
- ✅ **Dependency Graphs** (compilers, build systems)
- ✅ **Directory structures** (file systems)

---

## 🎯 Benefits of Ordinal System

### For Human Developers

✅ **Clarity**: Know exactly which task to do first
✅ **Autonomy**: No need to ask "can I start this?"
✅ **Efficiency**: Quickly identify parallel tasks
✅ **Organization**: Hierarchical structure facilitates navigation
✅ **Communication**: Team aligned on execution order

### For Artificial Intelligences

✅ **Algorithmic decision**: Can calculate order automatically
✅ **Optimization**: Suggest parallelization to accelerate development
✅ **Validation**: Detect circular dependencies
✅ **Planning**: Estimate total time considering parallel tasks
✅ **Prioritization**: Combine ordinal prefix with MoSCoW/Complexity

### For the Project

✅ **Speed**: Parallelization reduces total time
✅ **Quality**: Correct order avoids rework
✅ **Predictability**: More accurate timeline
✅ **Conflict reduction**: Isolated branches minimize merge conflicts
✅ **Traceability**: Documented dependency history

---

## 📝 Conclusion

The **Ordinal Task Organization** system is a powerful tool to:

1. **Organize** tasks from simplest to most complex
2. **Identify** dependencies and execution order
3. **Parallelize** development to accelerate deliveries
4. **Minimize** conflicts in version control
5. **Communicate** project structure clearly

Use this system when the project grows in complexity and the team needs to coordinate parallel development efforts.

---

**Version**: 1.0  
**Status**: ACTIVE  
**Maintained by**: Josué Amaral  
**Next review**: Based on community feedback
