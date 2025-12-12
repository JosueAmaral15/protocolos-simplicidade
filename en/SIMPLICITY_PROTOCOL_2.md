Aqui está a tradução do seu arquivo Markdown do português para o inglês:

```markdown
# Simplicity Protocol 2

**Author**: Josué Amaral
**Creation Date**: December 02, 2025
**Based on**: Simplicity Protocol 1 v2.0
**Version**: 2.2
**Last Update**: December 10, 2025
**Objective**: ADVANCED professional methodology for incremental quality development with a focus on security, performance, and continuous improvement

**Differences from Simplicity 1**:
- ✅ **10 new optional steps** for complex and critical projects
- ✅ Objective **Decision Matrix** for task selection
- ✅ **Security Checklist** (OWASP Top 10)
- ✅ **CI/CD with automatic Quality Gates**
- ✅ **ADR** (Architecture Decision Records)
- ✅ **Profiling and Optimization** for critical features
- ✅ Documented **Rollback Plans**
- ✅ **Sprint Retrospectives** (continuous improvement)
- ✅ **Peer Code Review** (if a team exists)
- ✅ **Accessibility Checklist** (GUI)

---

## 📊 Comparison of the 3 Protocols

| Aspect | Simplicity 1 | Simplicity 2 | Simplicity 3 |
|---|---|---|---|
| **Steps** | 13 mandatory | 13 mand + 10 opt | 16 mand + 3 opt |
| **Scenario** | Prototypes/internal | **Enterprise teams** | Solo in production |
| **Security** | ❌ No | ✅ OWASP mandatory | ✅ OWASP mandatory |
| **CI/CD** | ❌ No | ✅ Mandatory | ✅ Mandatory |
| **Rollback** | ❌ No | ✅ Mandatory | ✅ Mandatory |
| **Code Review** | ❌ No | ✅ **Peer mandatory** | ❌ Solo |
| **Retrospectives** | ❌ No | ✅ **Formal team** | ❌ Solo |
| **Accessibility** | ❌ No | ✅ WCAG 2.1 | ❌ Optional |
| **API Docs** | ❌ No | ✅ Formal Sphinx | ❌ Docstrings |
| **Overhead** | Low | **High** | Medium |
| **Production** | ❌ Not recommended | ✅ **Companies** | ✅ Solo devs |
| **Time/Task** | ~2-3h | ~4-6h | ~3-4h |
| **Best For** | Learning, prototyping | Large teams | Solo in production |

---

## 🎯 When to Use Each Protocol?

### **Simplicity Protocol 1** (13 mandatory steps)
**Use for**:
- ✅ Solo projects or small teams (1-3 devs)
- ✅ Simple to medium features
- ✅ Rapid prototyping
- ✅ First development of a functionality
- ✅ When speed is more important than perfection
- ✅ Non-critical internal projects

**Do not use for**:
- ❌ Critical production applications
- ❌ Systems with security requirements
- ❌ High-impact/high-risk features
- ❌ Projects with large teams (>5 devs)

### **Simplicity Protocol 2** (13 mandatory + 10 optional = 23 steps)
**Use for**:
- ✅ **Critical production applications** with a team
- ✅ Systems with **sensitive data** (LGPD, GDPR, PCI-DSS)
- ✅ **High-impact/high-risk features**
- ✅ Projects with **medium/large teams** (3+ devs)
- ✅ **Public Libraries/APIs** with multiple users
- ✅ Systems with critical **performance requirements**
- ✅ **Commercial/enterprise applications**
- ✅ Projects with **regulatory compliance** (ISO, SOC2)
- ✅ Code that requires **external audit**

**Do not use for**:
- ❌ **Rapid prototyping** (unnecessary overhead)
- ❌ **Disposable scripts** or single-use
- ❌ **Simple personal projects**
- ❌ **Solo developer** without a team → Use **Simplicity 3** (less overhead)
- ❌ **Non-critical internal apps** → Use **Simplicity 1**

**Rationale**: Simplicity 2 offers **maximum quality and security** through:
- **Peer Code Review**: Detects bugs that a solo developer might miss
- **Formal Retrospectives**: Continuous team improvement
- **Formal ADRs**: Documentation of architectural decisions for the long term
- **Accessibility WCAG**: Legal compliance for public apps
- **API Docs Sphinx**: Professional documentation for libraries

However, this rigor comes with a **cost**: ~4-6h per task vs ~2-3h in Simplicity 1. For a **solo developer**, this overhead doesn't pay off - use **Simplicity 3** which maintains production security without team bureaucracy.

---

**Changelog v2.2** (10/12/2025):
- ✅ **[COMPLEMENTATION]** Added comparative table of the 3 protocols (Simplicity 1/2/3)
- ✅ Expanded section "🎯 When to Use Simplicity 2?"
- ✅ Additional criteria: Regulatory compliance, external audit, solo dev (use S3)
- ✅ Detailed Rationale: Why code review/ADR/accessibility are worth the 4-6h overhead
- ✅ Comparison: Simplicity 2 vs 3 (team vs solo) with 12 aspects analyzed
- ✅ Inspiration: Concepts adapted from Simplicity 3 v3.1 (tables, criteria, rationale)

**Changelog v2.1** (09/12/2025):
- ✅ **[STEP 3]** Added recommendation for AI to provide suggestions and guesses for questions
- ✅ Recommended format: "❓ Question + 💡 AI Suggestion + Options A/B/C"
- ✅ Rationale: Accelerates decisions, reduces cognitive load, maintains consistency with existing code
- ✅ Classification: **OPTIONAL but HIGHLY RECOMMENDED**

**Changelog v2.0** (02/12/2025):
- ✅ **[NEW PROTOCOL]** Created Simplicity Protocol 2 based on Simplicity 1 v1.8
- ✅ **Step 2.5**: Decision Matrix for objective task selection (HIGH PRIORITY)
- ✅ **Step 6.5**: Security Checklist - OWASP Top 10 (HIGH PRIORITY)
- ✅ **Step 6.6**: Generate API Documentation (Sphinx/pdoc)
- ✅ **Step 8.5**: Accessibility Checklist - WCAG 2.1
- ✅ **Step 9.5**: Peer Code Review (Pull Request)
- ✅ **Step 10.5**: Profiling and Optimization (critical features)
- ✅ **Step 10.6**: Validate Quality Metrics - CI/CD (HIGH PRIORITY)
- ✅ **Step 11.5**: Create ADR (Architecture Decision Record)
- ✅ **Step 12.5**: Document Rollback Plan
- ✅ **Step 13.5**: Sprint Retrospective (continuous improvement)
- ✅ **Total**: 13 mandatory steps + 10 optional steps = 23 steps
- ✅ **Focus**: Security, Performance, Quality, Continuous Improvement

---

**Changelogs Inherited from Simplicity 1**:

**Changelog v1.8** (02/12/2025):
- ✅ **[REORGANIZATION]** Code Review integrated into CLI and GUI steps
- ✅ Step 7: Verify CLI Implementation (includes 9 quality criteria)
- ✅ Step 8: Verify GUI Implementation (includes 9 quality criteria)
- ✅ Step 9: Verify Integration with Main Program (maintained as a separate step)
- ✅ 9 Criteria: Omission, Ambiguity, Incorrect Fact, Redundancy, Inconsistency, Lack of Integration, Lower Cohesion, Higher Coupling, Strange Information
- ✅ Review integrated into the CLI/GUI verification process
- ✅ Total steps: 12 → 13 (added integration verification after GUI)

**Changelog v1.7** (02/12/2025):
- ✅ **[CRITICAL]** Added Step 8.5: Code Review (BEFORE testing)
- ✅ 9 Quality Criteria: Omission, Ambiguity, Incorrect Fact, Redundancy, Inconsistency, Lack of Integration, Lower Cohesion, Higher Coupling, Strange Information
- ✅ Complete review checklist (36 verification items)
- ✅ Recommended tools (pylint, vulture, radon, black, isort)
- ✅ Detailed CLI and GUI review process
- ✅ Practical examples of problems and corrections
- ✅ Integration with Step 9 (test after review)
- ✅ Total steps: 12 → 13 (8.5 added between 8 and 9)

**Changelog v1.6**:
- ✅ **[ADVANCED]** Added Step 9.2: Tests in Threads/Processes with Monitoring
- ✅ Execution of tests in a separate process (`multiprocessing.Process`)
- ✅ Real-time logging via `Queue` (progress of each test)
- ✅ Manual cancellation at any time (graceful Ctrl+C)
- ✅ Global + individual timeout (double protection)
- ✅ Real-time statistics (passed/failed/elapsed)
- ✅ Complete implementation of `test_runner_monitored.py` (~150 lines)
- ✅ Optional additional checklist (6 items)

**Changelog v1.5**:
- ✅ **[CRITICAL]** Added Step 9.1: Security in Tests
- ✅ 7 mandatory solutions to avoid infinite loops and timeouts
- ✅ Mandatory maximum timeout (30s per test)
- ✅ Mandatory headless environment for GUI tests (QT_QPA_PLATFORM=offscreen)
- ✅ Mandatory dry-run before executing tests (syntax + import + collect)
- ✅ Security checklist with 6 mandatory items
- ✅ Golden rules and safe commands documented
- ✅ Lessons learned from Task Example (infinite loop >1h)

**Changelog v1.4**:
- ✅ Reorganized final order: Implement → Integrate GUI → CLI → Test → Organize → Document → Commit
- ✅ Tests moved to AFTER integration checks (test integrated system)
- ✅ Organize root folder moved to BEFORE documentation (document clean state)
- ✅ Logic: Integrate → Test integration → Clean repository → Document final state

**Changelog v1.3**:
- ✅ Reorganized step order: GUI and CLI Integration Verification now come BEFORE Documentation
- ✅ New order: Tests → GUI Integration → CLI → Documentation → Organize → Commit
- ✅ Logic: Verifying integration before documenting ensures documentation reflects the actual state

**Changelog v1.2**:
- ✅ Added Step 8: Verify integration with main program
- ✅ Added Step 9: Verify CLI implementation with parameter passing
- ✅ Total steps: 10 → 12

---

## 🎯 Core Philosophy

> "There will always be complex tasks to do, but also those that are more difficult and those that are easier. **I want you to always start with the easier ones**."

**Principle**: From simple to complex, incremental, professional, and complete.

---

## 📋 Protocol Backbone (23 Steps: 13 Mandatory + 10 Optional)

### **Mandatory Steps** (Simplicity Protocol 1):
1. 📚 Read the documentation
2. ✅ Choose simpler tasks
3. ❓ Ask questions until 100% clarity
4. 🔍 Analyze and study the project
5. 🎯 Sprint the simpler tasks
6. 💻 Implement with professional architecture (GoF + GRASP)
7. ⌨️ Verify CLI Implementation + Code Review (9 criteria)
8. 🖥️ Verify GUI Implementation + Code Review (9 criteria)
9. 🔗 Verify Integration with Main Program
10. 🧪 Run tests (100% coverage)
11. 🧹 Organize project root folder
12. 📝 Fill in documentation
13. 🚀 Commit and push

### **Advanced Optional Steps** (Simplicity 2):
**2.5** 🎯 Decision Matrix (objective choice) - **HIGH PRIORITY**
**6.5** 🔒 Security Checklist (OWASP) - **HIGH PRIORITY**
**6.6** 📚 Generate API Documentation
**8.5** ♿ Accessibility Checklist (WCAG)
**9.5** 👥 Peer Code Review
**10.5** ⚡ Profiling and Optimization
**10.6** ✅ Quality Metrics (CI/CD) - **HIGH PRIORITY**
**11.5** 📋 Create ADR (Architectural Decision Records)
**12.5** 🔙 Rollback Plan
**13.5** 🔄 Sprint Retrospective

### 1️⃣ **Read the Documentation**
- Consult `TASKS.md` (or equivalent file defined by the user) to see pending tasks
- Consult `docs/REQUIREMENTS.md` to understand the project context
- Review previous specifications (`v2.9.X-SPECIFICATIONS.md`)
- Understand dependencies and existing architecture
- Check examples in `tests/files/` when applicable

**📋 About the Task File**:

The `TASKS.md` file is the **default file** for managing project tasks, but you can use any ASCII format file (`.txt`, `.md`, etc.) according to your preference.

**Task File Requirements**:
- ✅ **ASCII format mandatory**: `.md`, `.txt` or similar (readable as plain text)
- ❌ **NOT accepted**: `.docx`, `.pdf`, or binary formats
- 📍 **Location**: Project root or in `docs/` (e.g., `TASKS.md`, `TODO.md`, `requirements.md`)
- 🔄 **Alternative**: If you prefer another name/location, specify at project start

**If no task file exists**:
1. AI should ask the user: "Which file do you use to manage tasks?"
2. If none exists, suggest creating the default `TASKS.md`
3. Confirm file location and name with the user

**Why?**: Avoid rework and ensure coherence with existing code. The task file centralizes project planning and progress.

---

### 2️⃣ **Choose the Simplest Tasks**
- **Golden Rule**: Always start with the tasks **easiest to implement**
- Even in a list of complex tasks, **there are always some simpler than others**
- Proportionality: balance simplicity vs. impact

**Simplicity Criteria**:
- ✅ Fewer dependencies
- ✅ Well-defined and clear scope
- ✅ Fewer files to modify
- ✅ Lower risk of breaking existing functionalities
- ✅ Can be tested in isolation

**Real Example**:
```
List of remaining complex tasks:
[ ] Complex Feature Example (VERY COMPLEX - 50h)
[ ] Semantic AI Search (COMPLEX - 20h)
[ ] Tooltip preview on hover (SIMPLE - 30min) ✅ START HERE!
```

---

### 2️⃣.5️⃣ **Decision Matrix for Objective Task Selection** ⭐ NEW - HIGH PRIORITY

**Problem**: "Simplest" is subjective and can lead to incorrect choices
**Solution**: Objective scoring matrix with 5 quantifiable criteria

**Scoring Criteria** (0-5 points each):

1. **Technical Simplicity** (5=very simple, 0=very complex)
   - Amount of code needed
   - Algorithmic complexity
   - Amount of new concepts

2. **Dependencies** (5=zero dependencies, 0=many)
   - Files to modify
   - Modules that depend on this feature
   - External libraries required

3. **Impact** (5=high impact, 0=low)
   - Value for the end-user
   - Expected frequency of use
   - Benefit vs. effort

4. **Clarity of Requirements** (5=100% clear, 0=ambiguous)
   - Complete specification
   - Usage examples provided
   - Acceptance criteria defined

5. **Risk** (5=zero risk, 0=high risk)
   - Probability of breaking existing code
   - Reversibility of the change
   - Impact on critical features

**Prioritization Formula**:
```
Priority = (Simplicity × 2) + Dependencies + (Impact × 1.5) + Clarity + Risk

Maximum Score: 35 points
Minimum Score: 0 points
```

**Interpretation**:
- **30-35 points**: 🟢 IDEAL - Start immediately
- **20-29 points**: 🟡 GOOD - Strongly consider
- **10-19 points**: 🟠 MEDIUM - Evaluate context
- **0-9 points**: 🔴 COMPLEX - Leave for last

**Practical Application Example**:

| Task | Simpl<br>(0-5) | Dep<br>(0-5) | Imp<br>(0-5) | Clar<br>(0-5) | Risc<br>(0-5) | **Score** | **Decision** |
|---|---|---|---|---|---|---|---|
| **Tooltip Preview** | 5 | 5 | 3 | 5 | 5 | **33.5** 🟢 | **1st - START HERE** |
| **Feature** | 3 | 4 | 4 | 5 | 4 | **26.0** 🟡 | 2nd |
| **Integrated Editor** | 1 | 2 | 5 | 4 | 2 | **20.5** 🟡 | 3rd |
| **Semantic AI** | 0 | 1 | 4 | 2 | 1 | **10.0** 🟠 | 4th - Leave for last |

**"Tooltip Preview" Example Details**:
- **Simplicity: 5** - Just add QToolTip to existing widgets
- **Dependencies: 5** - Modify only 1 GUI file
- **Impact: 3** - Improves UX but not critical
- **Clarity: 5** - Requirement 100% clear (show preview on hover)
- **Risk: 5** - Zero risk of breaking anything (only adds tooltip)
- **Total: (5×2) + 5 + (3×1.5) + 5 + 5 = 33.5 points** 🟢

**Template for Filling**:
```markdown
## Decision Matrix - Sprint vX.X.X

| Task ID | Simplicity | Dependencies | Impact | Clarity | Risk | **Score** | Order |
|---|---|---|---|---|---|---|---|
| #XX | ? | ? | ? | ? | ? | **?** | ? |
| #YY | ? | ? | ? | ? | ? | **?** | ? |

