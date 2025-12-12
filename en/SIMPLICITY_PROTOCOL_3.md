# Simplicity 3 Protocol - Solo Developer in Production

**Author**: Josué Amaral
**Creation Date**: December 02, 2025
**Version**: 3.1
**Last Update**: December 09, 2025
**Objective**: Hybrid methodology for **solo developers** with application in **production**

---

## 🎯 Why Does Simplicity 3 Exist?

### Project Context
- 👤 **Solo Developer**: You program alone (without a team)
- 🚀 **Production**: Application has real users depending on it
- ⚠️ **Critical**: Bugs affect users, downtime has impact
- 📈 **Evolutive**: Long-term project, not a prototype

### Why NOT Simplicity 1?
❌ **Simplicity 1** is **insufficient for production**:
- ❌ No security checklist → Vulnerabilities can go to production
- ❌ No CI/CD automation → Manual validation = human errors
- ❌ No rollback plan → If it breaks in production, you're debugging alone
- ❌ No profiling → Performance degrades without you noticing
- ❌ Basic documentation → You forget complex decisions after 3 months

**Real Risk**: Simple application today = giant technical debt in 6 months.

### Why NOT Simplicity 2?
❌ **Simplicity 2** has **team overhead** unnecessary for a solo developer:
- ❌ **Peer Code Review** (Step 9.5) → You have no peers
- ❌ **Formal Sprint Retrospectives** (Step 13.5) → Overkill for one person
- ❌ **Formal ADRs** (Step 11.5) → Can be simplified to decision notes
- ❌ **Accessibility WCAG** (Step 8.5) → Only if the app is public/accessible
- ❌ **API Documentation Sphinx** (Step 6.6) → Docstrings are sufficient

**Real Problem**: Bureaucracy consumes development time without real gain for a solo developer.

### ✅ Simplicity 3 - Hybrid Solution

**Philosophy**: **Production security and automation** WITHOUT team overhead.

**Formula**:
```
Simplicity 3 = Simplicity 1 Base (13 steps)
                 + 3 MANDATORY production steps (Security, CI/CD, Rollback)
                 + 3 pragmatic OPTIONAL steps (Matrix, Profiling, ADR Notes)
                 = 16-19 total steps
```

**Additional MANDATORY Steps** (vs Simplicity 1):
1. ⭐ **Step 6.5: OWASP Security Checklist** - CRITICAL for production
2. ⭐ **Step 10.6: CI/CD Quality Gates** - Essential automation
3. ⭐ **Step 12.5: Rollback Plans** - Deployment safety

**Adapted OPTIONAL Steps** (when it makes sense):
4. 📊 **Step 2.5: Decision Matrix** - When you have 10+ tasks to prioritize
5. ⚡ **Step 10.5: Profiling** - For slow features (>1s)
6. 📝 **Step 11.5: Decision Notes** - Simplified ADR (not formal)