**Justification for Choice**:
Task #XX chosen because:
- Highest score (XX points)
- [specific reason]
- [specific reason]
```

**When Not to Use the Matrix**:
- ❌ Only 1 task available (no choice)
- ❌ Urgent/blocking task (ignore score)
- ❌ Critical production bugfix (absolute priority)

**Why use it**:
- ✅ **Objectivity**: Eliminates personal bias
- ✅ **Traceability**: Justifies decisions
- ✅ **Learning**: Improves future estimates
- ✅ **Communication**: Easy to explain choice to the team

---

### 3️⃣ **Ask the Programmer Questions and More Questions**
- **CRITICAL**: Never assume or guess requirements
- Ask **all necessary questions** until **100% clarity**
- Validate understanding before starting implementation
- 🤖 **[NEW v2.1]** AI **CAN and IS HIGHLY RECOMMENDED** to provide **suggestions and guesses** for the answer to each question (optional, but encouraged)

**Recommended Question Format with Suggestions**:
```
❓ Question: "How should it behave when [scenario X]?"
💡 AI Suggestion: "Based on existing code, I suggest [option A] because [reason Y]."
Options: A) [option A] | B) [option B] | C) [option C]
```

**Why AI Suggestions Are Important**:
- ✅ Accelerates decisions when the programmer is undecided
- ✅ AI has context of existing code and can suggest consistent patterns
- ✅ Reduces programmer's cognitive load (they just validate, not create from scratch)
- ✅ Maintains quality: AI suggests based on already implemented best practices

**Question Categories**:
1. **Functional Requirements**:
   - "How should it behave when [scenario X]?"
   - "What happens if the user [action Y]?"
   - "What is the priority between [option A] and [option B]?"

2. **Technical Requirements**:
   - "Should I use [library X] or build from scratch?"
   - "What is the expected output format?"
   - "Are there any performance restrictions?"

3. **Edge Cases**:
   - "What if the file is empty?"
   - "What if there are special characters?"
   - "How to handle None/null values?"

4. **Integration**:
   - "Does it need to integrate with [existing module]?"
   - "Should I maintain compatibility with [previous version]?"
   - "Where should the results be saved?"

5. **Understanding Validation**:
   - "I understand you want [X]. Is that correct?"
   - "My proposed solution is [Y]. Does it make sense?"
   - "Can I start, or did I miss anything?"

**Real Example (Task Example)**:
```
❓ "Get first N words (how many? 3-5?)?"
✅ Answer: "Default can be 30 characters"

❓ "Convert to camelCase removing accents?"
✅ Answer: "Yes, accents should be removed"

❓ "Name conflicts: how to resolve?"
✅ Answer: "If they have the same parent key, don't touch. Smaller line wins."
```

**Why?**: Saves time, avoids rework, ensures the solution meets exactly what was requested.

---

### 4️⃣ **Analyze and Study the Project**
- **CRITICAL**: After clarifying all doubts, **study the code before implementing**
- Read relevant documentation (README, docs/, comments in code)
- Understand existing architecture and patterns used
- Check dependencies and necessary imports
- Identify reusable functions/classes

**Analysis Checklist**:
1. **Documentation Review**:
   - `docs/REQUIREMENTS.md` - General project context
   - `docs/SPECIFICATIONS.md` - Specifications of previous versions
   - `README.md` - Overview and usage instructions
   - Docstrings of related modules

2. **Existing Code Analysis**:
   - Find modules similar to what will be implemented
   - Identify design patterns already used (GoF, GRASP)
   - Check naming conventions and structure
   - Locate reusable helper functions

3. **Dependency Mapping**:
   - Which modules need to be imported?
   - Are there name or version conflicts?
   - Which base classes or mixins should be inherited?
   - Where should new files be created?

4. **Compatibility Validation**:
   - Will the solution break existing code?
   - Is it necessary to refactor something before implementing?
   - Are there tests that need to be updated?
   - Will the public API be maintained?

**Real Example (Task Example - Tutorials)**:
```
✅ Analyzed: Other docks (ComponentA, ComponentB)
✅ Identified: BaseDock pattern with FileInputMixin
✅ Verified: QTreeWidget + QTextBrowser for navigation
✅ Studied: How other modules convert markdown → HTML
✅ Located: Where to add imports in app.py
✅ Confirmed: Menu structure in _build_menu()
→ Result: Implementation in 2h instead of 5h (60% savings)
```

**Why?**: Avoids refactoring, saves time, ensures consistent code with the existing codebase.

---

### 5️⃣ **Sprint the Simplest Tasks**
- Group 2-4 related tasks into a sprint
- Estimate total time: **maximum 3-4 hours** per sprint
- Stay focused: **one sprint = one version (e.g., vX.Y.Z)**

**Sprint Structure**:
```
Sprint vX.Y.Z (Task Example):
├── Task Example: Feature Update (estimated 3h)
│   ├── Subtask 1: Ask programmer questions (15min)
│   ├── Subtask 2: extract_all_keys_from_obj() (45min)
│   ├── Subtask 3: build_substitution_map_by_value() (45min)
│   ├── Subtask 4: Integration into cli_dedupe() (30min)
│   ├── Subtask 5: Unit tests (60min)
│   └── Subtask 6: Documentation (30min)
└── Total: 3h45min ✅
```

---

### 6️⃣ **Implement from Simple to Complex with Professional Architecture**
- **Within each task**, start with the easiest part
- Build incrementally: helper function → main function → integration
- Test each part before moving on

**Implementation Order**:
1. **Helper functions** (e.g., `extract_all_keys_from_obj()`)
2. **Main functions** (e.g., `build_substitution_map_by_value()`)
3. **Integration** (e.g., update `cli_dedupe()`)
4. **GUI/UX** (if applicable)
5. **Optimizations** (last step)

**Architectural Principles (Mandatory)**:

#### 🔄 **Code Reusability with Modules**
- Create separate modules for each responsibility
- Avoid duplication (DRY - Don't Repeat Yourself)
- Generic functions reusable in multiple contexts

**Example**:
```python
# ✅ GOOD: Reusable module
# src/utils/file_utils.py
def read_file_safe(path: str) -> Optional[str]:
    """Function reused in 10+ places"""
    try:
        with open(path, 'r', encoding='utf-8') as f:
            return f.read()
    except Exception as e:
        logger.error(f"Error reading {path}: {e}")
        return None

# ❌ BAD: Duplicate code in each module
# (repeats try/except 20 times)
```

#### 📦 **Hierarchies and Encapsulation**
- Use classes when there is shared state
- Encapsulate private attributes (`_attribute`)
- Expose only necessary public interface

**Example**:
```python
# ✅ GOOD: Proper encapsulation
class ReferenceUpdater:
    def __init__(self, project_dir: str):
        self._project_dir = project_dir
        self._substitutions = {}
    
    def update_references(self) -> Dict[str, int]:
        """Clear public interface"""
        self._scan_files()  # Private method
        self._build_map()   # Private method
        return self._apply_changes()

# ❌ BAD: Everything exposed, no structure
def do_everything(dir, old, new, backup, ext):
    # 200 lines without organization
```

#### 🎯 **High Cohesion and Low Coupling**
- **High Cohesion**: Each module/class has a single, clear responsibility
- **Low Coupling**: Independent modules, communication via interfaces

**Example**:
```python
# ✅ HIGH COHESION: Each class does ONE thing
class KeyExtractor:
    """Only extracts keys from structures"""
    def extract(self, data) -> Dict[str, str]: ...

class SubstitutionMapBuilder:
    """Only builds substitution maps"""
    def build(self, old, new) -> Dict[str, str]: ...

class FileUpdater:
    """Only updates files"""
    def update(self, files, map) -> int: ...

# ✅ LOW COUPLING: Communication via interfaces
class ReferenceUpdater:
    def __init__(self, extractor: KeyExtractor, builder: SubstitutionMapBuilder):
        self._extractor = extractor  # Dependency injection
        self._builder = builder

# ❌ BAD: Low cohesion, high coupling
class EverythingManager:
    def do_all(self):
        # Does extraction + building + updating + logging + GUI
        # Imports 20 different modules
        # Impossible to test in isolation
```

#### 🏗️ **GoF (Gang of Four) Patterns**
Apply design patterns when appropriate:

1. **Strategy Pattern** (algorithm choice at runtime):
```python
class CaseConverter:
    def __init__(self, strategy: CaseStrategy):
        self._strategy = strategy
    
    def convert(self, text: str) -> str:
        return self._strategy.apply(text)

class CamelCaseStrategy(CaseStrategy):
    def apply(self, text: str) -> str: ...

class SnakeCaseStrategy(CaseStrategy):
    def apply(self, text: str) -> str: ...
```

2. **Factory Pattern** (creation of complex objects):
```python
class ProcessorFactory:
    @staticmethod
    def create(type: str) -> Processor:
        if type == "data":
            return DATAProcessor()
        elif type == "ts":
            return TypeScriptProcessor()
```

3. **Observer Pattern** (event notification):
```python
class ProcessingModal(QDialog):
    cancel_requested = Signal()  # Observer pattern
    
    def _on_cancel_clicked(self):
        self.cancel_requested.emit()  # Notifies observers
```

4. **Command Pattern** (undo/redo):
```python
class ReplaceCommand:
    def __init__(self, file: str, old: str, new: str):
        self._file = file
        self._old = old
        self._new = new
    
    def execute(self): ...
    def undo(self): ...
```

#### 🎨 **GRASP (General Responsibility Assignment Software Patterns) Patterns**

1. **Information Expert**: Assign responsibility to the one who has the information
```python
# ✅ GOOD: Dictionary has the info, so it has the method
class DataStore:
    def __init__(self, data: dict):
        self._data = data
    
    def get_value(self, key_path: str) -> Optional[str]:
        """Dictionary knows its structure"""
        return self._navigate_path(key_path)

# ❌ BAD: External class manipulates internal structure
def get_value_from_dict(dict_data, key_path):
    # Direct access to the internal structure of the dict
```

2. **Creator**: Class A creates B if A contains/aggregates B
```python
# ✅ GOOD: RewriterDock creates its own widgets
class ComponentB(BaseDock):
    def __init__(self):
        self._create_widgets()  # Creator pattern
        self._setup_layout()
    
    def _create_widgets(self):
        self.ed_input = QLineEdit()  # Creates its children
        self.btn_process = QPushButton()
```

3. **Controller**: Delegate system operations to controller
```python
# ✅ GOOD: Controller coordinates operations
class RewriterController:
    def process_file(self, path: str):
        data = self._reader.read(path)
        processed = self._processor.process(data)
        self._writer.write(path, processed)

# ❌ BAD: GUI does everything directly
class RewriterDock:
    def on_button_click(self):
        # 50 lines of business logic in the GUI
```

4. **Low Coupling**: Minimize dependencies
```python
# ✅ GOOD: Generic interface
def update_references(updater: ReferenceUpdater):
    """Accepts any updater that implements the interface"""
    updater.update()

# ❌ BAD: Concrete dependency
def update_references(file_path: str, backup: bool, ext: list):
    """Many parameters, high coupling"""
```

5. **High Cohesion**: One class, one responsibility
```python
# ✅ GOOD: High cohesion
class FileReader:
    """Only reads files"""
    def read(self, path: str) -> str: ...

class DataValidator:
    """Only validates data"""
    def validate(self, data: dict) -> bool: ...

# ❌ BAD: Low cohesion
class FileManager:
    def read(self): ...
    def write(self): ...
    def validate(self): ...
    def send_email(self): ...  # ?!
```

**Anti-pattern** ❌:
```python
# DO NOT do everything at once:
def complex_function_with_everything():
    # 500 lines of code
    # Multiple responsibilities
    # Difficult to test
    # High coupling
    # No reusability
```

**Correct Pattern** ✅:
```python
# Module: src/rewriter/key_extractor.py
class KeyExtractor:
    """High cohesion: only extracts keys"""
    def extract_from_obj(self, data) -> Dict[str, str]:
        return self._recurse(data, prefix='t')

# Module: src/rewriter/substitution_builder.py
class SubstitutionMapBuilder:
    """High cohesion: only builds maps"""
    def build_by_value(self, old, new) -> Dict[str, str]:
        return self._match_values(old, new)

# Module: src/rewriter/reference_updater.py
class ReferenceUpdater:
    """Low coupling: uses interfaces"""
    def __init__(self, extractor: KeyExtractor, builder: SubstitutionMapBuilder):
        self._extractor = extractor  # Dependency injection
        self._builder = builder
    
    def update_project(self, dir: str) -> Dict[str, int]:
        """Coordinates but doesn't implement everything"""
        old = self._extractor.extract(self._read_old())
        new = self._extractor.extract(self._read_new())
        map = self._builder.build_by_value(old, new)
        return self._apply_to_files(dir, map)
```

---

### 6️⃣.5️⃣ **Security Checklist (OWASP Top 10)** ⭐ NEW - HIGH PRIORITY

**When to Apply**: During Step 6 (Implementation) if the feature involves:
- ✅ User input (forms, CLI arguments, file uploads)
- ✅ File/operating system access
- ✅ Network connections (APIs, databases, external services)
- ✅ Authentication/authorization
- ✅ Sensitive data (passwords, tokens, PII)

**OWASP Top 10 Applied**:

**1. 🛡️ Injection (SQL, Command, Path Traversal)**
```python
# ❌ INSECURE - SQL Injection
query = f"SELECT * FROM users WHERE id = {user_id}"  # NEVER DO THIS!

# ✅ SECURE - Parameterized Query
query = "SELECT * FROM users WHERE id = ?"
cursor.execute(query, (user_id,))

# ❌ INSECURE - Command Injection
os.system(f"convert {filename} output.png")  # NEVER DO THIS!

# ✅ SECURE - List of arguments
subprocess.run(["convert", filename, "output.png"], check=True)

# ❌ INSECURE - Path Traversal
with open(user_path, 'r') as f:  # ../../../etc/passwd
    data = f.read()

# ✅ SECURE - Validate and restrict path
from pathlib import Path
safe_path = Path(user_path).resolve()
if not safe_path.is_relative_to(ALLOWED_DIR):
    raise SecurityError("Path traversal detected!")
data = safe_path.read_text()
```

**2. 🔐 Broken Authentication**
```python
# ❌ INSECURE - Plain text password
password = "admin123"  # NEVER DO THIS!

# ✅ SECURE - Hashing with salt
import bcrypt
hashed = bcrypt.hashpw(password.encode(), bcrypt.gensalt())

# ❌ INSECURE - Session without timeout
session['user_id'] = user_id  # Never expires

# ✅ SECURE - Session with timeout
session['user_id'] = user_id
session.permanent = True
app.permanent_session_lifetime = timedelta(hours=1)
```

**3. 🔓 Sensitive Data Exposure**
```python
# ❌ INSECURE - API key in code
API_KEY = "sk-1234567890abcdef"  # NEVER DO THIS!

# ✅ SECURE - Environment variables
import os
API_KEY = os.getenv('API_KEY')
if not API_KEY:
    raise ValueError("API_KEY not set!")

# ❌ INSECURE - Sensitive data log
logger.info(f"User logged in: {email}, password: {password}")

# ✅ SECURE - Log without sensitive data
logger.info(f"User logged in: {email}")
```

**4. 🌐 XML External Entities (XXE)**
```python
# ❌ INSECURE - XML parsing without protection
import xml.etree.ElementTree as ET
tree = ET.parse(user_file)  # Vulnerable to XXE

# ✅ SECURE - Disable external entities
import defusedxml.ElementTree as ET
tree = ET.parse(user_file)
```

**5. 🚪 Broken Access Control**
```python
# ❌ INSECURE - No permission check
def delete_file(file_id):
    file = File.query.get(file_id)
    file.delete()  # Any user can delete any file!

# ✅ SECURE - Check ownership
def delete_file(file_id, current_user):
    file = File.query.get(file_id)
    if file.owner_id != current_user.id:
        raise PermissionError("You don't own this file!")
    file.delete()
```

**6. ⚙️ Security Misconfiguration**
```python
# ❌ INSECURE - Debug mode in production
app = Flask(__name__)
app.debug = True  # NEVER in production!

# ✅ SECURE - Debug only in development
app.debug = os.getenv('FLASK_ENV') == 'development'

# ❌ INSECURE - Too open permissions
os.chmod(secret_file, 0o777)  # Everyone can read/write

# ✅ SECURE - Restrictive permissions
os.chmod(secret_file, 0o600)  # Only owner can read/write
```

**7. 🎨 Cross-Site Scripting (XSS)**
```python
# ❌ INSECURE - Unescaped HTML
html = f"<div>Hello {user_name}</div>"  # XSS if user_name = "<script>..."

# ✅ SECURE - HTML escaping
from html import escape
html = f"<div>Hello {escape(user_name)}</div>"

# ✅ BETTER - Template engine with auto-escape
return render_template('hello.html', name=user_name)  # Jinja2 automatically escapes
```

**8. 🔄 Insecure Deserialization**
```python
# ❌ INSECURE - pickle from untrusted source
import pickle
data = pickle.loads(user_data)  # Code execution!

# ✅ SECURE - DATA (does not execute code)
import data
data = data.loads(user_data)
```

**9. 📦 Using Components with Known Vulnerabilities**
```bash
# ❌ INSECURE - Outdated dependencies
# requirements.txt
flask==0.12.0  # Old version with vulnerabilities

# ✅ SECURE - Updated dependencies
pip install --upgrade flask
pip-audit  # Checks for vulnerabilities

# Automatic - GitHub Dependabot
# .github/dependabot.yml
version: 2
updates:
  - package-ecosystem: "pip"
    directory: "/"
    schedule:
      interval: "weekly"
```

**10. 📋 Insufficient Logging & Monitoring**
```python
# ❌ INSECURE - No security logs
def login(username, password):
    user = authenticate(username, password)
    return user  # Silent failure

# ✅ SECURE - Log security events
def login(username, password):
    try:
        user = authenticate(username, password)
        logger.info(f"Login success: {username} from {request.remote_addr}")
        return user
    except AuthenticationError:
        logger.warning(f"Login failed: {username} from {request.remote_addr}")
        raise
```

**Security Checklist**:
```markdown
### Security Checklist - [Feature Name]

#### Injection
- [ ] All inputs are sanitized/validated?
- [ ] Queries use parameterization?
- [ ] System commands use argument lists (not strings)?
- [ ] Paths are validated against path traversal?

#### Authentication & Sessions
- [ ] Passwords are hash + salt (bcrypt/argon2)?
- [ ] Sessions have timeouts?
- [ ] Tokens are generated with crypto.secrets (not random)?
- [ ] Login failures are logged?

#### Sensitive Data
- [ ] API keys/secrets in environment variables?
- [ ] Sensitive data is NOT logged?
- [ ] Connections use HTTPS/TLS?
- [ ] Data at rest is encrypted (if necessary)?

#### Access Control
- [ ] Permissions checked before each operation?
- [ ] User only accesses their own resources?
- [ ] Principle of least privilege applied?

#### Configuration
- [ ] Debug mode DISABLED in production?
- [ ] Error messages DO NOT expose stack traces to the user?
- [ ] Correct file permissions (0o600 for secrets)?

#### Dependencies
- [ ] All dependencies updated?
- [ ] pip-audit executed without vulnerabilities?
- [ ] Dependabot configured (if GitHub)?
```

**Security Tools**:
```bash
# Static security analysis
pip install bandit
bandit -r src/ -f data -o security-report.data

# Check for vulnerabilities in dependencies
pip install pip-audit
pip-audit

# Scan for secrets in code
pip install detect-secrets
detect-secrets scan > .secrets.baseline

# Pre-commit hook for security
# .pre-commit-config.yaml
repos:
  - repo: local
    hooks:
      - id: bandit
        name: Security check (bandit)
        entry: bandit -r src/
        language: system
      
      - id: secrets
        name: Detect secrets
        entry: detect-secrets-hook
        language: system
```

**Why this step is critical**:
- ✅ **LGPD/GDPR Compliance**: Avoids fines and lawsuits
- ✅ **Reputation**: Data breaches destroy trust
- ✅ **Cost**: Security bugs are 100x more expensive to fix in production
- ✅ **Legal**: Civil and criminal liability

---

### 6️⃣.6️⃣ **Generate API Documentation** (Optional - If creating a library/reusable module)

**When to Apply**:
- ✅ Module will be used by other developers
- ✅ Public/open-source library
- ✅ REST/GraphQL API
- ✅ SDK or plugin
- ✅ Complex functions that need examples

**Do Not Apply If**:
- ❌ Disposable internal code
- ❌ One-off scripts
- ❌ Rapid prototype

**Recommended Tools**:

**1. Sphinx** (Complete professional documentation)
```bash
# Install
pip install sphinx sphinx-rtd-theme

# Initialize
cd docs/
sphinx-quickstart

# Automatically generate from docstrings
sphinx-apidoc -o source/ ../src/

# Compile
make html

# Result: docs/build/html/index.html
```

**Configuration** (`docs/source/conf.py`):
```python
extensions = [
    'sphinx.ext.autodoc',       # Automatic docstrings
    'sphinx.ext.napoleon',      # Google/NumPy style docstrings
    'sphinx.ext.viewcode',      # Link to source code
    'sphinx.ext.intersphinx',   # Links to other docs
]

html_theme = 'sphinx_rtd_theme'  # Read the Docs theme
```

**2. pdoc** (Simple and fast documentation)
```bash
# Install
pip install pdoc

# Generate (serves with hot-reload)
pdoc --http : src/

# Generate static HTML
pdoc --html --output-dir docs/ src/

# Result: docs/src/index.html
```

**3. MkDocs** (Documentation in Markdown)
```bash
# Install
pip install mkdocs mkdocs-material

# Initialize
mkdocs new .

# Serve with hot-reload
mkdocs serve

# Build for production
mkdocs build

# Deploy to GitHub Pages
mkdocs gh-deploy
```

**Example of Complete Docstring**:
```python
def build_substitution_map_by_value(
    old_keys: Dict[str, str],
    new_keys: Dict[str, str]
) -> Dict[str, str]:
    """
    Build substitution map matching keys by their VALUES (not names).
    
    This function compares translation values between old and new DATA files
    to detect feature that need updating. It ignores key names and
    focuses solely on value equality.
    
    Args:
        old_keys: Dictionary mapping old key paths to their values.
            Example: {"t.welcome": "Welcome", "t.hello": "Hello"}
        new_keys: Dictionary mapping new key paths to their values.
            Example: {"t.greeting": "Welcome", "t.hi": "Hi"}
    
    Returns:
        Dictionary mapping old key paths to new key paths where values match.
        Example: {"t.welcome": "t.greeting"}  # Both have value "Welcome"
    
    Raises:
        ValueError: If old_keys or new_keys are empty.
        TypeError: If inputs are not dictionaries.
    
    Examples:
        >>> old = {"t.btn1": "Save", "t.btn2": "Cancel"}
        >>> new = {"t.save_btn": "Save", "t.cancel_btn": "Cancel"}
        >>> build_substitution_map_by_value(old, new)
        {'t.btn1': 't.save_btn', 't.btn2': 't.cancel_btn'}
        
        >>> old = {"t.msg": "Hello"}
        >>> new = {"t.greeting": "Hi"}  # Different value
        >>> build_substitution_map_by_value(old, new)
        {}  # No matches
    
    Notes:
        - Comparison is case-sensitive and exact
        - First match wins if multiple new keys have same value
        - Parent keys are not matched (only leaf values)
    
    See Also:
        - extract_all_keys_from_obj: Extract keys from DATA/Obj
        - apply_substitutions_to_file: Apply map to TSX files
    
    References:
        - Task Example: Feature Update System
        - FEATURE_SPEC.md
    
    Version:
        Added in vX.Y.Z
    """
    # Implementation...
```

**API Documentation Checklist**:
```markdown
### API Documentation - [Module Name]

#### Coverage
- [ ] All public functions have docstrings?
- [ ] All parameters documented?
- [ ] All returns documented?
- [ ] Possible exceptions listed?

#### Quality
- [ ] Usage examples included?
- [ ] Edge cases documented?
- [ ] Type hints present (PEP 484)?
- [ ] Docstrings follow standard (Google/NumPy)?

#### Accessibility
- [ ] API docs published (Read the Docs, GitHub Pages)?
- [ ] Tutorial/Getting Started included?
- [ ] Changelog maintained?
- [ ] Link to docs in README?
```

**Why**:
- ✅ **Adoption**: Good docs = more users
- ✅ **Support**: Fewer repetitive questions
- ✅ **Onboarding**: New devs understand faster
- ✅ **Professionalism**: Shows project quality

---

### 7️⃣ **Verify CLI Implementation + Code Review**
- **CRITICAL**: Verify that the new functionality is available via **CLI (Command Line Interface)**
- **IMPORTANT**: During verification, apply the **9 Quality Criteria** to the CLI code
- It's not enough to implement a GUI, important functionalities must have a **CLI interface** for automation
- Verify subcommands, arguments, help text, integration, and code quality

**CLI Implementation Checklist**:

1. **Correct Import in app.py**:
   ```python
   # ✅ Verify if module was imported
   from .gui import (
       ComponentJ, ComponentK, ComponentI,
       ComponentC, ComponentD, ComponentA,
       ComponentB, ComponentF, ComponentG, ComponentH,
       ComponentE, NewComponent  # ← NEW module should be here
   )
   ```

2. **Export in Module's __init__.py**:
   ```python
   # src/gui/__init__.py
   from .text_to_data_dock import NewComponent
   
   __all__ = [
       'ComponentJ', 'ComponentK', 'ComponentI',
       'ComponentC', 'ComponentD', 'ComponentA',
       'ComponentB', 'ComponentF', 'ComponentG', 'ComponentH',
       'ComponentE', 'NewComponent'  # ← NEW module exported
   ]
   ```

3. **Menu Item Created and Connected**:
   ```python
   # In _build_menu() or similar
   m_tools = bar.addMenu(tr("menu.tools"))
   
   # Create QAction
   self.act_open_new_component = QAction(tr("menu.tools.text_to_data"), self)
   
   # Add to menu
   m_tools.addAction(self.act_open_new_component)
   
   # Connect signal
   self.act_open_new_component.triggered.connect(lambda: self.dock_new_component.show())
   ```

4. **Dock Initialized in __init__() or setup method**:
   ```python
   # In __init__() of MainWindow
   def __init__(self):
       super().__init__()
       # ... other docks ...
       self._open_new_component()  # ← Initialize dock
   
   def _open_new_component(self):
       self.dock_new_component = NewComponent(self)
       self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
       self.addDockWidget(Qt.RightDockWidgetArea, self.dock_new_component)
       self.dock_new_component.hide()
   ```

5. **Signals Connected** (if applicable):
   ```python
   # Connect custom signals
   self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
   
   def _load_data_from_source(self, data_str: str):
       """Callback to open DATA in editor"""
       if not hasattr(self, 'component_viewer'):
           self._open_component()
       self.component_viewer.load_data_string(data_str)
       self.component_viewer.show()
   ```

6. **i18n Translations Added**:
   ```data
   // src/i18n/en.data
   {
     "menu.tools.text_to_data": "Text to DATA Converter"
   }
   
   // src/i18n/pt_BR.data
   {
     "menu.tools.text_to_data": "Conversor de Texto para DATA"
   }
   ```

**Integration Test Checklist**:
- ✅ **Accessible menu**: Verify if item appears in the Tools menu
- ✅ **Dock opens**: Clicking the menu should open the dock correctly
- ✅ **Basic functionality**: Test simple conversion
- ✅ **Signals work**: Test integration with other components (e.g., Open in Editor)
- ✅ **No console errors**: There should be no ImportError, AttributeError, etc.
- ✅ **Translation working**: Menu in PT-BR should show translated text

**Real Example (Task Example - Text to DATA Converter)**:
```python
✅ Import: from .gui import NewComponent
✅ Export: __all__ = [..., 'NewComponent']
✅ Menu: self.act_open_new_component = QAction(tr("menu.tools.text_to_data"), self)
✅ Init: self._open_new_component() called in __init__()
✅ Signal: open_in_other_component_requested.connect(self._load_data_from_source)
✅ i18n: EN "Text to DATA Converter", PT-BR "Conversor de Texto para DATA"
✅ Test: Menu opens dock, conversion works, signal to editor OK
```

**Questions to Validate Integration**:
1. ❓ "Is the new module imported in the main file (app.py)?"
2. ❓ "Is the module exported in the folder's __init__.py?"
3. ❓ "Is there a menu item to access the functionality?"
4. ❓ "Is the menu item connected to the correct method?"
5. ❓ "Is the dock/component initialized at application startup?"
6. ❓ "Are custom signals connected?"
7. ❓ "Were translations added (EN and PT-BR)?"
8. ❓ "Is the functionality accessible without errors?"

**Why?**: Ensure that the implemented code is **actually usable** by the end-user, not just "works in isolation."

---

### 8️⃣ **Verify GUI Implementation + Code Review**
- **CRITICAL**: Verify that components are **integrated into the main program** and accessible
- **IMPORTANT**: During verification, apply the **9 Quality Criteria** to the GUI code
- It's not enough to implement the module/dock, it needs to be **accessible and functional** in the app
- Verify menu, imports, initialization, connections, and code quality

**Part A - Functional GUI Verification (Integration)**:

1. **Correct Import in app.py**:
   ```python
   # ✅ Verify if module was imported
   from .gui import (
       ComponentJ, ComponentK, ComponentI,
       ComponentC, ComponentD, ComponentA,
       ComponentB, ComponentF, ComponentG, ComponentH,
       ComponentE, NewComponent  # ← NEW module should be here
   )
   ```

2. **Export in Module's __init__.py**:
   ```python
   # src/gui/__init__.py
   from .text_to_data_dock import NewComponent
   
   __all__ = [
       'ComponentJ', 'ComponentK', 'ComponentI',
       'ComponentC', 'ComponentD', 'ComponentA',
       'ComponentB', 'ComponentF', 'ComponentG', 'ComponentH',
       'ComponentE', 'NewComponent'  # ← NEW module exported
   ]
   ```

3. **Menu Item Created and Connected**:
   ```python
   # In _build_menu() or similar
   m_tools = bar.addMenu(tr("menu.tools"))
   
   # Create QAction
   self.act_open_new_component = QAction(tr("menu.tools.text_to_data"), self)
   
   # Add to menu
   m_tools.addAction(self.act_open_new_component)
   
   # Connect signal
   self.act_open_new_component.triggered.connect(lambda: self.dock_new_component.show())
   ```

4. **Dock Initialized in __init__() or setup method**:
   ```python
   # In __init__() of MainWindow
   def __init__(self):
       super().__init__()
       # ... other docks ...
       self._open_new_component()  # ← Initialize dock
   
   def _open_new_component(self):
       self.dock_new_component = NewComponent(self)
       self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
       self.addDockWidget(Qt.RightDockWidgetArea, self.dock_new_component)
       self.dock_new_component.hide()
   ```

5. **Signals Connected** (if applicable):
   ```python
   # Connect custom signals
   self.dock_new_component.open_in_other_component_requested.connect(self._load_data_from_source)
   
   def _load_data_from_source(self, data_str: str):
       """Callback to open DATA in editor"""
       if not hasattr(self, 'component_viewer'):
           self._open_component()
       self.component_viewer.load_data_string(data_str)
       self.component_viewer.show()
   ```

6. **i18n Translations Added**:
   ```data
   // src/i18n/en.data
   {
     "menu.tools.text_to_data": "Text to DATA Converter"
   }
   
   // src/i18n/pt_BR.data
   {
     "menu.tools.text_to_data": "Conversor de Texto para DATA"
   }
   ```

**GUI Integration Test Checklist**:
- ✅ **Accessible menu**: Verify if item appears in the Tools menu
- ✅ **Dock opens**: Clicking the menu should open the dock correctly
- ✅ **Basic functionality**: Test simple conversion
- ✅ **Signals work**: Test integration with other components (e.g., Open in Editor)
- ✅ **No console errors**: There should be no ImportError, AttributeError, etc.
- ✅ **Translation working**: Menu in PT-BR should show translated text

**Part B - GUI Code Quality Review (9 Criteria)**:

During GUI verification, simultaneously apply the following criteria:

1. **❌ Omission** - Verify if GUI is complete:
   - [ ] All necessary widgets/controls implemented?
   - [ ] Error handling in handlers (e.g., FileNotFoundError)?
   - [ ] Resource cleanup (close files, disconnect signals)?
   - [ ] Visual feedback for long operations (QProgressBar, busy cursor)?

2. **🤔 Ambiguity** - GUI should be clear:
   - [ ] Descriptive and clear labels?
   - [ ] Informative tooltips on controls?
   - [ ] Descriptive error messages (QMessageBox)?
   - [ ] Intuitive method names (_on_button_clicked vs _handle)?

3. **❗ Incorrect Fact** - Correct GUI logic:
   - [ ] Signals connected to correct slots?
   - [ ] Correct layouts (QVBoxLayout, QHBoxLayout, QSplitter)?
   - [ ] Enable/disable controls according to state?
   - [ ] Correct input validation (QValidator)?

4. **♻️ Redundancy** - Avoid repetition in GUI:
   - [ ] Widgets created only once?
   - [ ] Validations centralized (not duplicated)?
   - [ ] Initialization code not repeated?

5. **⚠️ Inconsistency** - Consistent GUI pattern:
   - [ ] Uniform nomenclature (ed_ for QLineEdit, btn_ for QPushButton)?
   - [ ] Consistent message style?
   - [ ] Consistent layout spacing/margin?

6. **🔗 Lack of Integration** - GUI connected:
   - [ ] Dock added to MainWindow?
   - [ ] Menu item connected to dock.show()?
   - [ ] Custom signals connected?
   - [ ] Import present in app.py?

7. **🧩 Lower Cohesion** - Focused dock:
   - [ ] Dock only does UI (not business logic)?
   - [ ] Complex logic in separate module?
   - [ ] Each method has a single responsibility?

8. **🔗 Higher Coupling** - Decoupled GUI:
   - [ ] Dock does not depend on internal implementation of other docks?
   - [ ] Communication via signals/slots (not direct calls)?
   - [ ] GUI independently testable (mock logic)?

9. **🗑️ Strange Information** - Clean code:
   - [ ] No forgotten print() debugs?
   ] No unresolved TODOs?
   - [ ] No unused widgets?

**Example of Applied GUI Review**:
```python
# ❌ BEFORE - Omission, Ambiguity, Higher Coupling
class NewComponent(QDockWidget):
    def __init__(self):
        self.btn = QPushButton("Convert")  # Vague label
        self.btn.clicked.connect(self.convert)  # No error handling
    
    def convert(self):
        data = open(self.ed_file.text()).read()  # No validation, no close
        data_str = my_convert(data)  # Business logic in GUI
        print(data_str)  # Forgotten debug

# ✅ AFTER - Complete, Clear, Decoupled
class NewComponent(BaseDock):
    """Text to DATA Converter dock widget."""
    
    # Signal for communication
    open_in_other_component_requested = Signal(str)
    
    def __init__(self, parent=None):
        super().__init__(parent)
        self._create_widgets()
        self._setup_layout()
        self._connect_signals()
        
        # Controller for business logic
        self._converter = TextToJsonConverter()
    
    def _create_widgets(self):
        """Create UI widgets."""
        self.ed_file = QLineEdit()
        self.ed_file.setPlaceholderText("Enter file path or paste text")
        
        self.btn_convert = QPushButton("Convert to DATA")
        self.btn_convert.setToolTip("Convert text to DATA format")
        
        self.btn_open_component = QPushButton("Open in Editor")
        self.btn_open_component.setEnabled(False)  # Disabled until converted
    
    def _connect_signals(self):
        """Connect signals to slots."""
        self.btn_convert.clicked.connect(self._on_convert_clicked)
        self.btn_open_component.clicked.connect(self._on_open_component_clicked)
    
    def _on_convert_clicked(self):
        """Handle convert button click."""
        file_path = self.ed_file.text().strip()
        
        if not file_path:
            QMessageBox.warning(self, "Empty Input", "Please enter a file path or text.")
            return
        
        try:
            # Read file with context manager (ensures close)
            if Path(file_path).exists():
                with open(file_path, 'r', encoding='utf-8') as f:
                    text = f.read()
            else:
                text = file_path  # Treat as direct text
            
            # Convert using controller (decoupling)
            self._data_result = self._converter.convert(text)
            
            # Visual feedback
            QMessageBox.information(self, "Success", "Conversion successful!")
            self.btn_open_component.setEnabled(True)
        
        except FileNotFoundError:
            QMessageBox.critical(self, "File Not Found", f"File not found: {file_path}")
        except Exception as e:
            QMessageBox.critical(self, "Conversion Error", f"Error: {str(e)}")
    
    def _on_open_component_clicked(self):
        """Handle open in editor button click."""
        if hasattr(self, '_data_result'):
            self.open_in_other_component_requested.emit(self._data_result)  # Signal