**Removed from Simplicity 2** (don't make sense for solo dev):
- ❌ Step 9.5: Peer Code Review
- ❌ Step 13.5: Formal Sprint Retrospectives
- ❌ Step 8.5: Accessibility WCAG (unless app is public)
- ❌ Step 6.6: Formal API Documentation (docstrings are sufficient)

---

## 📊 Protocol Comparison

| Aspect | Simplicity 1 | Simplicity 3 | Simplicity 2 |
|---------|----------------|----------------|----------------|
| **Steps** | 13 mandatory | 16 oblig + 3 opt | 13 oblig + 10 opt |
| **Scenario** | Prototypes/internal | **Solo in production** | Enterprise teams |
| **Security** | ❌ No | ✅ OWASP mandatory | ✅ OWASP mandatory |
| **CI/CD** | ❌ No | ✅ Mandatory | ✅ Mandatory |
| **Rollback** | ❌ No | ✅ Mandatory | ✅ Mandatory |
| **Code Review** | ❌ No | ❌ Solo | ✅ Peers |
| **Retrospectives** | ❌ No | ❌ Solo | ✅ Team |
| **Overhead** | Low | **Medium** | High |
| **Production** | ❌ Not recommended | ✅ **IDEAL** | ✅ Yes |
| **Time/Task** | ~2-3h | ~3-4h | ~4-6h |

---

## 🎯 When to Use Simplicity 3?

### ✅ Use Simplicity 3 IF:
- ✅ You program **alone** (solo developer)
- ✅ Application is or will go to **production**
- ✅ You have **real users** depending on it (not a prototype)
- ✅ Bugs have **impact** (downtime, data loss)
- ✅ It's a **long-term project** (>6 months)
- ✅ You need **security** (user data, LGPD/GDPR)
- ✅ You want **automation** (CI/CD to not rely on memory)

### ❌ DO NOT use Simplicity 3 IF:
- ❌ Disposable prototype/POC → Use **Simplicity 1**
- ❌ Single-use script → Use **Simplicity 1**
- ❌ Team of 2+ people → Use **Simplicity 2** (has code review)
- ❌ Non-critical internal app → Use **Simplicity 1**
- ❌ Learning/experimenting → Use **Simplicity 1**

---

**Changelog v3.1** (09/12/2025):
- ✅ **[STEP 3]** Added recommendation for AI to provide suggestions and guesses for questions
- ✅ Recommended format: "❓ Question + 💡 AI Suggestion + Options A/B/C"
- ✅ Rationale: Speeds up decisions, reduces cognitive load, maintains consistency with existing code
- ✅ Classification: **OPTIONAL but HIGHLY RECOMMENDED**

**Changelog v3.0** (02/12/2025):
- ✅ **[HYBRID]** Created Simplicity 3 Protocol for solo developer in production
- ✅ Base: Simplicity 1 (13 steps) + 3 mandatory production steps
- ✅ **NEW MANDATORY**:
  - Step 6.5: OWASP Security Checklist (⭐ HIGH PRIORITY)
  - Step 10.6: CI/CD Quality Gates (⭐ HIGH PRIORITY)
  - Step 12.5: Rollback Plans (⭐ HIGH PRIORITY)
- ✅ **PRAGMATIC OPTIONAL**:
  - Step 2.5: Decision Matrix (when 10+ tasks)
  - Step 10.5: Profiling and Optimization (slow features)
  - Step 11.5: Decision Notes (simplified ADR)
- ✅ **REMOVED** (don't make sense for solo dev):
  - ❌ Peer Code Review (no peers)
  - ❌ Formal Sprint Retrospectives (overkill solo)
  - ❌ Accessibility WCAG (unless public)
  - ❌ Formal API Documentation (docstrings sufficient)
- ✅ Detailed Rationale: Why not Simplicity 1 or 2
- ✅ Comparative table of the 3 protocols
- ✅ Total: 16 mandatory + 3 optional = 16-19 steps

**Changelog v1.8** (02/12/2025):
- ✅ **[REORGANIZATION]** Code Review integrated into CLI and GUI steps
- ✅ Step 7: Verify CLI Implementation (includes 9 quality criteria)
- ✅ Step 8: Verify GUI Implementation (includes 9 quality criteria)
- ✅ Step 9: Verify Integration with Main Program (kept as separate step)
- ✅ 9 Criteria: Omission, Ambiguity, Incorrect Fact, Redundancy, Inconsistency, Lack of Integration, Lower Cohesion, Higher Coupling, Extraneous Information
- ✅ Review integrated into CLI/GUI verification process
- ✅ Total steps: 12 → 13 (integration verification added after GUI)

**Changelog v1.7** (02/12/2025):
- ✅ **[CRITICAL]** Added Step 8.5: Code Review (BEFORE tests)
- ✅ 9 Quality Criteria: Omission, Ambiguity, Incorrect Fact, Redundancy, Inconsistency, Lack of Integration, Lower Cohesion, Higher Coupling, Extraneous Information
- ✅ Complete review checklist (36 verification items)
- ✅ Recommended tools (pylint, vulture, radon, black, isort)
- ✅ Detailed CLI and GUI review process
- ✅ Practical examples of problems and corrections
- ✅ Integration with Step 9 (test after review)
- ✅ Total steps: 12 → 13 (8.5 added between 8 and 9)

**Changelog v1.6**:
- ✅ **[ADVANCED]** Added Step 9.2: Tests in Threads/Processes with Monitoring
- ✅ Test execution in separate process (`multiprocessing.Process`)
- ✅ Real-time logging via `Queue` (progress of each test)
- ✅ Manual cancellation at any time (graceful Ctrl+C)
- ✅ Global + individual timeout (double protection)
- ✅ Real-time statistics (passed/failed/elapsed)
- ✅ Full implementation of `test_runner_monitored.py` (~150 lines)
- ✅ Additional optional checklist (6 items)

**Changelog v1.5**:
- ✅ **[CRITICAL]** Added Step 9.1: Security in Tests
- ✅ 7 mandatory solutions to prevent infinite loops and timeouts
- ✅ Mandatory maximum timeout (30s per test)
- ✅ Mandatory headless environment for GUI tests (QT_QPA_PLATFORM=offscreen)
- ✅ Mandatory dry-run before executing tests (syntax + import + collect)
- ✅ Security checklist with 6 mandatory items
- ✅ Golden rules and safe commands documented
- ✅ Lessons learned from Task Example (infinite loop >1h)

**Changelog v1.4**:
- ✅ Reorganized final order: Implement → Integrate GUI → CLI → Test → Organize → Document → Commit
- ✅ Tests moved to AFTER integration verifications (test integrated system)
- ✅ Organize root folder moved to BEFORE documentation (document clean state)
- ✅ Logic: Integrate → Test integration → Clean repository → Document final state

**Changelog v1.3**:
- ✅ Reorganized step order: GUI and CLI Integration Verification now come BEFORE Documentation
- ✅ New order: Tests → GUI Integration → CLI → Documentation → Organize → Commit
- ✅ Logic: Verify integration before documenting ensures documentation reflects the real state

**Changelog v1.2**:
- ✅ Added Step 8: Verify integration with main program
- ✅ Added Step 9: Verify CLI implementation with parameter passing
- ✅ Total steps: 10 → 12

---

## 🎯 Core Philosophy

> "There will always be complex tasks to do, but also those that are more difficult and those that are easier. **I want you to always start with the easiest ones**."

**Principle**: From simple to complex, incremental, professional, and complete.

**NEW v3.0**: + **Production security and automation** without team overhead.

---

## 📋 Protocol Backbone (16 Mandatory Steps)

**Executive Summary** (⭐ = NEW vs Simplicity 1):
1. 📚 Read the documentation
2. ✅ Choose simpler tasks
   - 2.5 📊 [OPTIONAL] Decision Matrix (when 10+ tasks)
3. ❓ Ask questions until 100% clear
4. 🔍 Analyze and study the project
5. 🎯 Do sprints for the simpler tasks
6. 💻 Implement with professional architecture (GoF + GRASP)
   - 6.5 🔒 ⭐ **OWASP Security Checklist** (MANDATORY)
7. ⌨️ Verify CLI Implementation + Code Review (9 criteria)
8. 🖥️ Verify GUI Implementation + Code Review (9 criteria)
9. 🔗 Verify Integration with Main Program
🔟 🧪 Run tests (100% coverage)
   - 10.5 ⚡ [OPTIONAL] Profiling and Optimization (if >1s)
   - 10.6 🤖 ⭐ **CI/CD Quality Gates** (MANDATORY)
1️⃣1️⃣ 🧹 Organize root folder
   - 11.5 📝 [OPTIONAL] Decision Notes (simplified ADR)
1️⃣2️⃣ 📝 Fill documentation
   - 12.5 🔄 ⭐ **Rollback Plans** (MANDATORY)
1️⃣3️⃣ 🚀 Commit and push

**Total**: 13 base + 3 new mandatory ⭐ + 3 optional = **16-19 steps**

### 1️⃣ **Read the Documentation**
- Consult `docs/REQUIREMENTS.md` to understand the project context
- Review previous specifications (`v2.9.X-SPECIFICATIONS.md`)
- Understand dependencies and existing architecture
- Check examples in `tests/files/` when applicable

**Why?**: Avoid rework and ensure coherence with existing code.

---

### 2️⃣ **Choose the Simplest Tasks**
- **Golden Rule**: Always start with the **easiest tasks to implement**
- Even in a list of complex tasks, **there are always simpler ones than others**
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

### 2️⃣.5️⃣ **Objective Decision Matrix** [OPTIONAL]

**When to Use**: When you have 10+ tasks and it's not obvious which is simplest.

**What it is**: Scoring system with 5 criteria (0-5 points each):
1. **Technical Simplicity** (code, algorithm, new concepts)
2. **Dependencies** (files to modify, modules affected)
3. **Impact** (user value, frequency of use)
4. **Clarity** (defined requirements, examples)
5. **Risk** (breaking code, reversibility)

**Formula**:
```
Priority = (Simplicity × 2) + Dependencies + (Impact × 1.5) + Clarity + Risk
```

**Interpretation**:
- **30-35 points**: 🟢 IDEAL - Start immediately
- **20-29 points**: 🟡 GOOD
- **10-19 points**: 🟠 MEDIUM
- **0-9 points**: 🔴 COMPLEX - Leave for last

**Quick Example**:

| Task | Simpl | Dep | Imp | Clar | Risc | **Score** | Decision |
|------|-------|-----|-----|------|------|-----------|---------|
| **Tooltip Preview** | 5 | 5 | 3 | 5 | 5 | **33.5** 🟢 | **CHOOSE** |
| **Integrated Editor** | 1 | 2 | 5 | 4 | 2 | **20.5** 🟡 | Later |

**When NOT to use**:
- ❌ Only 1-3 tasks (obvious which is simplest)
- ❌ Urgent bugfix (ignores score)
- ❌ Blocking task (absolute priority)

📘 **Full details**: See `PROTOCOLO_SIMPLICIDADE_2.md` - Step 2.5 (template, examples)

---

### 3️⃣ **Ask Questions and More Questions to the Developer**
- **CRITICAL**: Never assume or guess requirements
- Ask **all necessary questions** until **100% of doubts are clarified**
- Validate understanding before starting implementation
- 🤖 **[NEW v3.1]** The AI **CAN and IS HIGHLY RECOMMENDED** to provide **suggestions and guesses** for the answer to each question (optional, but encouraged)

**Recommended Question Format with Suggestions**:
```
❓ Question: "How should it behave when [scenario X]?"
💡 AI Suggestion: "Based on existing code, I suggest [option A] because [reason Y]."
Options: A) [option A] | B) [option B] | C) [option C]
```

**Why AI Suggestions Are Important**:
- ✅ Speeds up decisions when the developer is undecided
- ✅ AI has context of existing code and can suggest consistent patterns
- ✅ Reduces developer's cognitive load (they only validate, don't create from scratch)
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
   - "Where to save the results?"

5. **Understanding Validation**:
   - "I understand you want [X]. Is that correct?"
   - "My proposed solution is [Y]. Does it make sense?"
   - "Can I start or did I forget something?"

**Real Example (Task Example)**:
```
❓ "Get first N words (how many? 3-5?)?"
✅ Answer: "Default can be 30 characters"

❓ "Convert to camelCase removing accents?"
✅ Answer: "Yes, accents should be removed"

❓ "Name conflicts: how to resolve?"
✅ Answer: "If they have the same parent key, don't touch. Shorter line wins."
```

**Why?**: Saves time, prevents rework, ensures the solution meets exactly what was requested.

---

### 4️⃣ **Analyze and Study the Project**
- **CRITICAL**: After clarifying all doubts, **study the code before implementing**
- Read relevant documentation (README, docs/, comments in code)
- Understand existing architecture and patterns used
- Check dependencies and necessary imports
- Identify reusable functions/classes

**Analysis Checklist**:
1. **Documentation Reading**:
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
   - Is it necessary to refactor anything before implementing?
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
→ Result: Implementation in 2h instead of 5h (60% saving)
```

**Why?**: Avoids refactorings, saves time, ensures consistent code with the existing base.

---

### 5️⃣ **Do Sprints for the Simplest Tasks**
- Group 2-4 related tasks into a sprint
- Estimate total time: **maximum 3-4 hours** per sprint
- Maintain focus: **one sprint = one version (e.g., vX.Y.Z)**

**Sprint Structure**:
```
Sprint vX.Y.Z (Task Example):
├── Task Example: Feature Update (estimated 3h)
│   ├── Subtask 1: Ask questions to the developer (15min)
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

#### 🔄 **Code Reuse with Modules**
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
- **High Cohesion**: Each module/class has a single clear responsibility
- **Low Coupling**: Independent modules, communication via interfaces

**Example**:
```python
# ✅ HIGH COHESION: Each class does ONE thing
class KeyExtractor:
    """Only extracts keys from structures"""
    def extract(self, data) -> Dict[str, str]: ...

class SubstitutionMapBuilder:
    """Only builds substitution map"""
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
        # Does extraction + build + update + logging + GUI
        # Imports 20 different modules
        # Impossible to test in isolation
```

#### 🏗️ **GoF (Gang of Four) Patterns**
Apply design patterns when appropriate:

1. **Strategy Pattern** (algorithm selection at runtime):
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

2. **Factory Pattern** (complex object creation):
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

#### 🎨 **GRASP (General Responsibility Assignment Software Patterns)**

1. **Information Expert**: Assign responsibility to the one with the information
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
    # Direct access to the dictionary's internal structure
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
    # No reuse
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

### 6️⃣.5️⃣ **OWASP Security Checklist** ⭐ [MANDATORY]

> **CRITICAL FOR PRODUCTION**: This step is **MANDATORY** in Simplicity 3.

**Why mandatory for production**:
- ✅ Vulnerabilities affect **real users**
- ✅ You are **alone** - no second pair of eyes
- ✅ LGPD/GDPR applies to user data
- ✅ Quick checklist (10-15min) prevents costly problems

**OWASP Top 10 - Simplified Checklist**:

```markdown
## Security Checklist - Task #XX

### 1. Injection (SQL, Command, Code)
- [ ] All SQL queries use **parametrization** (no f-strings)?
- [ ] Shell commands sanitized (**shlex.quote()** or avoided)?
- [ ] `eval()`, `exec()`, `__import__()` NOT used?

### 2. Authentication
- [ ] Passwords NEVER in plaintext (use **bcrypt/argon2**)?
- [ ] Tokens/sessions have **expiration** and **invalidation**?
- [ ] Rate limiting on login endpoints (prevent brute-force)?

### 3. Sensitive Data
- [ ] Sensitive data **NOT** in logs (passwords, tokens, CPF)?
- [ ] Sensitive files have **correct permissions** (600/700)?
- [ ] Secrets in **environment variables** (not hardcoded)?

### 4. XML/XXE (if using XML)
- [ ] XML parser has **entity expansion disabled**?
- [ ] Schema validation before parsing?

### 5. Access Control
- [ ] Permissions checked **before** critical operations?
- [ ] User cannot access data of **other users**?
- [ ] Paths validated (no **path traversal**: `../../etc/passwd`)?

### 6. Insecure Configurations
- [ ] **DEBUG=False** in production?
- [ ] Secrets **NOT** committed to Git (.env in .gitignore)?
- [ ] Dependencies updated (**pip-audit** without vulnerabilities)?

### 7. XSS (if web/HTML)
- [ ] HTML output **escaped** (use template engine)?
- [ ] User input **sanitized** before display?

### 8. Insecure Deserialization
- [ ] **pickle** avoided (or validated if necessary)?
- [ ] DATA preferred over pickle for external data?

### 9. Vulnerable Dependencies
- [ ] `pip-audit` executed and no HIGH/CRITICAL issues?
- [ ] Dependencies updated (last 6 months)?

### 10. Logs/Monitoring
- [ ] Critical operations **logged** (create, update, delete)?
- [ ] Logs **DO NOT** contain sensitive data?
```

**INSECURE vs SECURE Example**:

```python
# ❌ INSECURE - SQL Injection
def get_user(username):
    query = f"SELECT * FROM users WHERE name='{username}'"
    return db.execute(query)
# Attack: username = "admin' OR '1'='1"

# ✅ SECURE - Parameterized
def get_user(username):
    query = "SELECT * FROM users WHERE name=?"
    return db.execute(query, (username,))

# ❌ INSECURE - Command Injection
def backup_file(filename):
    os.system(f"tar -czf backup.tar.gz {filename}")
# Attack: filename = "file.txt; rm -rf /"

# ✅ SECURE - List of args
def backup_file(filename):
    subprocess.run(["tar", "-czf", "backup.tar.gz", filename], check=True)

# ❌ INSECURE - Password in log
logger.info(f"User {username} logged in with password {password}")

# ✅ SECURE - No sensitive data
logger.info(f"User {username} logged in successfully")

# ❌ INSECURE - Path Traversal
def read_file(user_path):
    with open(f"/app/data/{user_path}") as f:
        return f.read()
# Attack: user_path = "../../etc/passwd"

# ✅ SECURE - Validate path
def read_file(user_path):
    safe_path = os.path.abspath(f"/app/data/{user_path}")
    if not safe_path.startswith("/app/data/"):
        raise ValueError("Invalid path")
    with open(safe_path) as f:
        return f.read()
```

**Automated Tools** (run BEFORE commit):

```bash
# 1. Vulnerabilities in dependencies
pip install pip-audit
pip-audit
# If HIGH/CRITICAL reported, update deps

# 2. Security linter
pip install bandit
bandit -r . -ll  # Low confidence + Low severity
# Review reported issues

# 3. Detected secrets
pip install detect-secrets
detect-secrets scan > .secrets.baseline
# Review if any secret leaked
```

**Pre-commit Hook** (automate):

```yaml
# .pre-commit-config.yaml
repos:
  - repo: https://github.com/PyCQA/bandit
    rev: 1.7.6
    hooks:
      - id: bandit
        args: ['-ll']
  
  - repo: https://github.com/Yelp/detect-secrets
    rev: v1.4.0
    hooks:
      - id: detect-secrets
```

**When to SKIP the checklist** (rarely):
- ❌ Internal code without sensitive data
- ❌ Disposable single-use script
- ❌ Non-production prototype

**Estimated Time**: 10-15 minutes per task.

📘 **Complete checklist with 10 examples**: See `PROTOCOLO_SIMPLICIDADE_2.md` - Step 6.5

---

### 7️⃣ **Verify CLI Implementation + Code Review**
- **CRITICAL**: Verify that the new functionality is available via **CLI (Command Line Interface)**
- **IMPORTANT**: During verification, apply the **9 Quality Criteria** to the CLI code
- It's not enough to implement GUI, important functionalities must have a **CLI interface** for automation
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
- ✅ **Menu accessible**: Verify if item appears in Tools menu
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

**Why?**: Ensure that the implemented code is **really usable** by the end user, not just "works in isolation".

---

### 8️⃣ **Verify GUI Implementation + Code Review**
- **CRITICAL**: Verify that components are **integrated into the main program** and accessible
- **IMPORTANT**: During verification, apply the **9 Quality Criteria** to the GUI code
- It's not enough to implement the module/dock, it needs to be **accessible and functional** in the app
- Verify menu, imports, initialization, connections, and code quality

**Part A - GUI Functional Verification (Integration)**:

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
- ✅ **Menu accessible**: Verify if item appears in Tools menu
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
   - [ ] Uniform naming (ed_ for QLineEdit, btn_ for QPushButton)?
   - [ ] Consistent message style?
   - [ ] Consistent layout spacing/margin?

6. **🔗 Lack of Integration** - GUI connected:
   - [ ] Dock added to MainWindow?
   - [ ] Menu item connected to dock.show()?
   - [ ] Custom signals connected?
   - [ ] Import present in app.py?

7. **🧩 Lower Cohesion** - Focused dock:
   - [ ] Dock only handles UI (not business logic)?
   - [ ] Complex logic in separate module?
   - [ ] Each method has a single responsibility?

8. **🔗 Higher Coupling** - Decoupled GUI:
   - [ ] Dock does not depend on internal implementation of other docks?
   - [ ] Communication via signals/slots (not direct calls)?
   - [ ] GUI testable independently (mock business logic)?

9. **🗑️ Extraneous Information** - Clean code:
   - [ ] No forgotten print() debugs?
   - [ ] No unresolved TODOs?
   - [ ] No unused widgets?

**GUI Review Example Applied**:
```python
# ❌ BEFORE - Omission, Ambiguity, Higher Coupling
class NewComponent(QDockWidget):
    def __init__(self):
        self.btn = QPushButton("Convert")  # Vague label
        self.btn.clicked.connect(self.convert)  # No error handling
    
    def convert(self):
        data = open(self.ed_file.text()).read()  # No validation, no closing
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
            # Read file with context manager (ensures closing)
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

### 9️⃣ **Verify Integration with Main Program**
- **CRITICAL**: After implementing CLI and GUI, **verify that everything is integrated and working in the context of the main program**
- It's not enough to have isolated working code; it needs to be **accessible and operational** in the application
- Verify complete flow: menu → action → result
- Manually test functionality in the running program

**Complete Integration Checklist**:

1. **GUI Full Flow Test**:
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

2. **CLI Full Flow Test**:
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

3. **Inter-component Integration Test**:
   ```bash
   # Example: Convert text → Open in editor
   [ ] Clicking "Open in Editor" in the Text to DATA Converter opens the Editor?
   [ ] DATA is loaded correctly in the Editor?
   [ ] Editor can save the result?
   
   # Example: Search → Open file
   [ ] Clicking a search result opens the correct file?
   [ ] Cursor position goes to the correct line?
   ```

4. **Robustness Test**:
   ```bash
   # Error scenarios
   [ ] File not found displays clear message?
   [ ] Invalid input is handled gracefully?
   [ ] Canceled operation doesn't leave inconsistent state?
   [ ] Resources are released correctly (files closed, memory)?
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
# ❌ PROBLEM FOUND DURING INTEGRATION:
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
1. ❓ "Can the end user easily access the functionality?"
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

### 🔟 **Run Tests**
- **Mandatory**: Unit tests for each public function
- **Goal**: 100% coverage of implemented functionalities
- **Tools**: `unittest` (native) or `pytest`
- **CRITICAL**: Test the system **after integration** (GUI + CLI integrated)
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
- Validates that features truly work in the application context
- Avoids false positives (tests pass but feature is not accessible)
- Code has already been reviewed, so tests validate **quality code**

**Why?**: Ensure quality, prevent regressions, facilitate future maintenance.

---

#### 🛡️ **Step 9.1 - Security in Tests (CRITICAL)**

**Problem Identified** (Task Example - 01/12/2025):
- GUI tests froze in an **infinite loop** for >1 hour without timeout
- No automatic deadlock or freeze detection
- Tests waited for non-existent X11 display (headless environment)

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

**Why?**: Prevent infinite freezes, protect development time, ensure reliable tests.

---

### 🔟.5️⃣ **Profiling and Optimization** [OPTIONAL]

**When to Use**: Critical feature is **slow** (>1s for user).

**Tools**:
```bash
# CPU profiling
python -m cProfile -s cumulative app.py > profile.txt

# Memory profiling
pip install memory_profiler
python -m memory_profiler app.py
```

**Example**:
```python
# ❌ SLOW - O(n²) 5.2s for 1000 tasks
def find_duplicates_slow(tasks):
    for i, t1 in enumerate(tasks):
        for j, t2 in enumerate(tasks):
            if i != j and t1.title == t2.title:
                # duplicated

# ✅ FAST - O(n) 0.02s (260x faster)
def find_duplicates_fast(tasks):
    seen = {}
    for task in tasks:
        if task.title in seen:
            # duplicated
        seen[task.title] = task
```

**When to Stop**: Optimizing is only worthwhile if **time saved × frequency** > 1min/day.

📘 **Details**: See `PROTOCOLO_SIMPLICIDADE_2.md` - Step 10.5

---

### 🔟.6️⃣ **CI/CD Quality Gates** ⭐ [MANDATORY]

> **CRITICAL FOR PRODUCTION**: This step is **MANDATORY** in Simplicity 3.

**Why mandatory**:
- ✅ **Memory fails**: You forget to run tests manually
- ✅ **24/7 Automation**: CI validates **every** commit automatically
- ✅ **Confidence**: You know broken code won't go to production
- ✅ **Fast**: Feedback in minutes (not hours debugging)

**Pre-commit Hooks** (local validation):

```yaml
# .pre-commit-config.yaml
repos:
  - repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v4.5.0
    hooks:
      - id: trailing-whitespace
      - id: check-yaml
      - id: check-data
  
  - repo: https://github.com/psf/black
    rev: 23.12.1
    hooks:
      - id: black
  
  - repo: https://github.com/pycqa/flake8
    rev: 7.0.0
    hooks:
      - id: flake8
        args: ['--max-line-length=88']
  
  - repo: local
    hooks:
      - id: pytest
        name: pytest
        entry: pytest
        language: system
        args: ['tests/', '-v']
```

```bash
# Install
pip install pre-commit
pre-commit install

# Now every `git commit` executes validations automatically
# If it fails, commit is BLOCKED until corrected
```

**GitHub Actions** (CI pipeline):

```yaml
# .github/workflows/ci.yml
name: CI Quality Gates

on: [push, pull_request]

jobs:
  quality:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v4
    
    - name: Set up Python
      uses: actions/setup-python@v5
      with:
        python-version: '3.11'
    
    - name: Install deps
      run: |
        pip install -r requirements.txt
        pip install pytest pytest-cov flake8 black bandit
    
    - name: Black formatting
      run: black --check .
    
    - name: Flake8 linting
      run: flake8 . --max-line-length=88
    
    - name: Bandit security
      run: bandit -r . -ll
    
    - name: Tests + Coverage
      run: |
        pytest --cov=. --cov-report=term
        coverage report --fail-under=80
      # Fails if coverage < 80%
```

**GitLab CI**:

```yaml
# .gitlab-ci.yml
stages:
  - test

test:
  image: python:3.11
  script:
    - pip install -r requirements.txt pytest pytest-cov
    - pytest --cov=. --cov-report=term
    - coverage report --fail-under=80
```

**Badge in README** (visual status):

```markdown
[![CI](https://github.com/user/repo/workflows/CI/badge.svg)](https://github.com/user/repo/actions)
[![Coverage](https://codecov.io/gh/user/repo/branch/main/graph/badge.svg)](https://codecov.io/gh/user/repo)
```

**Setup Time**: ~30 minutes (once). Then automatic.

📘 **Complete configurations**: See `PROTOCOLO_SIMPLICIDADE_2.md` - Step 10.6

---

### 1️⃣1️⃣ **Organize Project Root Folder**
- ✅ Imports validated (module loads without errors)
- 📝 **Documented limitation**: GUI tests require unconﬁgured headless environment

---

#### 🔬 **Step 9.2 - Tests in Threads/Processes with Monitoring (ADVANCED)**

**Objective**: Full control over test execution with the possibility to **interrupt**, **monitor**, and **log** progress in real-time.

**When to Use**:
- GUI tests that may freeze
- Long-duration tests (>1 min)
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
    print(f"📊 Active monitoring. Press Ctrl+C to cancel.\n")
    
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

**Practical Use**:

```bash
# 1. Create monitored runner
cat > tests/run_tests_monitored.py << 'EOF'
# [code above]
EOF

# 2. Execute with monitoring
python tests/run_tests_monitored.py

# 3. Cancel at any time (Ctrl+C)
# The process will be gracefully terminated
```

**Advantages**:
- ✅ **Full control**: Can cancel tests at any time
- ✅ **Real-time logging**: See progress of each test
- ✅ **Global + individual timeout**: Double protection
- ✅ **Statistics**: Pass/fail in real-time
- ✅ **Isolation**: Tests run in a separate process (don't freeze the terminal)
- ✅ **Guaranteed cleanup**: `terminate()` + forced `kill()` if necessary

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
[ ] Define individual test timeout (default: 30s)
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

### 1️⃣1️⃣ **Organize Project Root Folder**
- **CRITICAL**: Before documentation, **organize the root folder**
- Remove temporary files, unnecessary backups
- Verify that all files are in their correct places
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

**Why?**: Keep repository clean, avoid committing junk, facilitate navigation, professionalism. Document the **clean** state of the project.

---

### 1️⃣1️⃣.5️⃣ **Decision Notes** [OPTIONAL]

**When to Use**: An important/non-obvious decision was made and you might forget the "why" later.

**What to document**:
- ✅ Choice of important library/framework
- ✅ Significant trade-off (performance vs simplicity)
- ✅ Decision NOT to do something (with rationale)
- ✅ Chosen architecture/pattern

**Simplified Format** (ADR light):

```markdown
# Decision: Use PyQt6 instead of Tkinter

**Date**: 2025-01-15
**Status**: ✅ Accepted

**Context**: Need GUI with professional dock widgets.

**Decision**: Chosen PyQt6.

**Why**:
- ✅ Native QDockWidget (Tkinter doesn't have)
- ✅ Styling with QSS (CSS-like)
- ✅ Excellent documentation

**Trade-offs**:
- ❌ GPL license (OK, project is open-source)
- ❌ Larger binary (~50MB vs ~5MB Tkinter)

**If it changes in the future**: Consider PySide6 (LGPL) if permissive license is needed.
```

**Where to store**:
```
docs/
├── decisions/
│   ├── 001-pyqt6-choice.md
│   ├── 002-data-storage.md
│   └── README.md
```

**When NOT to document**:
- ❌ Trivial decisions (naming, formatting)
- ❌ Obvious/conventional choices
- ❌ Self-explanatory code

**Time**: 5-10 minutes per important decision.

📘 **Formal ADR with template**: See `PROTOCOLO_SIMPLICIDADE_2.md` - Step 11.5

---

### 1️⃣2️⃣ **Fill New Documentation**
- **Update tasks/requirements file**: Mark tasks as `[X]` complete
- **Create SPECIFICATIONS.md**: Detailed document for the version
- **Update statistics**: Project completion percentage

**📋 Task Marking in Requirements File**:

**General Rule**:
- If a tasks/requirements file exists (e.g., `REQUIREMENTS.md`, `TODO.md`, `requirements.md`):
  - ✅ **Mark tasks as complete** after implementation: `[ ]` → `[X]`
  - ✅ **Update statistics** (percentages, counters)
  - ✅ **Add completion notes** (date, version, brief description)
  
- If a tasks/requirements file **DOES NOT exist**:
  - ❓ **Ask the user** for the file location/path
  - ❓ **Ask about next tasks and requirements** if no formal document
  - ❓ **Suggest creating** a task control file

**📁 TASKS.md File Location**:
- **Default preference**: The `TASKS.md` file, when created, should be placed in `docs/TASKS.md`
- **Create docs/ folder**: If the `docs/` folder does not exist in the project, it should be created automatically
- **Flexibility**: The user or programmer can choose to place it in another location if preferred
- **Creation example**:
  ```bash
  # Create docs folder if it doesn't exist
  mkdir -p docs
  
  # Create or update TASKS.md
  echo "# Tasks" > docs/TASKS.md
  ```

**Example of Marking (REQUIREMENTS.md)**:
```markdown
## 🟢 COULD HAVE (Low Priority)

### ✅ Completed Tasks

#### Task Example - Integrated File Editor (vX.Y.Z)
**Status**: ✅ Complete - 30/11/2025

**Objective**: Implement integrated text editor with scope differentiation by colors.

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

**Date**: DD/MM/YYYY
**Sprint**: X tasks in Y hours
**Methodology**: Simplicity 1 Protocol

## 📋 Sprint Objectives
- Task #X: [description]
- Task #Y: [description]

## 🎯 Implemented Tasks
### Task #X: [Name]
- **Problem**: [description of original problem]
- **Solution**: [how it was solved]
- **Modified Files**: [list]
- **Tests**: [quantity and status]

## ✅ Quality (Simplicity 1 Protocol)
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

### 1️⃣2️⃣.5️⃣ **Rollback Plans** ⭐ [MANDATORY]

> **CRITICAL FOR PRODUCTION**: This step is **MANDATORY** in Simplicity 3.

**Why mandatory**:
- ✅ **Production**: Bugs affect real users
- ✅ **Solo**: You are alone to resolve emergencies
- ✅ **Downtime**: Fast rollback minimizes impact
- ✅ **Confidence**: Deploy boldly knowing you can revert

**When to create a Rollback Plan**:
- ✅ Critical feature (payment, authentication, data)
- ✅ Change in data schema/migrations
- ✅ Public API alteration
- ✅ High-risk deployment

**Simplified Template**:

```markdown
# Rollback Plan - Task #XX: [Feature Name]

## Criteria for Rollback
Execute rollback IF:
- [ ] Error rate > 5% within 1h after deployment
- [ ] Users report data loss
- [ ] Frequent crashes (>5 reports)
- [ ] Performance worse than previous version (>2x slower)

## How to Revert (Step-by-Step)

### 1. Preparation (5min)
```bash
# Backup current state
cp data.db data.db.backup-$(date +%s)
cp app.log rollback-logs.txt
```

### 2. Code Rollback (5min)
```bash
# Revert to previous version
git checkout v1.9.5
# OR
pip install app==1.9.5 --force-reinstall
```

### 3. Restore Data (if necessary)
```bash
# Restore DATA/DB backup created during migration
cp data.data.backup data.data
```

### 4. Validate (5min)
```bash
# Smoke tests
app --version  # Should show v1.9.5
app test-basic-flow
```

## Total Rollback Time
~15-20 minutes (expected downtime)

## Backup Required
- ✅ Automatic backup created on deploy
- ✅ Git tag of previous version exists
- ❌ Does not depend on external services

## Data at Risk
- **High**: Data created after deployment (not in backup)
- **Low**: Existing data (preserved in backup)

**Mitigation**: Export new data before rollback.
```

**Alternative: Feature Flags** (better than rollback):

```python
# Disable feature remotely without redeploy
FEATURE_NEW_EXPORT = os.getenv("ENABLE_NEW_EXPORT", "false") == "true"

def export_data():
    if FEATURE_NEW_EXPORT:
        return new_export()  # New implementation
    else:
        return old_export()  # Safe fallback

# In case of problem: export ENABLE_NEW_EXPORT=false
# Users automatically revert to old version
```

**Quick Checklist**:
```markdown
- [ ] Rollback criteria defined (when to execute?)
- [ ] Rollback steps documented (how to revert?)
- [ ] Automated backup (data preserved?)
- [ ] Estimated rollback time (<30min?)
- [ ] Feature flag considered (better alternative?)
```

**Creation Time**: 10-15 minutes per critical feature.

📘 **Complete Rollback Plans**: See `PROTOCOLO_SIMPLICIDADE_2.md` - Step 12.5

---

### 1️⃣3️⃣ **Commit and Push**
- **Format**: Conventional Commits (feat/fix/docs/refactor/test)
- **Message**: Descriptive, complete, with context
- **Frequency**: 1 commit per task or logical group of changes

**Commit Message Structure**:
```
<type>: <short description> (<version>)

<ORIGINAL PROBLEM>:
- [Context of the problem]
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
- Implementation vX.Y.Z used string_similarity() (WRONG)
- Did not detect duplicate values, only name similarity
...

✅ IMPLEMENTED SOLUTION:
✅ extract_all_keys_from_obj()
   - Supports Obj AND dict types
   - Returns Dict[str, str] (path → value)
...

Closes: Task Example (vX.Y.Z)"

git push
```

---

## 🏆 Professional Quality Criteria

Every implementation must meet **100% of these criteria**:

| # | Criterion | Description | Validation |
|---|----------|-----------|-----------|
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

### Execution (Simplicity 1 Protocol)

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
- Answer: "Shorter line wins, don't touch if values differ"

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
- ✅ Separate modules (Reuse)
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
✅ **Simplicity 1 Protocol: 10/10 steps met** (v1.1 - 10 steps)
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
1. **Don't start with the hardest task**
   - ❌ "I'll do the text editor first (50h)"
   - ✅ "I'll do the tooltip preview first (30min)"

2. **Don't do everything at once**
   - ❌ "I'll implement everything in one giant function"
   - ✅ "I'll divide into 3 testable functions"

3. **Don't skip tests**
   - ❌ "I'll test manually later"
   - ✅ "I'll create 12 unit tests now"

4. **Don't make generic commits**
   - ❌ `git commit -m "updates"`
   - ✅ `git commit -m "feat: Task Example with VALUE EQUALITY (60 lines)"`

---

## 📚 References

- **REQUIREMENTS.md**: Complete list of project tasks
- **vX.Y.Z-COMPARISON.md**: First example of the protocol
- **vX.Y.Z-SPECIFICATIONS.md**: Sprint with 3 simple tasks
- **vX.Y.Z-SPECIFICATIONS.md**: Fast iterations
- **vX.Y.Z-SPECIFICATIONS.md**: 4 UX improvements
- **FEATURE_SPEC.md**: Example of detailed documentation

---

## 🔄 Continuous Cycle

Simplicity 1 Protocol is an **iterative cycle**:

```
┌──────────────────────────────────────────────┐
│  1. Read Documentation                         │
│  2. Choose Simplest Tasks                    │
│  3. Ask Questions to the Developer           │
│  4. Analyze and Study the Project             │
│  5. Plan Sprint (2-4 tasks, 3-4h)            │
│  6. Implement (GoF + GRASP architecture)    │
│  7. Verify GUI Integration                   │
│  8. Verify CLI Implementation                │
│  9. Test (100% coverage)                     │
│  10. Organize Root Folder                    │
│  11. Document (TASKS + vX.X.X-SPECS)         │
│  12. Commit + Push (conventional)            │
└──────────────────────────────────────────────┘
           ↓
    ┌──────────────┐
    │    REPEAT    │ ← There are always simpler tasks!
    └──────────────┘
```

**Result**: Constant progress, professional code, zero technical debt, **safe for production**.

---

## 🎯 Final Message

> "I want complete, professional, and **production-safe work** - developing alone!"

**Simplicity 3 ensures**:
- ✅ **Solid base**: 13 mandatory steps from Simplicity 1
- ✅ **Security**: OWASP checklist mandatory (zero vulnerabilities)
- ✅ **Automation**: CI/CD validates every commit (memory doesn't fail)
- ✅ **Protection**: Rollback plans for critical features
- ✅ **Pragmatic**: NO team overhead (code review, formal retrospectives)
- ✅ **Prioritization**: Decision matrix when necessary
- ✅ **Performance**: Profiling for slow features
- ✅ **Traceability**: Decision notes for important choices

**Simplicity 3 is ideal for**:
- 👤 **Solo developer** (you alone)
- 🚀 **Production** (real users depending)
- ⚠️ **Critical** (bugs have impact)
- 📈 **Long-term** (evolutive project >6 months)

**When to use another protocol**:
- Disposable prototype → Use **Simplicity 1**
- Team of 2+ people → Use **Simplicity 2** (has peer code review)

**Reread this document before each sprint!**

---

## 📚 Related Documents

- 📘 **PROTOCOLO_SIMPLICIDADE_1.md**: Base (13 steps) - For prototypes/internal
- 📕 **PROTOCOLO_SIMPLICIDADE_2.md**: Advanced (23 steps) - For enterprise teams
- 📗 **PROTOCOLO_SIMPLICIDADE_3.md**: Hybrid (16 steps) - **Solo dev in production** ⭐

---

**Version**: 3.0
**Last update**: December 02, 2025
**Maintained by**: Josué Amaral
**Status**: ACTIVE - Protocol for solo developer in production