```

**Recommended GUI Tools**:
```bash
# Check unused Qt imports
grep -r "from PySide6" src/gui/ | cut -d: -f2 | sort | uniq

# Check unconnected signals (manual review)
grep -r "Signal(" src/gui/ | grep -v ".connect("

# Check unused widgets (manual review)
grep -r "self\.\w\+ = Q" src/gui/

# Check debug prints (CRITICAL)
grep -r "print(" src/gui/ --exclude="*_test.py"
```

**Questions to Validate GUI**:
1. ❓ "Is the dock fully integrated into the menu and MainWindow?"
2. ❓ "Are all signals connected and working?"
3. ❓ "Is there error handling with visual feedback (QMessageBox)?"
4. ❓ "Is business logic separated from GUI code?"
5. ❓ "Is the code free of debug prints and unresolved TODOs?"
6. ❓ "Are labels, tooltips, and messages clear and descriptive?"
7. ❓ "Are resources (files, connections) closed correctly?"

**Real Example (Task Example - Text to DATA Converter)**:
```python
✅ Import: from .gui import NewComponent
✅ Export: __all__ = [..., 'NewComponent']
✅ Menu: self.act_open_new_component.triggered.connect(lambda: self.dock_new_component.show())
✅ Init: self._open_new_component() called in __init__()
✅ Signal: open_in_other_component_requested.connect(self._load_data_from_source)
✅ i18n: EN "Text to DATA Converter", PT-BR "Conversor de Texto para DATA"
✅ Review: No debug prints, error handling OK, logic decoupled
✅ Test: Menu opens dock, conversion works, signal to editor OK
```

---

### 8️⃣.5️⃣ **Accessibility Checklist (WCAG 2.1)** (Optional - For GUIs)

**When to Apply**:
- ✅ Desktop applications with GUI
- ✅ Web applications
- ✅ Tools used by diverse teams
- ✅ Open-source projects
- ✅ Compliance with accessibility laws

**Do Not Apply If**:
- ❌ CLI/backend only
- ❌ Internal script for personal use
- ❌ Non-public prototype

**WCAG 2.1 Level AA - POUR Principles**:

**1. Perceivable - Users must perceive the information**

```python
# ✅ ACCESSIBLE - Descriptive labels
self.btn_save = QPushButton("Save File")
self.btn_save.setToolTip("Save current file to disk (Ctrl+S)")
self.btn_save.setAccessibleName("Save file button")
self.btn_save.setAccessibleDescription("Saves the current file to disk")

# ❌ NOT ACCESSIBLE - No context
self.btn = QPushButton("OK")  # OK for what?
self.btn.setToolTip("OK")     # Doesn't help
```

**2. Operable - Users must operate the interface**

```python
# ✅ ACCESSIBLE - Keyboard navigation
self.ed_input.setFocusPolicy(Qt.StrongFocus)
self.btn_save.setShortcut(QKeySequence("Ctrl+S"))
self.btn_cancel.setShortcut(QKeySequence("Esc"))

# Visual focus indicator
self.ed_input.setStyleSheet("""
    QLineEdit:focus {
        border: 2px solid #0078d4;
        background-color: #f0f8ff;
    }
""")

# ❌ NOT ACCESSIBLE - Mouse only
self.btn.clicked.connect(self.on_click)  # No keyboard shortcut
```

**3. Understandable - Information and operation must be understandable**

```python
# ✅ ACCESSIBLE - Clear error messages
QMessageBox.critical(
    self,
    "File Not Found",
    f"The file '{filename}' could not be found.\n\n"
    f"Please check:\n"
    f"• The file path is correct\n"
    f"• You have read permissions\n"
    f"• The file was not deleted"
)

# ❌ NOT ACCESSIBLE - Generic error
QMessageBox.critical(self, "Error", "Operation failed")
```

**4. Robust - Content must be robust for assistive technologies**

```python
# ✅ ACCESSIBLE - Roles and relationships
self.lbl_name = QLabel("Name:")
self.ed_name = QLineEdit()
self.lbl_name.setBuddy(self.ed_name)  # Associates label with input

# Group related
self.group_personal = QGroupBox("Personal Information")
self.group_personal.setAccessibleName("Personal information group")

# ❌ NOT ACCESSIBLE - No structure
# Just loose widgets without semantic relationship
```

**WCAG 2.1 Accessibility Checklist**:

```markdown
### Accessibility Checklist - [GUI Name]

#### 1. Perceivable
- [ ] **Contrast**: Colors have minimum contrast 4.5:1 (normal text)?
- [ ] **Contrast**: Colors have minimum contrast 3:1 (large text >18pt)?
- [ ] **Alternatives**: Icons have descriptive tooltips?
- [ ] **Labels**: All inputs have associated labels?
- [ ] **Colors**: Information does not depend only on color?
- [ ] **Size**: Text is resizable (up to 200%)?

#### 2. Operable
- [ ] **Keyboard**: All functions accessible via keyboard?
- [ ] **Tab Order**: Navigation order makes sense?
- [ ] **Focus**: Focused element has clear visual indication?
- [ ] **Shortcuts**: Important commands have keyboard shortcuts?
- [ ] **Esc**: Dialogs can be closed with Esc?
- [ ] **Enter**: Enter submits forms/confirms actions?
- [ ] **Time**: No unexpected timeouts?

#### 3. Understandable
- [ ] **Language**: Content language is defined (i18n)?
- [ ] **Labels**: Input labels are clear?
- [ ] **Instructions**: Complex inputs have instructions?
- [ ] **Errors**: Error messages are specific and actionable?
- [ ] **Help**: Help/documentation easily accessible?
- [ ] **Navigation**: Menus have a logical structure?

#### 4. Robust
- [ ] **Screen Reader**: Tested with screen reader (NVDA/Orca)?
- [ ] **Semantics**: Correct widgets (QPushButton vs QLabel)?
- [ ] **Roles**: AccessibleName and AccessibleDescription defined?
- [ ] **Relationships**: Labels associated with buddy()?
- [ ] **Groups**: Related controls grouped (QGroupBox)?
```

**Practical Test with Screen Reader**:

```bash
# Linux - Install Orca
sudo apt install orca

# Start screen reader
orca --replace &

# Test application:
# 1. Navigate with Tab (should read each element)
# 2. Press Enter/Space (should activate buttons)
# 3. Fill forms (should read labels correctly)
# 4. Activate shortcuts (Ctrl+S, Esc, etc.)

# Windows - Use NVDA (free)
# https://www.nvaccess.org/download/

# macOS - VoiceOver (native)
# Cmd+F5 to activate
```

**Validation Tools**:

```bash
# Check color contrast
pip install color-contrast-checker
color-contrast-checker --foreground "#333333" --background "#ffffff"
# Result: AAA (passes all levels)

# Web accessibility analyzer (if applicable)
npm install -g pa11y
pa11y http://localhost:8000

# Lighthouse (Chrome DevTools)
# Audits → Accessibility → Generate Report
```

**Example of Accessible GUI**:

```python
class AccessibleConverterDock(QDockWidget):
    """Accessible text to DATA converter with WCAG 2.1 Level AA compliance."""
    
    def __init__(self, parent=None):
        super().__init__("Text to DATA Converter", parent)
        self.setAccessibleName("Text to DATA Converter Dock")
        self.setAccessibleDescription(
            "Convert structured text files to DATA format with preview"
        )
        self._create_accessible_widgets()
        self._setup_shortcuts()
    
    def _create_accessible_widgets(self):
        # Label + Input with buddy
        self.lbl_input = QLabel("&Input File:")
        self.ed_input = QLineEdit()
        self.ed_input.setAccessibleName("Input file path")
        self.ed_input.setAccessibleDescription("Enter path to text file to convert")
        self.ed_input.setPlaceholderText("e.g., data.csv or config.ini")
        self.lbl_input.setBuddy(self.ed_input)  # Alt+I focuses input
        
        # Button with tooltip and shortcut
        self.btn_convert = QPushButton("&Convert to DATA")
        self.btn_convert.setAccessibleName("Convert button")
        self.btn_convert.setAccessibleDescription(
            "Convert input file to DATA format. Shortcut: Ctrl+Enter"
        )
        self.btn_convert.setToolTip("Convert text to DATA (Ctrl+Enter)")
        self.btn_convert.setShortcut(QKeySequence("Ctrl+Return"))
        
        # Focus indicator
        self.btn_convert.setStyleSheet("""
            QPushButton:focus {
                border: 2px solid #0078d4;
                outline: 2px solid #0078d4;
                outline-offset: 2px;
            }
        """)
        
        # Group for semantic organization
        self.group_options = QGroupBox("Conversion &Options")
        self.group_options.setAccessibleName("Conversion options group")
        
        self.chk_pretty = QCheckBox("&Pretty print DATA")
        self.chk_pretty.setAccessibleName("Pretty print option")
        self.chk_pretty.setAccessibleDescription(
            "Format DATA with indentation for readability"
        )
        self.chk_pretty.setToolTip("Format DATA with indentation")
        
        # High contrast for status
        self.lbl_status = QLabel("Ready")
        self.lbl_status.setAccessibleName("Conversion status")
        self.lbl_status.setStyleSheet("""
            QLabel {
                color: #000000;
                background-color: #f0f0f0;
                padding: 4px;
                border: 1px solid #cccccc;
                font-weight: bold;
            }
        """)
    
    def _setup_shortcuts(self):
        """Configure keyboard shortcuts for accessibility."""
        # Esc closes the dock
        self.shortcut_close = QShortcut(QKeySequence("Esc"), self)
        self.shortcut_close.activated.connect(self.close)
        
        # F1 opens help
        self.shortcut_help = QShortcut(QKeySequence("F1"), self)
        self.shortcut_help.activated.connect(self._show_help)
    
    def _show_help(self):
        """Show accessible help dialog."""
        QMessageBox.information(
            self,
            "Text to DATA Converter - Help",
            "<h3>Keyboard Shortcuts</h3>"
            "<ul>"
            "<li><b>Ctrl+Enter</b>: Convert file</li>"
            "<li><b>Alt+I</b>: Focus input field</li>"
            "<li><b>Alt+O</b>: Toggle options group</li>"
            "<li><b>Esc</b>: Close dock</li>"
            "<li><b>F1</b>: Show this help</li>"
            "</ul>"
            "<h3>Screen Reader Support</h3>"
            "<p>This interface is fully accessible with screen readers.</p>"
        )
```

**Why this step is important**:
- ✅ **Inclusion**: ~15% of the population has some disability
- ✅ **Legal**: ADA, Section 508, EN 301 549 may require it
- ✅ **UX**: Good accessibility = good UX for everyone
- ✅ **SEO**: Accessibility improves rankings (if web)
- ✅ **Reputation**: Shows social responsibility

---

### 9️⃣ **Verify Integration with Main Program**
- **CRITICAL**: After implementing CLI and GUI, **verify that everything is integrated and working in the context of the main program**
- It's not enough to have code working in isolation; it needs to be **accessible and operational** in the application
- Verify complete flow: menu → action → result
- Manually test functionality in the running program

**Complete Integration Checklist**:

1. **Full GUI Flow Test**:
   ```bash
   # Start application
   python -m app --gui
   
   # Manually test:
   [ ] Menu item appears correctly?
   [ ] Clicking the menu opens the dock?
   [ ] Dock displays all controls?
   [ ] Basic functionality works (conversion, search, etc.)?
   [ ] Signals between components work (e.g., "Open in Editor")?
   [ ] Error messages appear when appropriate?
   [ ] i18n translation works (change language and verify)?
   ```

2. **Full CLI Flow Test**:
   ```bash
   # Test help
   python -m app convert --help
   
   # Test functionality
   python -m app convert test.txt --pretty -o output.data
   
   # Test pipes
   echo "name: John" | python -m app convert -
   
   # Verify:
   [ ] Help text appears?
   [ ] Arguments are recognized?
   [ ] Functionality executes without errors?
   [ ] Output is correct?
   [ ] Correct exit codes (0=success, 1=error)?
   ```

3. **Inter-Component Integration Test**:
   ```bash
   # Example: Convert text → Open in editor
   [ ] Clicking "Open in Editor" in the Text to DATA Converter opens the Editor?
   [ ] DATA is loaded correctly in the Editor?
   [ ] Editor can save the result?
   
   # Example: Search → Open file
   [ ] Clicking search result opens correct file?
   [ ] Cursor position goes to the correct line?
   ```

4. **Robustness Test**:
   ```bash
   # Error scenarios
   [ ] File not found displays clear message?
   [ ] Invalid input is handled gracefully?
   [ ] Canceled operation does not leave inconsistent state?
   [ ] Resources are correctly released (files closed, memory)?
   ```

5. **Performance Test** (if applicable):
   ```bash
   # Large files
   [ ] Processes files >10MB without freezing?
   [ ] Interface remains responsive during long operation?
   [ ] Progress bar/visual feedback works?
   [ ] Cancellation works during long operation?
   ```

**Real Example of Integration Problem**:
```python
# ❌ PROBLEM FOUND IN INTEGRATION:
# Task Example - Text to DATA Converter CLI
# Problem: Extractor() was being called without 3 mandatory parameters

# BEFORE (broke during integration):
def main():
    if args.command == 'convert':
        extractor = Extractor()  # ❌ TypeError: missing 3 required arguments

# AFTER (fixed):
def main():
    if args.command == 'convert':
        extractor = Extractor(
            avoid_keys="",
            avoid_keys_parameter="equals",
            with_quotation_marks=False
        )  # ✅ Works!
```

**Questions to Validate Integration**:
1. ❓ "Can the end-user easily access the functionality?"
2. ❓ "Do all usage flows work end-to-end?"
3. ❓ "Are there any errors or warnings in the console during normal use?"
4. ❓ "Is the functionality consistent with the rest of the application?"
5. ❓ "Is the documentation (help text, tooltips) clear and correct?"

**Why is this step critical?**:
- ✅ Detects problems that unit tests don't catch
- ✅ Validates real user experience
- ✅ Ensures all work is truly usable
- ✅ Avoids surprises after commit (tested code ≠ integrated code)

---

### 9️⃣.5️⃣ **Peer Code Review** (Optional - For Teams)

**When to Apply**:
- ✅ Team projects (2+ developers)
- ✅ Critical changes (security, data)
- ✅ Complex features (>200 lines)
- ✅ Code that others will maintain
- ✅ Open-source with contributors

**Do Not Apply If**:
- ❌ Solo/personal project
- ❌ Critical emergency hotfix
- ❌ Trivial changes (typos in docs)
- ❌ Disposable prototype

**Pull Request Process**:

```bash
# 1. Create feature branch
git checkout -b feature/task-42-add-export

# 2. Implement and commit
git add clarify_patched.py
git commit -m "Add CSV export feature (Task Example)"

# 3. Push and create PR
git push origin feature/task-42-add-export
# Open PR on GitHub/GitLab with template

# 4. Await review from at least 1 colleague
# 5. Implement requested changes
# 6. Merge after approval
```

**Pull Request Template**:

```markdown
## Description
Implements CSV export for Task Example of Simplicity Protocol.

## Type of Change
- [x] New feature
- [ ] Bug fix
- [ ] Refactoring
- [ ] Documentation

## Simplicity Protocol Checklist
- [x] Step 1: Task defined and selected (Task Example)
- [x] Step 2: Divided into subtasks
- [x] Step 6: Code implemented
- [x] Step 7: Manual code review (self-review)
- [x] Step 8: GUI manually tested
- [x] Step 9: Integration verified
- [x] Step 10: Unit tests (pytest)
- [x] Step 11: Code organized (PEP 8)

## How to Test
```bash
pytest tests/test_csv_export.py -v
python clarify_patched.py --export tasks.csv
```

## Screenshots (if applicable)
![CSV Export Dialog](screenshots/csv-export.png)

## Related
- Closes #42
- Related to #38 (Data Export Epic)
```

**Reviewer Checklist**:

```markdown
### Code Review Checklist - [PR Name]

#### 1. Functionality
- [ ] **Feature**: Does the implementation solve the described problem?
- [ ] **Edge Cases**: Are edge cases handled (empty input, None, etc.)?
- [ ] **Errors**: Do errors have clear messages?
- [ ] **UX**: Is the interface intuitive and consistent?

#### 2. Code
- [ ] **Readability**: Is the code clear and self-documented?
- [ ] **Simplicity**: Is the solution as simple as possible?
- [ ] **Duplication**: Is there no duplicate code?
- [ ] **Names**: Do variables/functions have descriptive names?
- [ ] **Comments**: Do comments explain "why," not "what"?

#### 3. Architecture
- [ ] **Separation**: Is logic separated from presentation?
- [ ] **Dependencies**: Are new dependencies justified?
- [ ] **Patterns**: Does it follow project patterns?
- [ ] **SOLID**: Are SOLID principles respected?

#### 4. Tests
- [ ] **Coverage**: Does new code have unit tests?
- [ ] **Cases**: Do tests cover critical scenarios?
- [ ] **Pass**: Do all tests pass in CI?
- [ ] **Readability**: Are tests clear and maintainable?

#### 5. Security
- [ ] **Input**: Does input validation exist?
- [ ] **SQL**: No SQL injection (use parameterized queries)?
- [ ] **Secrets**: No credentials in code?
- [ ] **Permissions**: Adequate permission checks?

#### 6. Performance
- [ ] **Loops**: Are loops efficient (no unnecessary O(n²))?
- [ ] **Queries**: Are DB queries optimized (indexes)?
- [ ] **Memory**: No memory leaks (close resources)?
- [ ] **Caching**: Is caching applied where it makes sense?

#### 7. Documentation
- [ ] **Docstrings**: Do public functions have docstrings?
- [ ] **README**: README updated if necessary?
- [ ] **CHANGELOG**: Is a changelog entry created?
- [ ] **Comments**: Are complex decisions documented?
```

**Example of Review Comment**:

```markdown
**❌ Problem - Missing input validation**

```python
# Line 142
def export_to_csv(self, filename):
    with open(filename, 'w') as f:
        # ...
```

**Suggestion**:
```python
def export_to_csv(self, filename):
    if not filename:
        raise ValueError("Filename cannot be empty")
    
    if not filename.endswith('.csv'):
        raise ValueError("Filename must end with .csv")
    
    try:
        with open(filename, 'w', encoding='utf-8') as f:
            # ...
    except IOError as e:
        raise IOError(f"Failed to write CSV: {e}")
```

**Rationale**: Without validation, the code can fail silently or generate invalid files.
```

**Tools for Code Review**:

```bash
# GitHub CLI - Create PR via terminal
gh pr create --title "Add CSV export" --body "Implements Task Example"

# Review PR locally
gh pr checkout 123
pytest
python clarify_patched.py --test

# Approve PR
gh pr review 123 --approve --body "LGTM! Clean and tested code."

# Request changes
gh pr review 123 --request-changes --body "Please add input validation (see comments)"
```

**GitLab - Merge Request Template**:

```yaml
# .gitlab/merge_request_templates/feature.md
## Feature Description
<!-- Describe what was implemented -->

## Simplicity Protocol Checklist
- [ ] Task defined (Step 1)
- [ ] Code implemented (Step 6)
- [ ] Tests passing (Step 10)
- [ ] Documentation updated (Step 12)

## How to Test
<!-- Commands to test the feature -->

## Screenshots
<!-- If applicable -->

/label ~feature
/assign @reviewer-name
```

**Code Review Culture**:

```markdown
### Principles for Constructive Reviews

1. **Be Kind**: "Consider adding validation" > "This is wrong"
2. **Explain Why**: Not just "Change this," but "Change this because..."
3. **Ask**: "What do you think about...?" > "You should..."
4. **Approve Quickly**: If it's good enough, approve (don't seek perfection)
5. **Learn**: See reviews as an opportunity to learn
6. **Automate**: Use linters for style, focus on logic

### Anti-Patterns to Avoid
- ❌ Excessive nitpicking (spaces, commas)
- ❌ Rewriting everything your way
- ❌ Leaving PR stalled for days
- ❌ Approving without reading (rubber stamping)
- ❌ Vague comments ("This is bad")
```

**Code Review Metrics**:

```python
# Example: tracking review metrics
review_metrics = {
    "pr_number": 123,
    "author": "alice",
    "reviewer": "bob",
    "lines_changed": 250,
    "files_changed": 3,
    "comments": 8,
    "time_to_first_review_hours": 4,
    "time_to_merge_hours": 18,
    "result": "approved"
}

# Healthy metrics:
# - Time to first review: < 8h
# - Time to merge: < 48h
# - Comments per PR: 3-10 (not too many, not too few)
# - Approval rate: > 80% (if < 50%, reviews are too strict)
```

**Why Code Review is valuable**:
- ✅ **Quality**: Detects bugs before production (15-20% on average)
- ✅ **Knowledge**: Distributes code knowledge within the team
- ✅ **Mentoring**: Junior developers learn from seniors
- ✅ **Consistency**: Maintains uniform project standards
- ✅ **Documentation**: PR discussions = historical context

---

### 10. **Run Tests**
- **Mandatory**: Unit tests for each public function
- **Goal**: 100% coverage of implemented functionalities
- **Tools**: `unittest` (native) or `pytest`
- **CRITICAL**: Test the system **after integration** (integrated GUI + CLI)
- **IMPORTANT**: Execute **AFTER** code review (Steps 7 and 8)

**Test Categories**:
1. **Happy Path**: Normal use cases
2. **Edge Cases**: Empty values, None, long strings
3. **Error Handling**: Expected exceptions
4. **Integration**: Complete flow (including GUI/CLI integration)
5. **Quality Validation**: Tests that validate the absence of the 9 problems from Steps 7 and 8

**Task Example**:
```python
✅ test_extract_from_dict_simple()
✅ test_extract_from_obj_type()
✅ test_simple_substitution_same_value()
✅ test_different_values_no_substitution()
✅ test_apply_substitutions_tsx_file()
✅ test_update_multiple_files()
# ... 12 tests in total (100% passing)
```

**Why test AFTER integration and review?**:
- Ensures tests validate the **integrated system**, not isolated components
- Detects integration problems during testing
- Validates that features actually work in the context of the application
- Avoids false positives (tests pass but feature is not accessible)
- Code has already been reviewed, so tests validate **quality code**

**Why?**: Ensure quality, prevent regressions, facilitate future maintenance.

---

#### 🛡️ **Step 9.1 - Security in Tests (CRITICAL)**

**Problem Identified** (Task Example - 01/12/2025):
- GUI tests hung in an **infinite loop** for >1 hour without timeout
- No automatic deadlock or hang detection
- Tests waited for a non-existent X11 display (headless environment)

**Mandatory Solutions**:

1. **⏱️ Mandatory Maximum Timeout** (30s per test):
   ```bash
   # ALWAYS use timeout in tests
   pytest tests/test_*.py --timeout=30 -v
   
   # Install pytest-timeout plugin if necessary
   pip install pytest-timeout
   ```

2. **🚨 Infinite Loop Detection** (warning in 10s):
   ```bash
   # More aggressive timeout to detect loops
   timeout 10s pytest tests/test_specific.py || echo "⚠️ TIMEOUT: Possible infinite loop detected!"
   ```

3. **🖥️ Mandatory Headless Environment** (GUI tests without display):
   ```bash
   # Use Qt offscreen platform
   QT_QPA_PLATFORM=offscreen pytest tests/test_gui_*.py -v --timeout=30
   
   # OR use pytest-xvfb for virtual X11 environment
   pip install pytest-xvfb
   pytest tests/test_gui_*.py --xvfb-backend xvfb --timeout=30
   ```

4. **✅ Mandatory Dry-Run** (before executing):
   ```bash
   # 1. Check syntax
   python -m py_compile tests/test_*.py && echo "✅ Valid syntax"
   
   # 2. Check imports
   python -c "from tests.test_module import *; print('✅ Imports OK')"
   
   # 3. List tests without executing
   pytest tests/test_*.py --collect-only
   ```

5. **⏲️ Time Monitoring** (record duration):
   ```bash
   # Measure total time and save log
   time pytest tests/test_*.py -v --timeout=30 | tee test_output.log
   
   # Use pytest-benchmark for metrics
   pytest tests/test_*.py --benchmark-only --timeout=30
   ```

**Why?**: Prevent infinite hangs, protect development time, ensure reliable tests.

---

### 10.5 **Profiling and Optimization** (Optional - For Critical Features)

**When to Apply**:
- ✅ Performance-critical features (loops, data processing)
- ✅ Operations that process large files (>10MB)
- ✅ Code that runs frequently (hot paths)
- ✅ Applications with latency requirements (<100ms)
- ✅ When users report slowness

**Do Not Apply If**:
- ❌ Feature runs rarely (initial setup)
- ❌ Performance is already good enough (<1s for user)
- ❌ Configuration/initialization code
- ❌ Prototypes or POCs

**Profiling with cProfile**:

```bash
# CPU Profiling - find slow functions
python -m cProfile -s cumulative clarify_patched.py > profile.txt

# Profiling with visualization
pip install snakeviz
python -m cProfile -o profile.stats clarify_patched.py
snakeviz profile.stats  # Opens browser with flamegraph
```

**Example Analysis**:

```python
# ❌ SLOW - O(n²) to process tasks
def find_duplicates_slow(tasks):
    """Finds duplicate tasks - SLOW VERSION."""
    duplicates = []
    for i, task1 in enumerate(tasks):
        for j, task2 in enumerate(tasks):
            if i != j and task1.title == task2.title:
                duplicates.append((task1, task2))
    return duplicates

# Profiling reveals: 85% of time in find_duplicates_slow()
# For 1000 tasks: 5.2 seconds

# ✅ FAST - O(n) using set
def find_duplicates_fast(tasks):
    """Finds duplicate tasks - OPTIMIZED VERSION."""
    seen = {}
    duplicates = []
    for task in tasks:
        if task.title in seen:
            duplicates.append((seen[task.title], task))
        else:
            seen[task.title] = task
    return duplicates

# After optimization: 0.02 seconds (260x faster)
```

**Memory Profiling**:

```bash
# Install memory_profiler
pip install memory_profiler

# Decorate function to profile
```

```python
from memory_profiler import profile

@profile
def load_large_file(filepath):
    """Load and process large DATA file."""
    with open(filepath, 'r') as f:
        data = data.load(f)  # Loads everything into memory
    
    # Process...
    results = []
    for item in data:
        results.append(process_item(item))
    
    return results

# Execute with profiling
# python -m memory_profiler clarify_patched.py
```

**Memory Optimization Example**:

```python
# ❌ MEMORY LEAK - Loads entire file (500MB)
def process_large_csv_bad(filepath):
    with open(filepath, 'r') as f:
        lines = f.readlines()  # 500MB in memory!
    
    results = []
    for line in lines:
        results.append(process_line(line))
    return results

# Memory profiler shows: Peak of 520MB

# ✅ OPTIMIZED - Streaming (constant 5MB)
def process_large_csv_good(filepath):
    results = []
    with open(filepath, 'r') as f:
        for line in f:  # Reads line by line
            results.append(process_line(line))
    return results

# Memory profiler shows: Peak of 8MB (65x less)
```

**Line-by-Line Profiling**:

```python
# Install line_profiler
# pip install line_profiler

# Decorate suspicious function
@profile  # Requires kernprof
def complex_calculation(data):
    """Function to profile line-by-line."""
    # Line 1: setup
    total = 0
    
    # Line 2: main loop
    for item in data:
        # Line 3: heavy calculation
        result = expensive_operation(item)
        total += result
    
    return total

# Execute
# kernprof -l -v clarify_patched.py
# Shows time per line of code
```

**Benchmarking Before/After**:

```python
import time

def benchmark(func, *args, iterations=100):
    """Benchmark function performance."""
    times = []
    for _ in range(iterations):
        start = time.perf_counter()
        func(*args)
        end = time.perf_counter()
        times.append(end - start)
    
    avg = sum(times) / len(times)
    return {
        "avg_ms": avg * 1000,
        "min_ms": min(times) * 1000,
        "max_ms": max(times) * 1000
    }

# Before optimization
before = benchmark(find_duplicates_slow, large_task_list)
print(f"BEFORE: {before['avg_ms']:.2f}ms")

# After optimization
after = benchmark(find_duplicates_fast, large_task_list)
print(f"AFTER: {after['avg_ms']:.2f}ms")
print(f"SPEEDUP: {before['avg_ms'] / after['avg_ms']:.1f}x")

# Output:
# BEFORE: 5240.32ms
# AFTER: 20.15ms
# SPEEDUP: 260.0x
```

**Optimization Checklist**:

```markdown
### Performance Checklist - [Feature Name]

#### Profiling Performed
- [ ] **CPU**: cProfile executed and analyzed
- [ ] **Memory**: memory_profiler executed (if > 100MB)
- [ ] **Hotspots**: Top 3 slowest functions identified
- [ ] **Baseline**: Time/memory before optimization documented

#### Optimizations Applied
- [ ] **Algorithm**: Complexity reduced (O(n²) → O(n log n) or O(n))
- [ ] **Structures**: Appropriate data structures (dict vs list)
- [ ] **I/O**: I/O optimized (buffering, streaming)
- [ ] **Cache**: Caching applied for repeated operations
- [ ] **Lazy**: Lazy loading for large data

#### Validation
- [ ] **Benchmark**: Before/after documented with speedup
- [ ] **Tests**: All tests still pass
- [ ] **Correctness**: Output identical to previous version
- [ ] **Limits**: Tested with realistic volume (10x typical data)

#### Documentation
- [ ] **Comments**: Non-obvious optimizations documented
- [ ] **Big-O**: Complexity documented in docstring
- [ ] **Trade-offs**: Trade-offs explained (memory vs speed)
```

**Advanced Tools**:

```bash
# py-spy - Sampling profiler (without modifying code)
pip install py-spy
py-spy record -o profile.svg -- python clarify_patched.py
# Generates interactive flamegraph

# Scalene - CPU + Memory + GPU profiler
pip install scalene
scalene clarify_patched.py
# Interactive dashboard in terminal

# pytest-benchmark for tests
pip install pytest-benchmark

# Example benchmark test
def test_find_duplicates_performance(benchmark):
    tasks = generate_large_task_list(1000)
    result = benchmark(find_duplicates_fast, tasks)
    assert len(result) > 0
    # benchmark automatically measures time
```

**When to Stop Optimizing**:

```python
# Pareto Rule: 80% of gains come from 20% of effort

# ✅ WORTH OPTIMIZING:
# - Reduction from 5s → 0.5s (10x) = 4.5s saved per execution
# - If executed 100x/day = 450s (7.5min) saved/day

# ❌ NOT WORTH OPTIMIZING:
# - Reduction from 0.05s → 0.02s (2.5x) = 0.03s saved
# - If executed 10x/day = 0.3s saved/day (insignificant)

# Criterion: Optimize if time saved × frequency > 1 minute/day
```

**Why Profiling is important**:
- ✅ **Evidence**: Optimize based on data, not "gut feeling"
- ✅ **Focus**: Identify real bottlenecks (not where we think they are)
- ✅ **ROI**: Prioritize optimizations with the greatest impact
- ✅ **Avoid**: Premature micro-optimizations that complicate code
- ✅ **Scalability**: Ensure code scales with larger data

---

### 10.6 **CI/CD Quality Gates** ⭐ (Optional - HIGH PRIORITY)

**When to Apply**:
- ✅ Team projects (2+ people)
- ✅ Production or critical code
- ✅ Open-source with contributors
- ✅ When consistent quality needs to be ensured
- ✅ Environments with multiple branches

**Do Not Apply If**:
- ❌ Solo/experimental project
- ❌ Disposable prototype
- ❌ Single-use scripts
- ❌ No CI infrastructure (GitHub/GitLab/Jenkins)

**Pre-commit Hooks - Local Validation**:

```yaml
# .pre-commit-config.yaml
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v4.5.0
    hooks:
      - id: trailing-whitespace
      - id: end-of-file-fixer
      - id: check-yaml
      - id: check-data
      - id: check-added-large-files
        args: ['--maxkb=500']
  
  - repo: https://github.com/psf/black
    rev: 23.12.1
    hooks:
      - id: black
        language_version: python3.11
  
  - repo: https://github.com/pycqa/flake8
    rev: 7.0.0
    hooks:
      - id: flake8
        args: ['--max-line-length=88', '--extend-ignore=E203']
  
  - repo: https://github.com/PyCQA/bandit
    rev: 1.7.6
    hooks:
      - id: bandit
        args: ['-ll', '-i']  # Low severity, ignore issues
  
  - repo: local
    hooks:
      - id: pytest
        name: pytest
        entry: pytest
        language: system
        pass_filenames: false
        args: ['tests/', '-v', '--tb=short']
```

```bash
# Install pre-commit
pip install pre-commit

# Activate hooks
pre-commit install

# Now every git commit executes validations automatically
# If it fails, commit is blocked until corrected
```

**GitHub Actions - CI Pipeline**:

```yaml
# .github/workflows/ci.yml
name: CI Quality Gates

on:
  push:
    branches: [ main, develop ]
  pull_request:
    branches: [ main ]

jobs:
  quality-checks:
    runs-on: ubuntu-latest
    strategy:
      matrix:
        python-version: ["3.10", "3.11", "3.12"]
    
    steps:
    - uses: actions/checkout@v4
    
    - name: Set up Python ${{ matrix.python-version }}
      uses: actions/setup-python@v5
      with:
        python-version: ${{ matrix.python-version }}
    
    - name: Install dependencies
      run: |
        python -m pip install --upgrade pip
        pip install -r requirements.txt
        pip install pytest pytest-cov flake8 black bandit mypy
    
    - name: Code Formatting (Black)
      run: |
        black --check clarify_patched.py
      continue-on-error: false
    
    - name: Linting (Flake8)
      run: |
        flake8 clarify_patched.py --max-line-length=88 --statistics
      continue-on-error: false
    
    - name: Type Checking (MyPy)
      run: |
        mypy clarify_patched.py --ignore-missing-imports
      continue-on-error: true  # Warnings, not errors
    
    - name: Security Scan (Bandit)
      run: |
        bandit -r clarify_patched.py -ll
      continue-on-error: false
    
    - name: Unit Tests with Coverage
      run: |
        pytest tests/ --cov=. --cov-report=xml --cov-report=term
      continue-on-error: false
    
    - name: Upload Coverage to Codecov
      uses: codecov/codecov-action@v3
      with:
        file: ./coverage.xml
        fail_ci_if_error: true
    
    - name: Coverage Threshold Check
      run: |
        coverage report --fail-under=80
      # Fails if coverage < 80%
```

**GitLab CI - Pipeline with Quality Gates**:

```yaml
# .gitlab-ci.yml
stages:
  - lint
  - test
  - security
  - deploy

variables:
  PIP_CACHE_DIR: "$CI_PROJECT_DIR/.cache/pip"

cache:
  paths:
    - .cache/pip

lint:black:
  stage: lint
  image: python:3.11
  script:
    - pip install black
    - black --check clarify_patched.py
  allow_failure: false

lint:flake8:
  stage: lint
  image: python:3.11
  script:
    - pip install flake8
    - flake8 clarify_patched.py --max-line-length=88 --statistics
  allow_failure: false

test:pytest:
  stage: test
  image: python:3.11
  script:
    - pip install -r requirements.txt
    - pip install pytest pytest-cov
    - pytest tests/ --cov=. --cov-report=term --cov-report=html
    - coverage report --fail-under=80
  coverage: '/TOTAL.*\s+(\d+%)$/'
  artifacts:
    reports:
      coverage_report:
        coverage_format: cobertura
        path: coverage.xml
    paths:
      - htmlcov/
  allow_failure: false

security:bandit:
  stage: security
  image: python:3.11
  script:
    - pip install bandit
    - bandit -r clarify_patched.py -f data -o bandit-report.data
  artifacts:
    reports:
      sast: bandit-report.data
  allow_failure: false

deploy:production:
  stage: deploy
  script:
    - echo "Deploying to production..."
    - # Deployment commands
  only:
    - main
  when: manual  # Manual deploy after quality gates pass
```

**Quality Metrics - Dashboards**:

```python
# Script to generate quality report
import subprocess
import data

def run_quality_checks():
    """Executes quality gates and generates report."""
    
    results = {
        "timestamp": datetime.now().isoformat(),
        "checks": {}
    }
    
    # 1. Code Coverage
    cov = subprocess.run(
        ["pytest", "--cov=.", "--cov-report=data"],
        capture_output=True
    )
    with open("coverage.data") as f:
        results["checks"]["coverage"] = data.load(f)["totals"]["percent_covered"]
    
    # 2. Linting Score
    flake8 = subprocess.run(
        ["flake8", "clarify_patched.py", "--statistics"],
        capture_output=True,
        text=True
    )
    results["checks"]["linting_errors"] = len(flake8.stdout.splitlines())
    
    # 3. Security Issues
    bandit = subprocess.run(
        ["bandit", "-r", ".", "-f", "data"],
        capture_output=True
    )
    bandit_data = data.loads(bandit.stdout)
    results["checks"]["security_issues"] = len(bandit_data["results"])
    
    # 4. Type Coverage (MyPy)
    mypy = subprocess.run(
        ["mypy", "clarify_patched.py", "--data-report", ".mypy"],
        capture_output=True
    )
    # Parse MyPy report...
    
    # Quality Score (0-100)
    score = (
        results["checks"]["coverage"] * 0.4 +
        (100 - min(results["checks"]["linting_errors"], 100)) * 0.3 +
        (100 - min(results["checks"]["security_issues"] * 10, 100)) * 0.3
    )
    results["quality_score"] = round(score, 2)
    
    # Pass/Fail Gates
    results["gates"] = {
        "coverage": results["checks"]["coverage"] >= 80,
        "linting": results["checks"]["linting_errors"] == 0,
        "security": results["checks"]["security_issues"] == 0
    }
    results["passed"] = all(results["gates"].values())
    
    return results

# Integrate with CI
if __name__ == "__main__":
    results = run_quality_checks()
    print(data.dumps(results, indent=2))
    
    if not results["passed"]:
        print("\n❌ Quality gates FAILED!")
        exit(1)
    else:
        print("\n✅ All quality gates PASSED!")
```

**Status Badge in README**:

```markdown
# Clarify - Task Management

[![CI Status](https://github.com/user/clarify/workflows/CI/badge.svg)](https://github.com/user/clarify/actions)
[![Coverage](https://codecov.io/gh/user/clarify/branch/main/graph/badge.svg)](https://codecov.io/gh/user/clarify)
[![Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=clarify&metric=alert_status)](https://sonarcloud.io/dashboard?id=clarify)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

Badges visually show quality status
```

**Why CI/CD is crucial**:
- ✅ **Automation**: Validates quality without manual intervention
- ✅ **Consistency**: Same rules for all developers
- ✅ **Prevention**: Detects problems before merge/deploy
- ✅ **Confidence**: Team knows that broken code won't go to production
- ✅ **Speed**: Fast feedback (minutes, not hours)

---

### 11. **Organize Project Root Folder**
- ✅ Imports validated (module loads without errors)
- 📝 **Documented limitation**: GUI tests require an unconfigured headless environment

---

#### 🔬 **Step 9.2 - Tests in Threads/Processes with Monitoring (ADVANCED)**

**Objective**: Full control over test execution with the possibility to **interrupt**, **monitor**, and **log** progress in real-time.

**When to Use**:
- GUI tests that might hang
- Long-running tests (>1 min)
- Tests with external dependencies (network, database)
- Need for real-time logging
- Need for manual cancellation during execution

**Implementation with `multiprocessing.Process`**:

```python
# tests/test_runner_monitored.py
import multiprocessing as mp
import time
import sys
from queue import Empty

def run_tests_in_process(test_module: str, queue: mp.Queue, timeout: int = 30):
    """
    Executes tests in a separate process with logging to a queue.
    
    Args:
        test_module: Test module (e.g., 'tests.test_file_list_dock')
        queue: Queue for progress communication
        timeout: Timeout in seconds
    """
    try:
        import pytest
        
        # Configure real-time logging
        class QueueReporter:
            def __init__(self, queue):
                self.queue = queue
            
            def pytest_runtest_logreport(self, report):
                """pytest hook to capture results."""
                if report.when == 'call':
                    status = '✅ PASS' if report.passed else '❌ FAIL'
                    self.queue.put({
                        'type': 'test_result',
                        'test': report.nodeid,
                        'status': status,
                        'duration': report.duration
                    })
        
        # Execute pytest with custom reporter
        queue.put({'type': 'info', 'msg': f'Starting tests: {test_module}'})
        
        result = pytest.main([
            test_module,
            '-v',
            f'--timeout={timeout}',
            '--tb=short',
            '-p', 'no:cacheprovider'  # Disable cache
        ])
        
        queue.put({'type': 'info', 'msg': f'Tests finished. Exit code: {result}'})
        queue.put({'type': 'exit', 'code': result})
        
    except Exception as e:
        queue.put({'type': 'error', 'msg': str(e)})
        queue.put({'type': 'exit', 'code': 1})

def monitor_test_execution(test_module: str, max_timeout: int = 300):
    """
    Monitors test execution with full control.
    
    Args:
        test_module: Test module
        max_timeout: Maximum timeout in seconds (default: 5 min)
    
    Returns:
        dict: Execution result with statistics
    """
    queue = mp.Queue()
    process = mp.Process(
        target=run_tests_in_process,
        args=(test_module, queue, 30)
    )
    
    print(f"🚀 Starting tests: {test_module}")
    print(f"⏱️  Maximum timeout: {max_timeout}s")
    print(f"📊 Monitoring active. Press Ctrl+C to cancel.\n")
    
    process.start()
    start_time = time.time()
    results = {'passed': 0, 'failed': 0, 'tests': []}
    
    try:
        while process.is_alive():
            elapsed = time.time() - start_time
            
            # Check global timeout
            if elapsed > max_timeout:
                print(f"\n⚠️  GLOBAL TIMEOUT ({max_timeout}s exceeded)")
                process.terminate()
                process.join(timeout=5)
                if process.is_alive():
                    process.kill()
                return {'status': 'timeout', 'elapsed': elapsed, 'results': results}
            
            # Read messages from the queue (non-blocking)
            try:
                msg = queue.get(timeout=0.5)
                
                if msg['type'] == 'test_result':
                    print(f"  {msg['status']} {msg['test']} ({msg['duration']:.2f}s)")
                    results['tests'].append(msg)
                    if '✅' in msg['status']:
                        results['passed'] += 1
                    else:
                        results['failed'] += 1
                
                elif msg['type'] == 'info':
                    print(f"ℹ️  {msg['msg']}")
                
                elif msg['type'] == 'error':
                    print(f"❌ ERROR: {msg['msg']}")
                
                elif msg['type'] == 'exit':
                    process.join(timeout=2)
                    elapsed = time.time() - start_time
                    print(f"\n✅ Tests finished in {elapsed:.2f}s")
                    return {
                        'status': 'completed',
                        'exit_code': msg['code'],
                        'elapsed': elapsed,
                        'results': results
                    }
            
            except Empty:
                # No message, continue monitoring
                pass
            
            # Show progress every 10s
            if int(elapsed) % 10 == 0 and int(elapsed) > 0:
                print(f"⏳ Executing... {int(elapsed)}s ({results['passed']} passed, {results['failed']} failed)")
    
    except KeyboardInterrupt:
        print("\n⚠️  Manual cancellation (Ctrl+C)")
        process.terminate()
        process.join(timeout=5)
        if process.is_alive():
            process.kill()
        elapsed = time.time() - start_time
        return {'status': 'cancelled', 'elapsed': elapsed, 'results': results}
    
    finally:
        if process.is_alive():
            process.terminate()
            process.join(timeout=5)

# Example usage:
if __name__ == '__main__':
    result = monitor_test_execution('tests/test_advanced_file_search.py', max_timeout=300)
    
    print(f"\n{'='*60}")
    print(f"Status: {result['status']}")
    print(f"Time: {result['elapsed']:.2f}s")
    print(f"Passed: {result['results']['passed']}")
    print(f"Failed: {result['results']['failed']}")
    print(f"{'='*60}")
```

**Practical Usage**:

```bash
# 1. Create monitored runner
cat > tests/run_tests_monitored.py << 'EOF'
# [code above]
EOF

# 2. Execute with monitoring
python tests/run_tests_monitored.py

# 3. Cancel at any time (Ctrl+C)
# The process will be terminated gracefully
```

**Advantages**:
- ✅ **Full control**: Can cancel tests at any time
- ✅ **Real-time logging**: See progress of each test
- ✅ **Global + individual timeout**: Double protection
- ✅ **Statistics**: Pass/fail in real-time
- ✅ **Isolation**: Tests run in a separate process (don't block the terminal)
- ✅ **Guaranteed cleanup**: `terminate()` + `kill()` forced if necessary

**Optional Configurations**:

1. **File Logging** (in addition to stdout):
   ```python
   # Add to run_tests_in_process:
   import logging
   logging.basicConfig(
       filename=f'test_{time.time()}.log',
       level=logging.INFO,
       format='%(asctime)s - %(message)s'
   )
   ```

2. **Sound Notification** (upon completion):
   ```python
   import os
   # At the end of monitor_test_execution:
   os.system('paplay /usr/share/sounds/freedesktop/stereo/complete.oga')
   ```

3. **CI/CD Integration**:
   ```python
   # Return correct exit code:
   sys.exit(0 if result['status'] == 'completed' and result['results']['failed'] == 0 else 1)
   ```

**Additional Checklist (Step 9.2 - Optional)**:
```
[ ] Create test_runner_monitored.py with multiprocessing
[ ] Define global timeout (default: 5 min)
[ ] Define individual timeout per test (default: 30s)
[ ] Implement real-time logging (Queue)
[ ] Test manual cancellation (Ctrl+C)
[ ] Verify process cleanup (ps aux | grep pytest)
```

**When NOT to use**:
- Simple and fast tests (<10s total)
- Tests without GUI (pure backend)
- CI/CD with native timeout configured
- First execution of tests (unnecessary overhead)

---

### 11. **Organize Project Root Folder**
- **CRITICAL**: Before documentation, **organize the root folder**
- Remove temporary files, unnecessary backups
- Verify all files are in the correct places
- Clear cache and generated files (`__pycache__`, `.pyc`)
- Ensure `.gitignore` is updated

**Organization Checklist**:
1. **Removal of Temporary Files**:
   ```bash
   # Remove old backups
   rm -f *.backup_* *.bak *~
   
   # Clear Python cache
   find . -type d -name "__pycache__" -exec rm -rf {} +
   find . -type f -name "*.pyc" -delete
   find . -type f -name "*.pyo" -delete
   ```

2. **Directory Structure Verification**:
   - `src/` - source code
   - `tests/` - unit tests
   - `docs/` - documentation
   - Organized root files (README, setup.py, etc.)

**Example**:
```bash
# BEFORE (messy folder):
├── src/
├── apply_v2913_patches.py  ❌ temporary
├── test_temp.py           ❌ disposable test
├── backup_old/            ❌ old backup
├── __pycache__/           ❌ cache
└── file.py.backup_v2913   ❌ unnecessary backup

# AFTER (organized):
├── src/          ✅
├── tests/        ✅
├── docs/         ✅
└── README.md     ✅
```

**Why?**: Keep repository clean, avoid committing garbage, facilitate navigation, professionalism. Document the **clean** state of the project.

---

### 11.5 **Architecture Decision Records (ADR)** (Optional)

**When to Apply**:
- ✅ Important architectural decisions (framework, library, pattern)
- ✅ Significant trade-offs were made
- ✅ Long-term projects (> 6 months)
- ✅ Teams with turnover (onboarding)
- ✅ When "why did we do it this way?" will be asked

**Do Not Apply If**:
- ❌ Trivial decisions (naming, formatting)
- ❌ Short-term solo project
- ❌ Disposable prototype
- ❌ Obvious/conventional decisions

**What is ADR?**

ADR (Architecture Decision Record) documents **why** important decisions were made, not just **what** was decided. Useful for:
- Justifying choices for future developers
- Avoiding reopening already resolved discussions
- Learning from past decisions (good and bad)

**ADR Template**:

```markdown
# ADR-001: Choice of PyQt6 for GUI

## Status
✅ **ACCEPTED** - 2024-01-15

## Context
The project needs a graphical user interface (GUI) to manage tasks in addition to the existing CLI.

**Requirements**:
- Cross-platform (Linux, Windows, macOS)
- Integration with existing Python code
- Ability to create complex layouts (docks, tabs, menus)
- Licensing compatible with GPL
- Active community and documentation

**Alternatives Considered**:
1. **Tkinter** (native Python)
2. **PyQt6** (Qt bindings)
3. **wxPython** (wxWidgets bindings)
4. **Kivy** (mobile-first)

## Decision
We chose **PyQt6** for the GUI implementation.

## Consequences

### Positive ✅
- **Advanced Layout**: QDockWidget, QMainWindow allow professional layout
- **Rich Widgets**: QTreeWidget, QTableWidget already implemented and robust
- **Styling**: QSS (CSS-like) allows visual customization
- **Documentation**: Excellent official documentation + large community
- **Performance**: Native C++, faster than Tkinter
- **Cross-platform**: Works well on Linux, Windows, macOS

### Negative ❌
- **License**: GPL or commercial (~$450/dev) - we chose GPL
- **Size**: Larger binary (~50MB) vs Tkinter (~5MB)
- **Learning Curve**: More complex than Tkinter
- **External Dependency**: Requires `pip install PyQt6`

### Risks 🚨
- **GPL License**: Project must be open-source (OK for us)
- **Breaking Changes**: Qt6 is recent, there may be changes
- **Packaging**: PyInstaller needs special configuration for PyQt6

### Discarded Alternatives
- **Tkinter**: Primitive layout, no native dock widgets
- **wxPython**: Inferior documentation, smaller community
- **Kivy**: Mobile-focused, non-native desktop style

## Implementation
- Refactor existing code to separate presentation logic
- Create `ClarifyGUI` class with QMainWindow
- Maintain CLI compatibility for existing users
- Document PyQt6 installation in README

## References
- [PyQt6 Documentation](https://www.riverbankcomputing.com/static/Docs/PyQt6/)
- [Qt6 Documentation](https://doc.qt.io/qt-6/)
- Task Example: "Add GUI with docking support"

## Notes
If in the future we need a more permissive license (MIT/Apache), consider:
- Migrating to PySide6 (Qt LGPL binding)
- Rewriting with Tkinter + ttkbootstrap
- Using Dear PyGui (MIT, but OpenGL, not native)

---
**Author**: Josué
**Date**: 2024-01-15
**Last Update**: 2024-01-15
```

**Directory Structure for ADRs**:

```
clarify/
├── docs/
│   ├── adr/
│   │   ├── 001-choice-of-pyqt6.md
│   │   ├── 002-data-storage-format.md
│   │   ├── 003-simplicity-protocol-versioning.md
│   │   └── README.md  (ADR Index)
│   ├── PROTOCOLO_SIMPLICIDADE_1.md
│   └── PROTOCOLO_SIMPLICIDADE_2.md
├── clarify_patched.py
└── README.md
```

**ADR Index** (`docs/adr/README.md`):

```markdown
# Architecture Decision Records

## Active Decisions
- [ADR-001](001-choice-of-pyqt6.md): Choice of PyQt6 for GUI ✅ ACCEPTED
- [ADR-003](003-simplicity-protocol-versioning.md): Simplicity Protocol Versioning ✅ ACCEPTED

## Superseded Decisions
- [ADR-002](002-data-storage-format.md): DATA as storage format ⚠️ SUPERSEDED
  - Superseded by SQLite in ADR-004 (2024-02-01)

## Rejected Decisions
- (none)

## Proposed (Pending Discussion)
- ADR-005: Implement plugin support
- ADR-006: Migrate from DATA to SQLite

---

## Template
New ADRs should follow the template in `adr-template.md`

## Numbering
ADRs are numbered sequentially: 001, 002, 003, etc.
```

**Example of Superseded ADR**:

```markdown
# ADR-002: DATA as Storage Format

## Status
⚠️ **SUPERSEDED** by [ADR-004](004-migrate-to-sqlite.md) on 2024-02-01

## Context
(original context...)

## Decision
Use DATA for task persistence.

## Consequences

### Why was it superseded?
DATA worked well for up to ~500 tasks, but performance degraded significantly:
- Read time: 2.5s for 1000 tasks (unacceptable)
- Concurrency: Does not support multiple simultaneous windows
- Queries: Difficult to filter/search without loading everything

**Solution**: Migrate to SQLite (ADR-004) while keeping DATA as an optional export.

---
**Author**: Josué
**Original Date**: 2023-11-10
**Superseded**: 2024-02-01
```

**Tools for ADRs**:

```bash
# adr-tools - CLI to create ADRs
npm install -g adr-log

# Create new ADR
adr new "Implement caching layer"

# List all ADRs
adr list

# Supersede old ADR
adr new -s 2 "Migrate from DATA to SQLite"
# Creates new ADR and marks #2 as superseded

# Generate visualization
adr generate graph > adr-graph.svg
```

**When to Create ADR**:

```python
# ✅ DESERVES ADR - Impactful decision
"""
We decided to use SQLite instead of DATA.
Impact:
- Changes data persistence (migration needed)
- Affects performance (10x faster)
- Adds dependency (sqlite3 - native)
- Data access code needs refactoring
"""

# ❌ DOES NOT DESERVE ADR - Trivial decision
"""
We decided to rename variable 'x' to 'task_count'.
Impact: Code clarity only.
"""

# ✅ DESERVES ADR - Significant trade-off
"""
We decided NOT to implement task encryption.
Rationale:
- High complexity (key management)
- Low benefit (tasks are not sensitive)
- Can be added later if needed
"""
```

**ADR Checklist**:

```markdown
### ADR Checklist - ADR-XXX: [Title]

#### Complete Content
- [ ] **Status**: Proposed/Accepted/Rejected/Superseded defined
- [ ] **Context**: Problem clearly described
- [ ] **Alternatives**: At least 2 alternatives considered
- [ ] **Decision**: Choice explicitly stated
- [ ] **Consequences**: Positive AND negative documented
- [ ] **Risks**: Risks identified and proposed mitigations

#### Quality
- [ ] **Justification**: "Why" is clear (not just "what")
- [ ] **Trade-offs**: Trade-offs explicitly stated
- [ ] **Reversibility**: Cost of reversing documented
- [ ] **References**: Links to relevant docs/issues/PRs

#### Process
- [ ] **Numbering**: ADR numbered sequentially
- [ ] **Index**: README.md updated with new ADR
- [ ] **Review**: ADR reviewed by at least 1 person
- [ ] **Commit**: Committed along with related code
```

**ADR in Pull Request**:

```markdown
## PR #145: Implement SQLite storage

### Description
Migrates persistence from DATA to SQLite storage (Task Example).

### Architecture Decision
This PR implements **ADR-004: Migrate to SQLite**.

**Trade-offs**:
- ✅ 10x faster (2.5s → 0.2s for 1000 tasks)
- ✅ Supports concurrency (multiple windows)
- ❌ Migration required for existing users
- ❌ More complex persistence code

**Mitigated Risks**:
- Automatic migration on first use (v2.0.0)
- Automatic DATA backup before migration
- Rollback available if migration fails

### See ADR
- [ADR-004: Migrate to SQLite](docs/adr/004-migrate-to-sqlite.md)
- Supersedes ADR-002 (DATA storage)

### Checklist
- [x] ADR created and committed
- [x] Migration code implemented
- [x] Migration tests added
- [x] Documentation updated
```

**Why ADRs are valuable**:
- ✅ **Context**: Future devs understand "why" decisions were made
- ✅ **Avoids Rework**: Don't reopen already resolved discussions
- ✅ **Onboarding**: New members learn architecture quickly
- ✅ **Learning**: Team learns from past decisions (good and bad)
- ✅ **Auditing**: Stakeholders see transparent decision process

---

### 12. **Fill in New Documentation**
- **Update tasks/requirements file**: Mark tasks as `[X]` complete
- **Create SPECIFICATIONS.md**: Detailed version document
- **Update statistics**: Project completion percentage
- **🤖 [OPTIONAL] Manage AI task recommendations**

**📋 TASKS.md Management**:

**General Rule**:
- If a tasks/requirements file exists (e.g., `TASKS.md`, `TODO.md`, `requirements.md`):
  - ✅ **Mark tasks as complete** after implementation: `[ ]` → `[X]`
  - ✅ **Update statistics** (percentages, counters)
  - ✅ **Add completion notes** (date, version, brief description)
  - 🤖 **[OPTIONAL] Add new AI-recommended tasks** (see details in SIMPLICITY_PROTOCOL_1.md - Step 12)
  
- If a tasks/requirements file **DOES NOT exist**:
  - ❓ **Ask the user** for the file location/path
  - ❓ **Ask about next tasks and requirements** if no formal document
  - ❓ **Suggest creating** `TASKS.md` as the default file

**🤖 AI Task Recommendations**:
For enterprise teams (Simplicity 2), AI recommendations should be **reviewed in sprint retrospectives** (Step 13.5) before being added to TASKS.md. This ensures team consensus and alignment with stakeholders.

📘 **Complete details of recommendation functionality**: See `SIMPLICITY_PROTOCOL_1.md` - Step 12 - Section "AI Task Recommendations"

**Example of Marking (REQUIREMENTS.md)**:
```markdown
## 🟢 COULD HAVE (Low Priority)

### ✅ Completed Tasks

#### Task Example - Integrated File Editor (vX.Y.Z)
**Status**: ✅ Complete - 30/11/2025

**Objective**: Implement an integrated text editor with scope differentiation by colors.

**Implementation**:
1. ✅ ComponentE with QTextEdit and syntax highlighting
2. ✅ Scope differentiation by colors (HTML tags, DATA keys, etc.)
3. ✅ Open/save files (.txt, .data, .html, .tsx, .py)
4. ✅ Integration with File menu → Open Editor

**Files Created**:
- `src/gui/editor_dock.py` (500+ lines)
- `tests/test_editor_dock.py` (15 tests)

### 🔨 Pending Tasks
- **[]** Next unimplement task...
```

**Minimum Recommended Structure**:
```markdown
# Project - Tasks

## Categories
- MUST HAVE: [X/Y complete] (Z%)
- SHOULD HAVE: [X/Y complete] (Z%)
- COULD HAVE: [X/Y complete] (Z%)
- WOULD HAVE: [X/Y complete] (Z%)

## Statistics
- **TOTAL**: [X/Y complete] (Z%)
```

**Version Documentation Structure**:
```markdown
# Clarify v2.9.X - [Descriptive Name]

**Date**: DD/MM/AAAA
**Sprint**: X tasks in Y hours
**Methodology**: Simplicity Protocol 1

## 📋 Sprint Objectives
- Task #X: [description]
- Task #Y: [description]

## 🎯 Implemented Tasks
### Task #X: [Name]
- **Problem**: [description of original problem]
- **Solution**: [how it was solved]
- **Modified Files**: [list]
- **Tests**: [quantity and status]

## ✅ Quality (Simplicity Protocol 1)
- ✅ Modular Architecture
- ✅ Type Hints (100%)
- ✅ Complete Docstrings
- ✅ Error Handling
- ✅ Tests (X passing)
- ✅ Semantic Commits
- ✅ Complete Documentation
- ✅ Clean Code (PEP8)

## 📊 Statistics
- TOTAL: X% complete (Y/Z tasks)
- Commits: N pushed
```

---

### 12.5 **Rollback Plans** (Optional - For Critical Features)

**When to Apply**:
- ✅ Critical features in production
- ✅ Data schema changes/migrations
- ✅ Changes to public APIs
- ✅ Deploying high-risk features
- ✅ When downtime is unacceptable

**Do Not Apply If**:
- ❌ Experimental/beta feature (flag controlled)
- ❌ Internal change with no user impact
- ❌ Prototype or dev/staging environment only
- ❌ Trivial hotfix (typo, css)

**What is a Rollback Plan?**

A documented plan to **revert** a change if something goes wrong in production. Unlike "undoing a commit," rollback considers:
- Data state (migrations, schemas)
- External dependencies (APIs, services)
- Active users (downtime, data in transit)

**Rollback Plan Template**:

```markdown
# Rollback Plan - Task Example: SQLite Migration

## Change Summary
**Feature**: Migration from DATA to SQLite storage
**Version**: v2.0.0 → v1.9.x
**Impact**: HIGH - Alters persistence format
**Risk**: MEDIUM - Data migration may fail

## Criteria for Rollback
Execute rollback IF:
- [ ] Error rate > 5% within 1 hour after deploy
- [ ] Users report data loss (tasks disappearing)
- [ ] Performance worse than previous version (> 2x slower)
- [ ] Frequent crashes (> 10 reports in 24h)
- [ ] Automatic migration fails for > 10% users

DO NOT execute rollback IF:
- ✅ Only 1-2 users report problems (investigate first)
- ✅ Minor bug that can be hotfixed quickly
- ✅ Acceptable performance (< 1s), even if not ideal

## Step-by-Step Rollback

### Phase 1: Preparation (5 minutes)
1. **Notify users**:
   ```bash
   # Create maintenance banner
   echo "⚠️ Maintenance in progress - Rolling back to v1.9.5" > maintenance.txt
   ```

2. **Backup current state**:
   ```bash
   # Backup current SQLite database
   cp ~/.config/clarify/clarify.db ~/.config/clarify/clarify.db.backup-$(date +%s)
   
   # Backup logs
   cp ~/.config/clarify/clarify.log /tmp/clarify-rollback-logs.txt
   ```

3. **Verify DATA backup available**:
   ```bash
   # Confirm DATA backup exists (created during migration)
   ls -lh ~/.config/clarify/tasks.data.backup
   # Should show file created during migration to v2.0.0
   ```

### Phase 2: Rollback (10 minutes)
1. **Revert code to previous version**:
   ```bash
   cd ~/clarify
   git checkout v1.9.5  # Tag of previous stable version
   
   # OR if in production via package manager
   pip install clarify==1.9.5 --force-reinstall
   ```

2. **Restore data from DATA backup**:
   ```bash
   # Copy DATA backup back
   cp ~/.config/clarify/tasks.data.backup ~/.config/clarify/tasks.data
   
   # Remove SQLite database (v1.9.5 does not use)
   rm ~/.config/clarify/clarify.db
   ```

3. **Verify data integrity**:
   ```bash
   # Validate DATA is not corrupted
   python -c "import data; data.load(open('~/.config/clarify/tasks.data'))"
   # Should complete without error
   
   # Count tasks
   python -c "import data; data = data.load(open('~/.config/clarify/tasks.data')); print(f'{len(data[\"tasks\"])} tasks restored')"
   ```

4. **Restart application**:
   ```bash
   # If process running, kill
   pkill -f clarify
   
   # Start v1.9.5
   python clarify.py
   ```

### Phase 3: Validation (5 minutes)
1. **Smoke Tests**:
   ```bash
   # Test 1: App starts without crash
   clarify --version
   # Expected: v1.9.5
   
   # Test 2: List tasks
   clarify list
   # Expected: Tasks displayed correctly
   
   # Test 3: Add task
   clarify add "Test rollback task"
   # Expected: Task added without error
   
   # Test 4: GUI opens (if applicable)
   clarify --gui &
   # Expected: GUI opens without crash
   ```

2. **Check logs**:
   ```bash
   tail -n 50 ~/.config/clarify/clarify.log
   # Verify absence of SQLite errors
   ```

3. **Contact affected users**:
   - Ask 3-5 users to test basic functionality
   - Confirm their data is intact

### Phase 4: Communication (Immediate)
1. **Notify stakeholders**:
   ```markdown
   ## Rollback Executed - v2.0.0 → v1.9.5
   
   **Timestamp**: 2024-01-20 15:30 UTC
   **Reason**: Error rate 12% in SQLite migration (criterion: >5%)
   **Status**: ✅ Rollback complete, system stable
   **Impact**: v2.0.0 users must reinstall v1.9.5
   
   **User Action**:
   ```bash
   pip install clarify==1.9.5 --force-reinstall
   ```
   
   Data preserved via automatic DATA backup.
   
   **Next Steps**:
   - Root cause analysis of migration failure
   - Fix planned for v2.0.1 (ETA: 2024-01-25)
   - Expanded beta testing before release
   ```

2. **Create post-mortem issue**:
   ```markdown
   # Post-Mortem: Rollback v2.0.0 → v1.9.5
   
   ## Timeline
   - 14:00 UTC: Deploy v2.0.0
   - 14:30 UTC: First reports of migration failure
   - 15:00 UTC: Error rate reaches 12% (rollback criterion: >5%)
   - 15:15 UTC: Rollback decision made
   - 15:30 UTC: Rollback complete
   
   ## Root Cause
   - SQLite migration failed for DATA files > 5MB
   - Cause: 30s timeout insufficient for complex tasks
   - Affected ~12% of users (heavy users with >500 tasks)
   
   ## Lessons Learned
   - ✅ Rollback plan worked perfectly
   - ✅ Automatic backup saved data
   - ❌ Testing did not cover heavy users (>500 tasks)
   - ❌ Migration timeout too short
   
   ## Action Items
   - [ ] Increase migration timeout to 5min (#145)
   - [ ] Add progress bar for long migrations (#146)
   - [ ] Create test suite with large datasets (#147)
   - [ ] Beta program with heavy users before release (#148)
   ```

## Estimated Rollback Time
- **Preparation**: 5 minutes
- **Execution**: 10 minutes
- **Validation**: 5 minutes
- **TOTAL**: ~20 minutes (expected downtime)

## External Dependencies
- ✅ DATA backup automatically created during migration
- ✅ Git tags of previous versions available
- ❌ Does not depend on external services (DB, APIs)

## Data at Risk
- **High Risk**: Tasks created/edited after v2.0.0 deploy (do not exist in backup)
- **Low Risk**: Tasks existing before v2.0.0 (preserved in backup)

**Mitigation**: Export SQLite → DATA before rollback to preserve recent changes.

```bash
# Export script before rollback
python -c "
import sqlite3, data
conn = sqlite3.connect('~/.config/clarify/clarify.db')
cursor = conn.execute('SELECT * FROM tasks')
tasks = [dict(zip([col[0] for col in cursor.description], row)) for row in cursor.fetchall()]
data.dump({'tasks': tasks}, open('rollback-export.data', 'w'), indent=2)
"
# Users can manually merge changes later
```

## Contact Persons
- **Rollback Decision**: @lead-dev (Josué)
- **Technical Execution**: @dev-team
- **User Communication**: @support-team

---
**Created**: 2024-01-15
**Last Update**: 2024-01-15
**Tested**: ❌ No (run dry-run before deploy)
```

**Feature Flags - Alternative to Rollback**:

```python
# Instead of full rollback, use a feature flag to disable feature

class Config:
    """Configuration with feature flags."""
    
    # Feature flag - remote control
    SQLITE_STORAGE_ENABLED = os.getenv("CLARIFY_SQLITE_ENABLED", "true").lower() == "true"
    
    def get_storage_backend(self):
        """Get storage backend based on feature flag."""
        if self.SQLITE_STORAGE_ENABLED:
            return SQLiteStorage()
        else:
            return DATAStorage()  # Safe fallback

# In case of problem, disable remotely:
# export CLARIFY_SQLITE_ENABLED=false
# Or via config file / admin dashboard

# Users automatically revert to DATA without reinstalling
```

**Reversible Migrations**:

```python
# Migrations must be reversible

class MigrationV2:
    """Migration from DATA to SQLite - REVERSIBLE."""
    
    def up(self):
        """Migrate DATA → SQLite."""
        # 1. Create DATA backup
        shutil.copy("tasks.data", "tasks.data.backup")
        
        # 2. Create SQLite schema
        self._create_sqlite_schema()
        
        # 3. Migrate data
        self._migrate_data_to_sqlite()
        
        # 4. DO NOT delete DATA (keep for rollback)
        # os.remove("tasks.data")  ❌ NEVER do this
    
    def down(self):
        """Rollback SQLite → DATA."""
        if not os.path.exists("tasks.data.backup"):
            raise RollbackError("Backup DATA not found - cannot rollback!")
        
        # 1. Restore backup
        shutil.copy("tasks.data.backup", "tasks.data")
        
        # 2. Remove SQLite
        os.remove("clarify.db")
        
        print("✅ Rollback complete - using DATA storage")
```

**Rollback Plan Checklist**:

```markdown
### Rollback Plan Checklist - Task #XX

#### Planning
- [ ] **Criteria**: Clear criteria for when to execute rollback
- [ ] **Steps**: Detailed step-by-step documented
- [ ] **Time**: Estimated rollback time calculated
- [ ] **Dependencies**: External dependencies identified
- [ ] **Data**: Data loss risk assessed

#### Preparation
- [ ] **Backup**: Automated backup mechanism implemented
- [ ] **Tags**: Git tags of stable versions created
- [ ] **Scripts**: Rollback scripts tested in staging
- [ ] **Contacts**: Contact persons defined

#### Validation
- [ ] **Dry-run**: Rollback tested in staging environment
- [ ] **Smoke Tests**: Smoke tests defined for post-rollback validation
- [ ] **Communication**: Communication template prepared
- [ ] **Post-mortem**: Post-mortem template created
```

**Why Rollback Plans are critical**:
- ✅ **Confidence**: Team can make bold deploys knowing they can revert
- ✅ **Downtime**: Minimizes downtime (20min vs hours debugging)
- ✅ **Data**: Protects user data (backup strategy)
- ✅ **Communication**: Prepared template = fast and clear communication
- ✅ **Learning**: Structured post-mortem generates learning

---

### 13. **Commit and Push**
- **Format**: Conventional Commits (feat/fix/docs/refactor/test)
- **Message**: Descriptive, complete, with context
- **Frequency**: 1 commit per task or logical group of changes

**Commit Message Structure**:
```
<type>: <short description> (<version>)

<ORIGINAL PROBLEM>:
- [Problem context]
- [Why it was necessary to solve]

<IMPLEMENTED SOLUTION>:
✅ [Feature/function 1]
   - [Technical detail]
✅ [Feature/function 2]
   - [Technical detail]

✅ [TESTS]:
   - [Quantity] unit tests ([status])
   - [Tested categories]

<MODIFIED FILES>:
- [file1.py] (+X lines)
- [file2.py] (~Y lines)
- [tests/test_X.py] (NEW - Z lines)
- [docs/REQUIREMENTS.md] (updated statistics)

<UPDATED STATISTICS>:
- [CATEGORY]: X → Y complete (A% → B%)
- TOTAL: X → Y complete (A% → B%)

<USAGE EXAMPLE>: (if applicable)
  [Practical demonstration]

Refs: [related documentation]
Closes: Task #X (vX.X.X)
```

**Real Example** (Task Example):
```bash
git add src/ tests/ docs/REQUIREMENTS.md
git commit -m "feat: complete Task Example - Feature Update System (vX.Y.Z)

ORIGINAL PROBLEM:
- vX.Y.Z implementation used string_similarity() (INCORRECT)
- Did not detect duplicate values, only name similarity
...

✅ IMPLEMENTED SOLUTION:
✅ extract_all_keys_from_obj()
   - Supports Obj AND dict type
   - Returns Dict[str, str] (path → value)
...

Closes: Task Example (vX.Y.Z)"

git push
```

---

## 🏆 Professional Quality Criteria

Every implementation must meet **100% of these criteria**:

| # | Criterion | Description | Validation |
|---|---|---|---|
| 1 | **Modular Architecture** | Each feature in a separate module | Own file in `src/` |
| 2 | **Type Hints** | 100% of parameters typed | `def func(x: int) -> str:` |
| 3 | **Docstrings** | All public functions documented | Args, Returns, Examples |
| 4 | **Error Handling** | Try/except with clear messages | `except Exception as e:` |
| 5 | **Tests** | Unit + integration (100% coverage) | `tests/test_*.py` passing |
| 6 | **Semantic Commits** | Conventional Commits | `feat:`, `fix:`, `docs:` |
| 7 | **Documentation** | REQUIREMENTS.md + SPECIFICATIONS.md | Updated and complete |
| 8 | **Clean Code** | PEP8, semantic names, DRY | Functions < 50 lines |

---

## 📊 Practical Application: Task Example (Complete Example)

### Initial Situation
```markdown
Pending tasks in the SHOULD HAVE category:
[ ] Complex Feature Example (VERY COMPLEX)
[ ] Semantic AI Search (VERY COMPLEX)
[⚠️] Feature Update (PARTIAL - simpler!) ✅ CHOSEN
[ ] Google Translate API integration (COMPLEX)
```

### Planned Sprint
```
vX.Y.Z: Complete Task Example
Estimate: 3-4 hours
Complexity: MEDIUM (simpler than the others)
```

### Execution (Simplicity Protocol 1)

**1. Read Documentation** ✅
- Read: `docs/FEATURE_SPEC.md` (662 lines)
- Understood: string similarity vs. value equality problem

**2. Choose Simple Task** ✅
- Task Example is **simpler** than text editor or AI
- Clear scope: 2 main functions + integration

**3. Ask Questions** ✅
- Asked: "How many words to get? 3-5?"
- Answer: "Default 30 characters"
- Asked: "Convert to camelCase?"
- Answer: "Yes, remove accents"
- Asked: "Name conflicts?"
- Answer: "Smaller line wins, don't touch if values are different"

**4. Sprint** ✅
- 6 subtasks planned (including questions)
- Estimated time: 3h45min

**5. Implement with Architecture** ✅
```
Order executed:
1. extract_all_keys_from_obj() (helper function - High Cohesion)
2. build_substitution_map_by_value() (main function - Low Coupling)
3. Update cli_dedupe() (integration - Dependency Injection)
4. Create tests (validation)
5. Documentation (finalization)

Applied Patterns:
- ✅ Separate modules (Reusability)
- ✅ Type hints in all functions
- ✅ Information Expert (GRASP): each function has the info it needs
- ✅ Low coupling: independent functions
- ✅ High cohesion: each function does ONE thing
```

**6. Run Tests** ✅
```
12 unit tests created:
- 4 tests for extract_all_keys_from_obj()
- 5 tests for build_substitution_map_by_value()
- 2 tests for apply_substitutions_to_file()
- 1 test for update_references_in_project()
Result: 12/12 passing (100%)
```

**7. Documentation** ✅
```
Files created/updated:
- docs/REQUIREMENTS.md (Task Example marked [X])
- docs/FEATURE_SPEC.md (already existed)
- tests/test_reference_updater.py (NEW - 350 lines)
Statistics: 59.6% → 60.6% (63 tasks complete)
```

**8. Commit and Push** ✅
```bash
Commit: 903bca4
Message: 60 lines (complete and detailed)
Status: pushed to GitHub ✅
```

### Final Result
✅ **Task Example 100% complete**
✅ **Simplicity Protocol 1: 10/10 steps completed** (v1.1 - 10 steps)
✅ **Real time: ~3h (within estimate)**
✅ **Zero bugs detected**
✅ **Professional documentation**

**Note**: This example uses v1.1 of the protocol (10 steps). v1.2 adds 2 more steps (GUI and CLI integration).

---

## 🎓 Lessons Learned

### ✅ What Works
1. **Choose the simplest**: Task Example was easier than text editor
2. **Incrementality**: Helper function → main → integration
3. **Tests first**: Detected 2 necessary adjustments before committing
4. **Complete documentation**: Facilitates future maintenance

### ❌ Anti-patterns to Avoid
1. **Don't start with the most difficult task**
   - ❌ "I'll do the text editor first (50h)"
   - ✅ "I'll do the tooltip preview first (30min)"

2. **Don't do everything at once**
   - ❌ "I'll implement everything in one giant function"
   - ✅ "I'll split into 3 testable functions"

3. **Don't skip tests**
   - ❌ "I'll test manually later"
   - ✅ "I'll create 12 unit tests now"

4. **Don't make generic commits**
   - ❌ `git commit -m "updates"`
   - ✅ `git commit -m "feat: Task Example with VALUE EQUALITY (60 lines)"`

---

## 📚 References

- **REQUIREMENTS.md**: Complete list of project tasks
- **vX.Y.Z-COMPARISON.md**: First protocol example
- **vX.Y.Z-SPECIFICATIONS.md**: Sprint with 3 simple tasks
- **vX.Y.Z-SPECIFICATIONS.md**: Rapid iterations
- **vX.Y.Z-SPECIFICATIONS.md**: 4 UX improvements
- **FEATURE_SPEC.md**: Example of detailed documentation

---

## 🔄 Continuous Cycle

Simplicity Protocol 1 is an **iterative cycle**:

```
┌──────────────────────────────────────────────┐
│  1. Read Documentation                       │
│  2. Choose Simplest Tasks                    │
│  3. Ask the Programmer Questions             │
│  4. Analyze and Study the Project            │
│  5. Plan Sprint (2-4 tasks, 3-4h)            │
│  6. Implement (GoF + GRASP architecture)     │
│  7. Verify GUI Integration                   │
│  8. Verify CLI Implementation                │
│  9. Test (100% coverage)                     │
│  10. Organize Project Root Folder            │
│  11. Document (TASKS + vX.X.X-SPECS)         │
│  12. Commit + Push (conventional)            │
└──────────────────────────────────────────────┘
           ↓
    ┌──────────────┐
    │    REPEAT    │ ← There are always simpler tasks!
    └──────────────┘
```

**Result**: Constant progress, professional code, zero technical debt.

---

### 13.5 **Sprint Retrospectives** (Optional - For Continuous Improvement)

**When to Apply**:
- ✅ Long-term projects (>3 months)
- ✅ Team work (2+ people)
- ✅ Iterative cycles (sprints, milestones)
- ✅ When you want to continuously improve the process
- ✅ After completing an important epic/milestone

**Do Not Apply If**:
- ❌ Ad-hoc solo project (no repetition)
- ❌ One-off script or prototype
- ❌ Single-deadline project (non-iterative)
- ❌ No commitment to improvement (retrospective is only valuable if it generates actions)

**What is a Sprint Retrospective?**

A meeting (or document, if solo) at the end of each sprint/milestone to reflect on:
- ✅ **What went well** (keep doing)
- ❌ **What didn't go well** (stop doing)
- 💡 **What we can improve** (start doing)
- 📊 **Progress metrics**

**Retrospective Template**:

```markdown
# Sprint Retrospective #5 - Clarify Project

**Date**: 2024-01-20
**Sprint**: 2024-01-08 → 2024-01-20 (2 weeks)
**Participants**: Josué (dev), Alice (reviewer)
**Milestone**: v2.0.0 - SQLite Migration

---

## 📊 Sprint Metrics

### Progress
- **Tasks Completed**: 8/10 (80%)
- **Story Points**: 21/25 (84%)
- **Bugs Found**: 3
- **Bugs Fixed**: 3
- **Commits**: 24
- **PRs**: 6 (5 merged, 1 pending)

### Quality
- **Test Coverage**: 87% (↑ 5% since previous sprint)
- **Code Review**: 100% (all PRs reviewed)
- **CI/CD**: 23/24 builds successful (95.8%)
- **Average PR → Merge Time**: 18h (goal: <24h) ✅

### Velocity
- **Planned Velocity**: 25 SP
- **Actual Velocity**: 21 SP
- **Efficiency**: 84% (goal: >80%) ✅

---

## ✅ What Went Well (Keep Doing)

### 1. Simplicity Protocol
**Impact**: HIGH
**What worked**: Following 13 steps ensured consistent quality.
**Evidence**: Zero production bugs in tasks that followed full protocol.
**Action**: Continue using, consider making mandatory for all devs.

### 2. Pre-commit Hooks
**Impact**: MEDIUM
**What worked**: Hooks caught 15 formatting errors before commit.
**Evidence**: Zero code review comments on formatting.
**Action**: Keep hooks, add bandit (security) to config.

### 3. Pair Programming on Complex Features
**Impact**: HIGH
**What worked**: SQLite migration (Task Example) done in pair = zero rework.
**Evidence**: PR approved first-time, no changes requested.
**Action**: Use pair programming for tasks with risk > MEDIUM.

---

## ❌ What Didn't Go Well (Stop Doing / Fix)

### 1. Too Much Manual GUI Testing
**Impact**: HIGH
**Problem**: GUI tested manually every time = 30min per task, repetitive.
**Evidence**: 8 tasks × 30min = 4 hours spent on manual tests.
**Root Cause**: Lack of automated GUI tests.
**Action**:
- [ ] Implement pytest-qt for automated GUI tests (Task Example)
- [ ] Create smoke test suite that runs in CI (Task Example)
- **Owner**: Josué | **Deadline**: Sprint #6

### 2. Scope Creep in Task Example
**Impact**: MEDIUM
**Problem**: Task "Migrate to SQLite" grew from 8 SP → 13 SP during sprint.
**Evidence**: Task took 3 days instead of 2 days estimated.
**Root Cause**: Underestimated complexity of migration + rollback plan.
**Action**:
- [ ] Add 25% buffer to "first-time" task estimates (Task Example)
- [ ] Split large epics into smaller tasks (<5 SP each)
- **Owner**: Alice | **Deadline**: Next planning

### 3. Delayed Documentation
**Impact**: LOW
**Problem**: ADRs created after PR merged, not during.
**Evidence**: ADR-004 committed 2 days after merge of PR #145.
**Root Cause**: Forgot to include ADR in PR checklist.
**Action**:
- [ ] Update PR template to include "ADR created?" (Task Example)
- [ ] Pre-commit hook to check if docs/adr/ was modified when src/ changes
- **Owner**: Josué | **Deadline**: Sprint #6

---

## 💡 Ideas for Improvement (Start Doing)

### 1. Weekly Micro-Retrospectives
**Proposal**: Short retrospective (10min) every Friday.
**Rationale**: Retrospective every 2 weeks = some lessons forgotten.
**Experiment**: Test for 4 weeks, evaluate if it adds value.
**Action**:
- [ ] Create micro-retro template (3 questions only)
- [ ] Schedule 10min every Friday 4 PM
- **Owner**: Alice | **Status**: Experimental

### 2. Refactoring Fridays
**Proposal**: Last sprint afternoon dedicated to refactoring/tech debt.
**Rationale**: Tech debt accumulating (TODO comments: 23 → 31 since last sprint).
**Experiment**: Dedicate 3h on Friday to clean tech debt.
**Action**:
- [ ] Create `tech-debt` tag in issue tracker
- [ ] Reserve 3h on Friday for tech debt sprint #6
- **Owner**: Josué | **Status**: Experimental

### 3. Automated Changelog Generation
**Proposal**: Automatically generate CHANGELOG.md from commits.
**Rationale**: Writing changelog manually = 20min repetitive per sprint.
**Solution**: Use `git-cliff` or `conventional-changelog`.
**Action**:
- [ ] Evaluate tools (git-cliff vs conventional-changelog)
- [ ] Integrate into CI pipeline
- **Owner**: Alice | **Deadline**: Sprint #7

---

## 📈 Comparison with Previous Sprints

| Metric | Sprint #3 | Sprint #4 | Sprint #5 | Trend |
|---|---|---|---|---|
| Velocity | 18 SP | 22 SP | 21 SP | ↔️ Stable |
| Coverage | 78% | 82% | 87% | ↗️ Improving |
| Production Bugs | 2 | 1 | 0 | ↗️ Excellent |
| PR→Merge Time | 36h | 24h | 18h | ↗️ Improving |
| Tech Debt Items | 18 | 23 | 31 | ↘️ **ALERT** |

**Analysis**:
- ✅ Quality improving (coverage ↑, bugs ↓)
- ✅ Efficiency improving (faster PRs)
- ⚠️ **Tech debt accumulating** - needs attention (Refactoring Fridays)

---

## 🎯 Action Items for Next Sprint

| # | Action | Owner | Deadline | Priority |
|---|---|---|---|---|
| #89 | Implement pytest-qt for GUI | Josué | Sprint #6 | 🔴 HIGH |
| #90 | Create CI smoke test suite | Josué | Sprint #6 | 🔴 HIGH |
| #91 | Add 25% buffer to estimates | Alice | Planning #6 | 🟡 MEDIUM |
| #92 | Update PR template (ADR) | Josué | Sprint #6 | 🟢 LOW |
| - | Test weekly micro-retros | Alice | Sprint #6 | 🧪 Experimental |
| - | Dedicate 3h Friday tech debt | Josué | Sprint #6 | 🧪 Experimental |

**Tracked in**: [GitHub Project - Sprint #6](link)

---

## 💬 Team Feedback

### Josué
> "Simplicity Protocol is working very well. I feel that quality is better. Concerned about tech debt accumulating - let's try Refactoring Fridays."

### Alice
> "Code reviews are faster and smoother. Loved pair programming on the SQLite migration. Suggestion: can we do retrospectives more frequently? Every 2 weeks feels like a long time."

---

## 📚 Lessons Learned

### Technical
1. **SQLite Migrations**: Always create automatic backup + rollback plan.
2. **Feature Flags**: Better than full rollback for large features.
3. **GUI Testing**: Pytest-qt saves significant time vs manual.

### Process
1. **Retrospectives**: 2 weeks = good, but weekly micro-retros can add value.
2. **Estimates**: First time doing something = add 25% buffer.
3. **Tech Debt**: Needs dedicated time, not "when there's leftover time."

### Personal
1. **Pair Programming**: Worth it for complex/critical tasks.
2. **Communication**: PRs with rich context = faster reviews.
3. **Documentation**: ADRs should be created DURING PR, not after.

---

**Next Retrospective**: 2024-02-03 (Sprint #6)
**Format**: In-person or updated document
**Facilitator**: Alice (rotating)
```

## 🎯 Final Message

> "I want a complete and professional job!"

**This protocol guarantees**:
- ✅ Professional quality (13 mandatory + 10 advanced optional steps)
- ✅ Incremental progress (from simple to complex)
- ✅ Complete documentation (never forget what was done)
- ✅ Tested and secure code (100% reliable)
- ✅ Verified integration (functional GUI + CLI)
- ✅ Organized commits (clean history)
- ✅ **[NEW v2.0]** Enterprise practices (Security, CI/CD, ADRs, Retrospectives)

**Reread this document before each sprint!**

---

**Version**: 2.0
**Last updated**: January 20, 2024
**Maintained by**: Josué Amaral
**Status**: ACTIVE - Advanced protocol for critical/enterprise projects
```
