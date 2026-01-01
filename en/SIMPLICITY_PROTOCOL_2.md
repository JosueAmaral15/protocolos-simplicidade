Aqui está a tradução do seu arquivo Markdown do português para o inglês:

```markdown
# Simplicity Protocol 2

**Author**: Josué Amaral  
**Creation Date**: December 02, 2025  
**Based on**: Simplicity Protocol 1 v2.3  
**Version**: 2.5  
**Last Update**: January 1, 2026  
**Objective**: ADVANCED professional methodology for incremental quality development with a focus on security, performance, and continuous improvement

**Changelog v2.5** (01/01/2026):
- ✅ **[NEW]** Default Recommended Stack for Websites (Enterprise Focus)
- ✅ Same base: Next.js 15 + React 19 + TypeScript + Tailwind
- ✅ Mandatory enterprise validation: Technical meeting + formal ADR
- ✅ Additional analysis: Cost, corporate compliance, commercial support
- ✅ TypeScript mandatory for large teams
- ✅ Monorepo-ready with Turbo
- ✅ Enterprise use cases: Netflix, TikTok, Uber use Next.js
- ✅ When NOT to use: Mandatory corporate stack, compliance restrictions

**Changelog v2.4** (01/01/2026):
- ✅ **[CRITICAL]** Added Step 1.0: Complete Documentation Reading (PRIORITY)
- ✅ Enterprise focus: Mandatory reading of ADRs, security and compliance
- ✅ Minimum enterprise structure: ADR template, security/, api/
- ✅ README template with stakeholders and approvers
- ✅ Complete ADR (Architecture Decision Record) template
- ✅ Expanded checklist (12 items) including compliance validation
- ✅ Formal documentation mandatory for every architectural decision
- ✅ Team coordination via shared documentation
- ✅ Rationale: Documentation is evidence for auditing

**Changelog v2.3** (01/01/2026):
- ✅ **[MANDATORY]** Added Step 1.5: Technology Stack Research
- ✅ Additional enterprise validation: Technical meeting + stakeholders
- ✅ Formal ADR mandatory for tech stack decision
- ✅ Licensing cost and corporate compliance analysis
- ✅ Corporate standards verification
- ✅ Expanded checklist (13 items) including stakeholder approval
- ✅ Specific ADR template for tech stack choice
- ✅ Alignment with Simplicity 1 v2.1 (same core functionality)

**Changelog v2.2** (10/12/2025):
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
- ✅ **Step 6.7**: Generate API Documentation (Sphinx/pdoc)
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

## ⚠️ Golden Rule: Absolute Priority for Workspace Errors

> **CRITICAL FOR AIs**: Before implementing new features or continuing with tasks, **all workspace errors must be fixed BY YOU (AI)**.

### 🤖 This Rule is For AI Assistants

**If you are an AI (Cursor, GitHub Copilot, etc.):**
- ✅ **YOU MUST** fix all existing errors BEFORE implementing new features
- ✅ **YOU MUST** resolve issues proactively, not wait for humans to fix them
- ✅ **YOU MUST** treat error correction as the highest priority
- ✅ **YOU MUST** clean the workspace before adding new code

**This rule does NOT mean:**
- ❌ That human developers must stop implementing when errors exist
- ❌ That the project cannot advance while errors are present
- ❌ That humans need to manually fix the errors

### 🚨 Types of Errors That Block Development

Consider the existence of errors in the workspace (visible in the IDE's "Problems" tab) as **undesirable and blocking**. If any of the following types of errors occur, **fixing them is an absolute priority** before continuing:

1. **❌ Syntax Issues**
   - Code parsing errors
   - Unclosed parentheses, braces, or brackets
   - Incorrect indentation (Python)
   - Missing semicolons (JavaScript, C, Java)

2. **❌ Code Inconsistencies**
   - Variables declared but not used
   - Unused or missing imports
   - Dead code (unreachable code)
   - Type mismatches (TypeScript, Python with type hints)

3. **❌ Unexpected Omissions**
   - Functions declared but not implemented
   - Missing required parameters
   - Missing return statements when expected
   - Missing mandatory documentation

4. **❌ Incorrect Facts**
   - References to non-existent variables
   - Function calls with wrong number of arguments
   - Access to non-existent properties
   - Imports of non-existent modules

5. **❌ Ambiguities**
   - Type checking warnings
   - Possible null/undefined references
   - Variable shadowing
   - Dangerous implicit type conversions

6. **❌ Missing Files**
   - Dependencies not installed
   - Imported modules not found
   - Missing configuration files
   - Referenced but non-existent assets

7. **❌ Execution Failures**
   - Build failures
   - Compilation errors
   - Failing tests
   - Linter errors (when configured)

### ✅ When You Can Continue

**ONLY** continue with development of new features when:

- ✅ **Zero errors** in the workspace "Problems" tab
- ✅ **All builds** complete successfully
- ✅ **All tests** pass (if they already exist)
- ✅ **Linter/formatter** doesn't report critical errors
- ✅ **Type checker** doesn't report errors (if applicable)

### 📋 Checklist Before Each Task

```markdown
Before starting any new task:

[ ] Check IDE "Problems" tab (0 errors)
[ ] Run project build (success)
[ ] Run existing tests (all passing)
[ ] Run linter/formatter (no critical errors)
[ ] Verify imports and dependencies (all resolved)
[ ] Confirm code is in clean state (committable)
```

### ⏱️ Estimated Time for Fixing

- **Syntax Errors**: ~2-5 minutes per error
- **Imports/Dependencies**: ~5-10 minutes
- **Type Errors**: ~5-15 minutes per error
- **Failing Tests**: ~10-30 minutes (depends on complexity)

**Rule of Thumb**: If you have >10 errors in the workspace, **dedicate 1-2 hours** to clean everything before proceeding.

### 🎯 Rationale

**Why is this rule critical?**

1. **Cascade Prevention**: One uncorrected error can generate 10 new errors
2. **Code Quality**: Code with errors = immediate technical debt
3. **Reliability**: New features on top of broken code = guaranteed bugs
4. **Productivity**: Fixing old + new errors is more time-consuming than fixing only old ones
5. **Professionalism**: Clean, error-free code is a minimum requirement

**Message for AIs**: 
> "Until the errors are resolved BY YOU (AI), tasks and features cannot continue being implemented BY YOU (AI). Fix the errors first, then continue with implementation."

---

## 🔍 Binary Search for Bug Localization

> **IMPORTANT FOR AIs**: When dealing with error correction and bug elimination, remember that you can use **binary search** to locate defects efficiently.

### 🎯 Core Concept

Binary search is a powerful technique that reduces the search space by half with each iteration, allowing you to locate defects in **O(log N) steps**, where N is the number of lines, commands, or instructions in the algorithm.

**Practical Example**: 
- If an error is on line 48 of a file with 512 lines
- Linear search: up to 512 checks
- Binary search: only **9 checks** (log₂(512) = 9)

### 📋 Binary Search Debugging Methodology

#### **1️⃣ Initial Step: Divide Code in Half**

Starting with a file of N lines where an error exists:
1. Comment out half of the code (e.g., lines 257-512)
2. Execute/test the remaining half (lines 1-256)
3. Check if the error persists

**Decision**:
- ✅ **Error persists**: The bug is in the active half (1-256)
- ❌ **Error disappears**: The bug is in the commented half (257-512)

#### **2️⃣ Recursion: Keep Dividing**

Once you've identified the half with the problem, repeat the process:

**Iteration 2** (error in 1-256):
- Comment out lines 129-256
- Test lines 1-128
- Identify which quarter contains the bug

**Iteration 3** (error in 1-128):
- Comment out lines 65-128
- Test lines 1-64
- Identify which eighth contains the bug

**Continue until** you locate exactly the problematic line/block.

#### **3️⃣ Complete Example: 512 Lines → Line 48**

```
Iteration 1: [1-512]   → Test [1-256]   ✅ Error present
Iteration 2: [1-256]   → Test [1-128]   ✅ Error present  
Iteration 3: [1-128]   → Test [1-64]    ✅ Error present
Iteration 4: [1-64]    → Test [1-32]    ❌ Error absent → Bug in [33-64]
Iteration 5: [33-64]   → Test [33-48]   ✅ Error present
Iteration 6: [33-48]   → Test [33-40]   ✅ Error present
Iteration 7: [41-48]   → Test [41-44]   ✅ Error present
Iteration 8: [45-48]   → Test [45-46]   ✅ Error present
Iteration 9: [47-48]   → Test [line 47]  ❌ Error absent → ✅ Bug on line 48!
```

**Result**: 9 iterations to find the bug in 512 lines (vs. up to 512 linear attempts).

### 🛠️ Implementation Techniques

#### **A) Temporary Comments**
```python
# BINARY SEARCH - Iteration 1: Testing [1-256]
# Lines 257-512 temporarily disabled
# def suspicious_function():  
#     potentially_buggy_code()
#     more_code()
```

#### **B) Debug Flags**
```python
DEBUG_BINARY_SEARCH = True
RANGE_START = 1
RANGE_END = 256

if DEBUG_BINARY_SEARCH and not (RANGE_START <= current_line <= RANGE_END):
    return  # Skip execution outside test range
```

#### **C) Git Bisect** (for bugs introduced in commits)
```bash
# Use git bisect to find the commit that introduced the bug
git bisect start
git bisect bad HEAD              # Current commit has bug
git bisect good v1.0.0           # Commit v1.0.0 didn't have bug
# Git automatically performs binary search on commits
```

#### **D) Partitioned Unit Tests**
```python
# Split test suite in half
pytest tests/test_module_part1.py  # First half
pytest tests/test_module_part2.py  # Second half
# Identify which half contains failing test
```

### 🎨 Creative Applications of Binary Search

Binary search is not limited to lines of code. It can be applied to:

1. **📦 Dependencies/Imports**:
   - Comment out half of the imports
   - Identify which import causes conflict/error
   
2. **🔧 Configuration Parameters**:
   - Disable half of the configurations
   - Find problematic configuration

3. **🗃️ Input Data**:
   - Process half of the dataset
   - Identify which subset causes error

4. **⚙️ Features/Functionality**:
   - Disable half of the features
   - Locate feature causing regression

5. **🧩 Modules/Components**:
   - Disable half of the modules
   - Find module with bug

6. **📅 Version History** (Git Bisect):
   - Test version in middle of history
   - Find commit that introduced bug

7. **🔄 Loop Iterations**:
   - Execute half of the iterations
   - Identify in which iteration error occurs

### ✅ Binary Search Debugging Checklist

```markdown
[ ] 1. Confirm error is consistently reproducible
[ ] 2. Identify total scope (N lines/modules/commits)
[ ] 3. Calculate required iterations: log₂(N)
[ ] 4. Create backup or test branch
[ ] 5. Iteration 1: Comment/disable upper/lower half
[ ] 6. Run test and check if error persists
[ ] 7. Record result and reduce scope by half
[ ] 8. Repeat until isolating exact line/block/commit
[ ] 9. Analyze isolated code to understand root cause
[ ] 10. Apply fix and validate with tests
[ ] 11. Remove debug code/temporary comments
```

### 🎯 When to Use Binary Search for Debugging

**✅ Use when:**
- Error is reproducible but cause is not obvious
- Large codebase (>100 lines)
- Suspect bug is in specific but broad region
- Error appeared after large changes (multiple commits)
- Test fails but there's no clear indication of problem
- Performance degraded but don't know which function is responsible

**❌ Don't use when:**
- Error is sporadic/non-reproducible (race condition, timing issue)
- Stack trace already points to exact line of problem
- Code is very small (<50 lines)
- Bug is obvious after quick code review

### ⏱️ Binary Search Efficiency

| Size (N) | Linear Search | Binary Search | Gain |
|----------|--------------|---------------|------|
| 32 lines  | up to 32 steps | 5 steps | 6.4x faster |
| 128 lines | up to 128 steps | 7 steps | 18.3x faster |
| 512 lines | up to 512 steps | 9 steps | 56.9x faster |
| 1024 lines | up to 1024 steps | 10 steps | 102.4x faster |
| 4096 lines | up to 4096 steps | 12 steps | 341.3x faster |

### 💡 Practical Tips

1. **Document the Process**: Record each iteration and result
2. **Use Version Control**: Create branches for each test
3. **Automate When Possible**: Scripts to comment/uncomment blocks
4. **Combine with Logs**: Add prints to confirm block execution
5. **Test Independently**: Ensure the test is deterministic
6. **Validate Before and After**: Confirm bug exists before and is fixed after

### 🚀 Rationale

**Why is binary search powerful for debugging?**

1. **⚡ Algorithmic Efficiency**: O(log N) vs O(N) - exponential time savings
2. **🎯 Precise Isolation**: Reduces uncertainty systematically
3. **🧠 Lower Cognitive Load**: Simple decisions (error present: yes/no)
4. **📊 Predictability**: Know exactly how many steps will be needed
5. **🔄 Universal Applicability**: Works for code, data, configurations, history
6. **✅ Success Guarantee**: If the bug is reproducible, binary search always finds it

**Message for AIs**:
> "Creativity in using binary search has no limits. Always consider whether a debugging problem can be reduced to a binary search - you'll save time and find bugs faster."

---

## 🧠 Associative Memory Factor

> **IMPORTANT FOR AIs**: During error investigation and correction, apply the **Associative Memory Factor** to learn from past patterns and accelerate future diagnostics.

### 🎯 What is Associative Memory?

**Associative Memory** is AI's ability to:
- 🧠 **Recognize patterns** recurring in errors and defects
- 🔗 **Associate causes and effects** in different contexts
- 📈 **Generalize solutions** from specific cases
- 📉 **Deduce problems** from general to specific (top-down)
- 📊 **Induce rules** from specific to general (bottom-up)

### 🐍 Connection with Python Traceback

Traceback presents errors in **top-down** structure:
```
main.py (ROOT/Orchestrator)
  ↓
processor.py (BRANCH/Coordinator)
  ↓
validator.py (LEAF/Executor) ← Error here!
```

**Associative Insight**:
- Errors in **leaves** → violated preconditions
- Errors in **branches** → incorrect coordination logic
- Errors in **root** → problematic integration

### 🔬 Complementary Approaches

**Deductive (General → Specific)**:
- Apply known general rules to diagnose
- Ex: "AttributeError usually indicates uninitialized object"

**Inductive (Specific → General)**:
- Observe repeated cases to create general rule
- Ex: "70% of IndexError are from incorrect index manipulation"

**Neuro-Symbolic (Combination)**:
- Unites deduction (symbolic AI) with induction (neural AI)
- Learns continuously while applying rules

### 🐛 Defect Taxonomy

Five categories of highly undesirable defects:

1. **Incorrect Fact**: Wrong or outdated information
2. **Extraneous Information**: Code/comments that don't belong to context
3. **Ambiguity**: Code with multiple possible interpretations
4. **Inconsistency**: Violation of established patterns
5. **Omission**: Missing code or logic (validations, error handling)

### 🔄 Error Patterns

**Input-Independent Errors**:
- Always occur, regardless of data
- Problem in **logic**, not in **data**

**Specific Scope Errors**:
- One bug, multiple symptoms in different parts
- Look for **shared dependency**

**Common Import Errors**:
- Multiple modules fail because they import buggy code
- Fix once resolves all cases

### 🤝 Application in Code Review (Protocol 2)

During code reviews, beyond individual review, apply associative memory:

**Defect Taxonomy Checklist**:
- [ ] **Incorrect Fact**: Outdated values, constants, or comments
- [ ] **Extraneous Information**: Commented code, obsolete TODOs, unused imports
- [ ] **Ambiguity**: Vague names, incomplete documentation
- [ ] **Inconsistency**: Violation of naming conventions or patterns
- [ ] **Omission**: Missing validations, exception handling, or edge cases

**Team Knowledge Base**:
- Maintain record of common error patterns in the team
- Share effective solutions in documentation
- Conduct retrospectives on recurring defects
- Create prevention guides based on accumulated experience

### ✅ Application Checklist

When investigating and fixing errors:

**Analysis Phase**:
- [ ] Examine Traceback from top to bottom (root → leaf)
- [ ] Identify error level (orchestrator/coordinator/executor)
- [ ] Consult knowledge base for similar patterns
- [ ] Apply deduction: general rules → specific hypothesis
- [ ] Search induction: multiple cases → general pattern

**Correction Phase**:
- [ ] Validate absence of Incorrect Fact
- [ ] Remove Extraneous Information
- [ ] Eliminate Ambiguities
- [ ] Ensure Consistency with project patterns
- [ ] Fix Omissions (validations, error handling)

**Learning Phase**:
- [ ] Add case to knowledge base
- [ ] Update general rules if new pattern identified
- [ ] Document solution for future reference
- [ ] Share learning with the team
- [ ] Reinforce associations of confirmed patterns

### 📖 Complete Documentation

For a comprehensive understanding of the Associative Memory Factor, see the complete section integrated in this protocol below.

---

## 📋 Associative Memory Factor - Complete Documentation

### 🎯 Overview

The **Associative Memory Factor** is a fundamental concept that integrates the Simplicity Protocols, allowing artificial intelligence to learn from past error patterns and apply that knowledge in investigating and correcting future defects.

#### 🔍 What is Associative Memory?

Associative memory is the ability to:
- ✅ **Recognize patterns** recurring in errors and defects
- ✅ **Associate causes and effects** specific to different contexts
- ✅ **Generalize solutions** from specific cases
- ✅ **Deduce problems** from general to specific
- ✅ **Induce rules** from specific to general

#### 🎯 Objective

Enable AI to develop a "memory" of problems and solutions, creating associations between:
- Error types and their root causes
- Observed symptoms and accurate diagnoses
- Project contexts and defect patterns
- Applied solutions and their effectiveness

---

### 🐍 Connection with Python Traceback

#### 📊 How Traceback Works

Python's Traceback presents errors in a **top-down** structure (from outside to inside):

```python
Traceback (most recent call last):
  File "main.py", line 10, in <module>          # ← ROOT (Orchestrator)
    processar_dados()
  File "processador.py", line 45, in processar_dados  # ← BRANCH (Coordinator)
    validar_entrada(dados)
  File "validador.py", line 23, in validar_entrada    # ← LEAF (Executor)
    assert len(dados) > 0                             # ← SPECIFIC ERROR
AssertionError: empty list
```

#### 🎯 Top-Down Investigation Methodology

**Level 1: Orchestrator (main.py)**
- Where was the error **triggered**?
- What is the **execution context**?
- What **data** was passed?

**Level 2: Coordinator (processador.py)**
- How was the data **transformed**?
- What **business logic** was applied?
- Were there **intermediate validations**?

**Level 3: Executor (validador.py)**
- Which **specific operation** failed?
- Which **precondition** was violated?
- What is the technical **root cause**?

#### 🧠 Memory Association

AI should **remember** and **associate**:
- **Observed pattern**: `AssertionError` in input validation
- **Common cause**: Empty data not handled at upper level
- **Typical solution**: Add check before calling `validar_entrada()`
- **Future prevention**: Always validate non-empty list before processing

#### 🔄 Analogy with Import Tree

The Traceback structure mirrors the Import Tree concept:

```
main.py (ROOT)
  └─ processador.py (BRANCH)
       └─ validador.py (LEAF) ← Error here!
```

**Associative Memory Insight**:
- Errors in **leaves** usually indicate **violated preconditions**
- Errors in **branches** usually indicate **incorrect coordination logic**
- Errors in **root** usually indicate **problematic integration or orchestration**

---

### 🔬 Deductive and Inductive Approaches

#### 📉 Deductive Approach (General → Specific)

**Concept**: Start from a general rule to identify specific cases.

**Practical Example**:

**General Rule**: "AttributeError usually indicates that an object was not initialized correctly"

**Specific Application**:
```python
# Observed error
AttributeError: 'NoneType' object has no attribute 'process'

# Deduction:
1. ✅ General rule: AttributeError → object not initialized
2. ✅ Hypothesis: variable returned None instead of object
3. ✅ Investigation: check methods that return the object
4. ✅ Solution: add None check or fix initialization
```

**Deductive Flow**:
```
General Theory (prior knowledge)
         ↓
Specific Hypothesis (based on error)
         ↓
Test Hypothesis (debugging)
         ↓
Confirmation/Refutation
```

#### 📈 Inductive Approach (Specific → General)

**Concept**: Observe repeated specific cases to create a general rule.

**Practical Example**:

**Observation 1**:
```python
# Project A
IndexError: list index out of range
# Cause: loop using range(len(lista) + 1)
```

**Observation 2**:
```python
# Project B  
IndexError: list index out of range
# Cause: accessing lista[i] without checking len(lista)
```

**Observation 3**:
```python
# Project C
IndexError: list index out of range
# Cause: manual iteration with incorrectly incremented index
```

**Induction (General Rule)**:
> "70% of `IndexError` are caused by incorrect manual index manipulation.  
> **Preventive solution**: Always prefer iterators (`for item in lista`) instead of manual indices."

**Inductive Flow**:
```
Specific Case 1
      +
Specific Case 2
      +
Specific Case 3
      ↓
Identified Pattern
      ↓
General Rule (new associative memory)
      ↓
Preventive Application in Future Projects
```

#### 🔄 Deductive-Inductive Combination (Neuro-Symbolic)

**Complete Learning Cycle**:

1. **Deductive**: Apply existing general rules to diagnose current error
2. **Validation**: Confirm or refute deductive hypothesis
3. **Inductive**: If new pattern is observed, add to knowledge base
4. **Refinement**: Update general rules with new specific cases

**Cycle Example**:
```
[Deductive] Rule: "TypeError usually indicates incompatible type"
           ↓
[Application] Error: TypeError when adding string + int
           ↓
[Validation] ✅ Confirmed: attempt at incompatible sum
           ↓
[Inductive] New pattern: "TypeError with '+' → check types before operation"
           ↓
[Memory] Store: "Always validate types before mathematical operations"
```

---

### 🐛 Software Defect Taxonomy

The software defect taxonomy identifies five main categories of highly undesirable and unexpected problems:

#### 1️⃣ Incorrect Fact

**Definition**: Information in code that is wrong or outdated.

**Examples**:
```python
# ❌ Incorrect fact
PI = 3.14  # Imprecise value

# ✅ Correction
PI = 3.14159265359  # Correct value with adequate precision
```

```python
# ❌ Incorrect fact  
MAX_UPLOAD_SIZE = 5 * 1024  # Comment says "5MB" but code is 5KB

# ✅ Correction
MAX_UPLOAD_SIZE = 5 * 1024 * 1024  # 5MB correct
```

**Associative Memory**:
- Always validate **numeric constants** against requirements
- Review **comments** to ensure alignment with code
- Use **boundary tests** for critical values

#### 2️⃣ Extraneous Information

**Definition**: Code, comments, or logic that doesn't belong to the current context.

**Examples**:
```python
# ❌ Extraneous information
def calcular_preco(valor):
    # TODO: implement VIP customer discount
    # print("DEBUG: valor =", valor)  # Forgotten debug code
    # import random  # Unused import
    resultado = valor * 1.1
    return resultado
```

```python
# ✅ Correction
def calcular_preco(valor):
    """Calculate price with 10% fee."""
    resultado = valor * 1.1
    return resultado
```

**Associative Memory**:
- Remove **unused commented code**
- Eliminate **unnecessary imports** (use linter)
- Clean **completed TODOs** or move them to task system

#### 3️⃣ Ambiguity

**Definition**: Code or documentation that can be interpreted in multiple ways.

**Examples**:
```python
# ❌ Ambiguous
def processar(dados):
    """Process the data."""  # What does "process" mean?
    return dados
```

```python
# ✅ Specific
def normalizar_e_validar_entrada_usuario(dados_brutos):
    """
    Normalize user input (lowercase, trim) and validate email format.
    
    Args:
        dados_brutos: String with email provided by user
        
    Returns:
        String with normalized and validated email
        
    Raises:
        ValueError: If email format is invalid
    """
    email_normalizado = dados_brutos.strip().lower()
    if "@" not in email_normalizado:
        raise ValueError("Invalid email: missing '@'")
    return email_normalizado
```

**Associative Memory**:
- Use **descriptive names** that explain intention
- Add **detailed docstrings** with Args/Returns/Raises
- Include **usage examples** in documentation
- Prefer **specificity** over brevity

#### 4️⃣ Inconsistency

**Definition**: Violation of established patterns or conventions in the project.

**Examples**:
```python
# ❌ Inconsistent
def calcular_total(preco):  # snake_case
    return preco * 1.1

def CalcularDesconto(preco):  # PascalCase - INCONSISTENT!
    return preco * 0.9

def calcPreco(valor):  # camelCase - INCONSISTENT!
    return valor
```

```python
# ✅ Consistent
def calcular_total(preco):  # snake_case
    return preco * 1.1

def calcular_desconto(preco):  # snake_case
    return preco * 0.9

def calcular_preco_final(valor):  # snake_case
    return valor
```

**More Inconsistency Examples**:
```python
# ❌ Inconsistent parameter order
def enviar_email(destinatario, assunto, corpo): pass
def enviar_sms(corpo, numero): pass  # Different order!

# ✅ Consistent order
def enviar_email(destinatario, assunto, corpo): pass
def enviar_sms(destinatario, corpo): pass
```

**Associative Memory**:
- Establish **style guide** at project start
- Use **linters** (pylint, flake8) to enforce standards
- Maintain **naming consistency** (snake_case for Python)
- Follow **consistent parameter order** in similar functions
- Apply **uniform return patterns** (always return type, never mix None with values)

#### 5️⃣ Omission

**Definition**: Missing code or logic that should exist.

**Examples**:
```python
# ❌ Omission: missing input validation
def dividir(a, b):
    return a / b  # ZeroDivisionError if b == 0!
```

```python
# ✅ With validation
def dividir(a, b):
    if b == 0:
        raise ValueError("Divisor cannot be zero")
    return a / b
```

```python
# ❌ Omission: missing exception handling
dados = baixar_dados_api()  # Can fail due to network!
processar(dados)
```

```python
# ✅ With handling
try:
    dados = baixar_dados_api()
except RequestException as e:
    logger.error(f"Failed to download data: {e}")
    dados = carregar_dados_cache()
processar(dados)
```

**Associative Memory**:
- Always add **precondition validation**
- Implement **exception handling** for operations that can fail
- Include **edge case tests** to detect omissions
- Add **logging** in critical operations
- Document **known limitations** if something cannot be implemented

#### 🎯 Impact on Development

These five defect types are **highly undesirable and unexpected** because:

❌ **Don't contribute** to meeting developer's requirements  
❌ **Don't satisfy** direct client's needs  
❌ **Don't add value** for client's clients (end users)  
❌ **Introduce risks** of bugs in production  
❌ **Reduce reliability** of the system  
❌ **Increase costs** of maintenance and support

✅ **Protocols Objective**: **Systematically eliminate** these five defects through rigorous validation, review, and testing processes.

---

### 🔄 Error Patterns and Associative Memory

#### 🎯 Input-Independent Errors

**Concept**: Errors that occur **always**, regardless of provided data.

**Example**:
```python
# ❌ Always present error
def processar_lista(items):
    resultado = []
    for i in range(len(items) + 1):  # BUG: always causes IndexError
        resultado.append(items[i])
    return resultado
```

**Characteristics**:
- ✅ Reproducible in **100% of cases**
- ✅ Doesn't depend on **specific data**
- ✅ Indicates **structural** error in logic
- ✅ Easier to **diagnose and fix**

**Associative Memory**:
> "If error occurs in all tests with different data, the problem is in the **logic** and not in the **data**."

#### 🎯 Specific Scope Errors

**Concept**: Errors confined to a specific module, function, or file.

**Example**:
```python
# Module: validador.py
def validar_cpf(cpf):
    # BUG: incorrect validation here
    return len(cpf) == 11  # Over-simplification!

# Multiple places using validador.py:
# - cadastro.py: validation failure
# - login.py: validation failure  
# - perfil.py: validation failure
```

**Characteristics**:
- ✅ **Single location** with bug
- ✅ **Multiple symptoms** in different parts of system
- ✅ Fix **once** resolves **all cases**

**Associative Memory**:
> "If multiple components show same error, look for **shared dependency** (common import)."

#### 🎯 Errors from Importing Buggy Code

**Concept**: Different algorithms fail because they import the same defective module.

**Example**:
```python
# utils.py (BUGGY CODE)
def formatar_data(data):
    return data.strftime("%d/%m/%Y")  # BUG: fails if data = None

# modulo_a.py
from utils import formatar_data
resultado_a = formatar_data(data_a)  # ❌ Fails

# modulo_b.py  
from utils import formatar_data
resultado_b = formatar_data(data_b)  # ❌ Fails

# modulo_c.py
from utils import formatar_data  
resultado_c = formatar_data(data_c)  # ❌ Fails
```

**Investigation with Associative Memory**:

1. **Observation**: 3 different modules fail with same `AttributeError`
2. **Pattern**: All import `utils.formatar_data`
3. **Hypothesis**: Bug is in `utils.py`, not in modules using it
4. **Validation**: Test `formatar_data` in isolation
5. **Correction**: Fix in `utils.py` once
6. **Verification**: All 3 modules work again

**Associative Memory**:
> "Identical error pattern in different modules → investigate **shared dependencies** first."

#### 📊 Pattern Knowledge Base

AI should build and maintain an **associative knowledge base**:

| Error Pattern | Probable Cause | Investigation Strategy | Typical Solution |
|---------------|----------------|------------------------|------------------|
| `AttributeError: 'NoneType'` | Uninitialized variable | Track None returns | Add check or fix initialization |
| `IndexError: list index out of range` | Loop with incorrect indices | Check ranges and len() | Use iterators instead of indices |
| `KeyError` | Key doesn't exist in dict | Check dict population | Use dict.get() or validate key exists |
| `TypeError: unsupported operand` | Incompatible types | Check variable types | Add conversion or type validation |
| `RecursionError: maximum recursion depth` | Recursion without base case | Analyze stop condition | Add/fix base case |
| `ImportError` / `ModuleNotFoundError` | Missing dependency | Check requirements | Install dependency |

**Continuous Update**:
- ✅ For each resolved error, **add** to knowledge base
- ✅ For each confirmed pattern, **reinforce** association
- ✅ For each false positive, **refine** diagnostic rule

---

### 🧠 Integration with Neuro-Symbolic Artificial Intelligence

#### 🎯 What is Neuro-Symbolic AI?

**Symbolic AI** (Deductive):
- Based on **explicit rules** and **formal logic**
- Example: "If error == 'AttributeError' then check initialization"

**Neural AI** (Inductive):
- Based on **pattern learning** from data
- Example: Neural network trained to recognize error types by symptoms

**Neuro-Symbolic AI** (Combination):
- **Combines** explicit rules with pattern learning
- **Unites** deduction (top-down) with induction (bottom-up)
- **Allows** transparent reasoning and continuous adaptation

#### 🔄 Analogy with HDC (Hyperdimensional Computing)

The problem statement mentions HDC as a reference for uniting concepts:

**HDC**: Represents concepts as high-dimensional vectors, allowing:
- ✅ Association between similar concepts
- ✅ Composition of complex concepts
- ✅ Memory retrieval by similarity

**Application in Debugging**:
```
Vector(Error) = Vector(Type) + Vector(Context) + Vector(Stacktrace)

Similarity(Current_Error, Historical_Error) → Retrieve Solution
```

#### 🎯 Neuro-Symbolic Debugging Cycle

```
1. [Symbolic] Apply known general rules (deduction)
                      ↓
2. [Neural] Search similar patterns in history (association)
                      ↓
3. [Symbolic] Formulate specific hypothesis (diagnosis)
                      ↓
4. [Neural] Validate hypothesis with tests (induction)
                      ↓
5. [Symbolic] Apply correction based on rule
                      ↓
6. [Neural] Learn new pattern and update base
```

#### 📊 Complete Practical Example

**Situation**: Unexpected error when processing file upload

**Phase 1 - Deduction (Symbolic)**:
```
Traceback shows: ValueError in parse_csv()
General rule: "ValueError usually indicates incorrect data format"
Hypothesis: CSV file is malformed
```

**Phase 2 - Association (Neural)**:
```
Search in history: similar errors with CSV
Pattern found: 3 previous cases with UTF-8/Latin1 encoding
Association: "ValueError in CSV → encoding problem"
```

**Phase 3 - Diagnosis (Symbolic)**:
```
Refined hypothesis: CSV file uses Latin1 encoding but code assumes UTF-8
Test: Try opening with encoding='latin1'
```

**Phase 4 - Validation (Neural)**:
```
Test confirms: file opens with Latin1
Induction: "Confirmed pattern - CSV files from legacy system use Latin1"
```

**Phase 5 - Correction (Symbolic)**:
```python
# Before (buggy)
with open(arquivo, 'r') as f:
    dados = csv.reader(f)

# After (fixed)
with open(arquivo, 'r', encoding='latin1') as f:
    dados = csv.reader(f)
```

**Phase 6 - Learning (Neural)**:
```
Add to knowledge base:
"CSV + ValueError + parse error → try encoding='latin1'"
Reinforce pattern: 4 confirmed cases
Create preventive rule: Always specify encoding explicitly
```

---

### ✅ Usage Checklist

#### 🎯 For Artificial Intelligences

When investigating and fixing errors, AI should:

**Analysis Phase**:
- [ ] Examine Traceback from top to bottom (root → leaf)
- [ ] Identify error level (orchestrator/coordinator/executor)
- [ ] Consult knowledge base for similar patterns
- [ ] Apply deduction: general rules → specific hypothesis
- [ ] Search induction: multiple cases → general pattern

**Investigation Phase**:
- [ ] Check if error is input-independent
- [ ] Identify specific scope of problem
- [ ] Look for shared code (common imports)
- [ ] Apply binary search if necessary
- [ ] Use git bisect for regressions

**Correction Phase**:
- [ ] Validate absence of Incorrect Fact
- [ ] Remove Extraneous Information
- [ ] Eliminate Ambiguities
- [ ] Ensure Consistency with project patterns
- [ ] Fix Omissions (validations, error handling)

**Learning Phase**:
- [ ] Add case to knowledge base
- [ ] Update general rules if new pattern identified
- [ ] Document solution for future reference
- [ ] Reinforce associations of confirmed patterns

#### 📊 Success Metrics

**Good Associative Memory Indicators**:
- ✅ **Reduced diagnostic time** (less time to identify cause)
- ✅ **Increased correction rate** (more errors fixed on first attempt)
- ✅ **Effective prevention** (fewer recurring errors)
- ✅ **Growing knowledge base** (more documented patterns)
- ✅ **Consistent application** (standardized solutions)

---

### 🎓 Conclusion

The **Associative Memory Factor** transforms the debugging approach from reactive to proactive:

- 🧠 **Learns** from past errors
- 🔍 **Recognizes** recurring patterns
- 🎯 **Applies** validated solutions
- 📈 **Evolves** continuously
- 🚀 **Prevents** future problems

The integration of **deductive** (top-down) and **inductive** (bottom-up) approaches, combined with systematic analysis of **defect taxonomy**, creates a neuro-symbolic AI capable of:

✅ Diagnosing errors more quickly  
✅ Applying more effective solutions  
✅ Preventing recurring problems  
✅ Continuously improving its knowledge base  
✅ Better serving developer and client requirements

---

## 🌐 Code Language: Variable Naming and Comments

> **IMPORTANT FOR AIs**: The choice of language for variable names and comments should be defined at the beginning of the project, preferably during the first session of interaction with the programmer.

### 📋 Default Rule

**By default**, when programming with artificial intelligence:
- ✅ **Variable names**: Should be in **English** (recommended for international projects)
- ✅ **Comments**: Should be in **English** (recommended for international projects)
- ✅ **Docstrings**: Should be in **English** (recommended for international projects)

**Note**: For Portuguese-speaking developers working on national projects, **Portuguese is the recommended default**. The AI should adapt based on the programmer's language preference.

**Justification**: Facilitates understanding and maintenance of code for developers, maintaining consistency with project documentation and communication. English is recommended for international projects, while native language (e.g., Portuguese) is recommended for national projects.

### 🤔 Mandatory Question in First Session

**The AI MUST ask the programmer at the first moment (or during the first session)**:

```
❓ Code Language Preferences

To maintain consistency in the project, I need to define the default 
language for variable names and comments in the code:

💡 Suggestion: English (recommended for international projects)
   or Native Language (recommended for national projects)

Options:
A) 🇺🇸 English - Variables and comments in English (RECOMMENDED for international)
B) 🇧🇷 Native Language - Variables and comments in native language (RECOMMENDED for national)
C) 🌍 Mixed - Variables in English, comments in native language
D) ⚙️ Custom - Specify custom preference

What is your preference?
```

### ✅ Available Options

#### Option A: 🇺🇸 English (RECOMMENDED for International Projects)
```python
# ✅ Example in English
def calculate_total_price(items: List[Item]) -> float:
    """
    Calculates the total price of a list of items.
    
    Args:
        items: List of items to be summed
        
    Returns:
        Total price with taxes included
    """
    subtotal_price = sum(item.price for item in items)
    tax_rate = 0.15
    final_price = subtotal_price * (1 + tax_rate)
    return final_price
```

#### Option B: 🇧🇷 Native Language (e.g., Portuguese)
```python
# ✅ Exemplo em Português
def calcular_preco_total(itens: List[Item]) -> float:
    """
    Calcula o preço total de uma lista de itens.
    
    Args:
        itens: Lista de itens a serem somados
        
    Returns:
        Preço total com impostos incluídos
    """
    preco_subtotal = sum(item.preco for item in itens)
    taxa_imposto = 0.15
    preco_final = preco_subtotal * (1 + taxa_imposto)
    return preco_final
```

#### Option C: 🌍 Mixed (Variables in English, Comments in Native Language)
```python
# ✅ Mixed Example
def calculate_total_price(items: List[Item]) -> float:
    """
    Calcula o preço total de uma lista de itens.
    
    Args:
        items: Lista de itens a serem somados
        
    Returns:
        Preço total com impostos incluídos
    """
    subtotal_price = sum(item.price for item in items)
    tax_rate = 0.15  # Taxa de imposto de 15%
    final_price = subtotal_price * (1 + tax_rate)
    return final_price
```

### 📝 Register the Preference

After the programmer's response, the AI should:

1. **Register the preference** in a visible location (e.g., README.md, CONTRIBUTING.md)
2. **Apply consistently** throughout all generated code
3. **Remember the preference** in future sessions of the same project

**Example Registration in README.md**:
```markdown
## 🌐 Code Conventions

- **Code Language**: English
- **Variables**: Names in English (e.g., `active_user`, `calculate_total`)
- **Comments**: In English
- **Documentation**: In English
```

### 🔄 Preference Change

The programmer can request a language change at any time:
- ✅ "Switch to English from now on"
- ✅ "I prefer comments in Portuguese, but variables in English"
- ✅ "Use English only for public APIs"

**The AI should confirm the change** and update the conventions documentation.

### ⚠️ Common Exceptions

Regardless of the language choice, **keep in English**:
- ✅ Library and framework names (e.g., `import pandas`, `from flask import`)
- ✅ Language keywords (e.g., `def`, `class`, `if`, `for`)
- ✅ Public API names (if code is distributed internationally)
- ✅ Technical terms without adequate translation (e.g., `callback`, `payload`, `refactoring`)

### 🎯 Rationale

**Why ask the programmer?**

1. **Project Context**: National vs. international projects have different needs
2. **Team**: Brazilian team may prefer Portuguese; international team needs English
3. **Readability**: Code is read more times than written - should be clear for maintainers
4. **Consistency**: Defining standard at the start avoids confusing language mixing
5. **Professionalism**: Demonstrates attention to detail and respect for developer preferences

**Why English as recommended for international?**

For international/open-source projects:
- ✅ Universal programming language
- ✅ Easier collaboration with developers worldwide
- ✅ Better integration with English documentation and resources
- ✅ Industry standard for libraries and frameworks

**Why Native Language for national projects?**

For national/regional projects (e.g., Portuguese for Brazil/Portugal):
- ✅ Developers read and understand faster
- ✅ Facilitates onboarding of new team members
- ✅ Documentation and code in same language = less mental translation
- ✅ Variables represent business concepts in native language

**When to prefer English?**

- 🌍 International open-source project
- 🌍 Multicultural team
- 🌍 Product aimed at global market
- 🌍 Library/framework for public distribution

---

## 📧 Contact Methods for User Feedback

> **IMPORTANT FOR AIs**: During the first session of interaction with the programmer, the artificial intelligence must ask if the developer would like to include contact methods in the project so that users can provide feedback to those responsible.

### 📋 Context and Purpose

Software projects greatly benefit from direct user feedback. Comments, suggestions, criticisms, complaints, compliments, and opinions are fundamental for the evolution and continuous improvement of the project.

### 🤔 Mandatory Question in the First Session

**The AI MUST ask the programmer at the very first moment (or during the first session)**:

```
❓ Contact Methods for User Feedback

Would you like to include contact methods in the project so users
can send feedback (comments, suggestions, criticisms, complaints,
compliments, and opinions)?

💡 Suggestion: Yes (recommended for projects with end users)

Options:
A) ✅ Yes, include email for feedback (DEFAULT RECOMMENDED)
B) ✅ Yes, include GitHub Issues (for open-source projects)
C) ✅ Yes, include contact form in the application
D) ✅ Yes, include multiple channels (email + issues + form)
E) ❌ No, do not include contact methods

What is your preference?
```

### ✅ Available Options

#### Option A: ✅ Email for Feedback (DEFAULT RECOMMENDED)

**What to include**:
- Dedicated email for feedback
- All types of feedback are welcome:
  - 💬 General comments
  - 💡 Improvement suggestions
  - 🐛 Constructive criticisms
  - 😞 Complaints about problems
  - 🎉 Compliments and recognition
  - 📝 Opinions about features

**Where to document**:
```markdown
## 📧 Feedback and Contact

Your opinion is very important to us! Send your comments, 
suggestions, criticisms, complaints, compliments, and opinions to:

**Email**: feedback@yourproject.com

All feedback is read and considered for future improvements.
```

**Implementation example (README.md)**:
```markdown
## 📮 Feedback

We'd love to hear from you! Send your comments, suggestions, 
criticisms, complaints, compliments, and opinions to:

- **Email**: contact@myproject.com
- **Response**: We typically respond within 48 hours

Your feedback helps us improve continuously!
```

#### Option B: ✅ GitHub Issues

**For open-source projects**:
```markdown
## 🐛 Report Problems or Give Feedback

Use [GitHub Issues](https://github.com/your-user/your-project/issues) to:

- 🐛 Report bugs
- 💡 Suggest new features
- 💬 Share general feedback
- ❓ Ask questions

**Available templates**:
- Bug Report
- Feature Request  
- General Feedback
```

#### Option C: ✅ Contact Form in the Application

**For web/desktop applications**:
- Add "Feedback" or "Contact" section in the interface
- Form with fields:
  - Name (optional)
  - Email (for response)
  - Type: Comment | Suggestion | Criticism | Complaint | Compliment | Opinion
  - Message
- Send via email or save to database

**Implementation example (GUI)**:
```python
# Menu: Help → Send Feedback
class FeedbackDialog(QDialog):
    def __init__(self):
        super().__init__()
        self.setWindowTitle("Send Feedback")
        
        # Feedback type
        self.type_combo = QComboBox()
        self.type_combo.addItems([
            "💬 Comment",
            "💡 Suggestion",
            "🐛 Criticism/Bug",
            "😞 Complaint",
            "🎉 Compliment",
            "📝 Opinion"
        ])
        
        # Email (optional)
        self.email_input = QLineEdit()
        self.email_input.setPlaceholderText("your@email.com (optional)")
        
        # Message
        self.message_text = QTextEdit()
        self.message_text.setPlaceholderText(
            "Share your comments, suggestions, criticisms, "
            "complaints, compliments, or opinions..."
        )
        
        # Send button
        self.send_button = QPushButton("Send Feedback")
        self.send_button.clicked.connect(self.send_feedback)
```

#### Option D: ✅ Multiple Channels

**Combine several options**:
```markdown
## 📞 Get in Touch

We value your feedback! You can contact us through:

### 📧 Email
- **General Feedback**: feedback@project.com
- **Technical Support**: support@project.com
- We respond within 48 hours

### 💬 GitHub Issues
- Report bugs: [Issues](https://github.com/user/project/issues)
- Suggest features: [Discussions](https://github.com/user/project/discussions)

### 🌐 Contact Form
- Access: Menu → Help → Send Feedback
- Or: https://project.com/contact

### 📱 Social Media
- Twitter: [@yourproject](https://twitter.com/yourproject)
- Discord: [Community](https://discord.gg/yourproject)
```

#### Option E: ❌ Do Not Include

**When to choose this option**:
- ⚠️ Personal/internal projects without external users
- ⚠️ Disposable prototypes
- ⚠️ Single-use scripts

**Consequence**: Users will not have a direct channel for feedback, which may limit the project's evolution.

### 📝 Register the Preference

After the programmer's response, the AI should:

1. **Add contact/feedback section** in README.md
2. **Create CONTACT.md file** (if needed) with details
3. **Implement form** (if application with interface)
4. **Document** in CONTRIBUTING.md (for open-source projects)

**Registration example (README.md)**:
```markdown
## 📬 Feedback and Contact

This project values user feedback! 

- **Email**: feedback@project.com
- **Feedback types welcome**: Comments, suggestions, criticisms, 
  complaints, compliments, and opinions
- **Response time**: Within 48 business hours

Your feedback is essential for continuous improvement!
```

### 🎯 Rationale

**Why ask about contact methods?**

1. **Continuous Improvement**: Direct feedback helps identify problems and opportunities
2. **Engagement**: Users who can give feedback feel more connected to the project
3. **Quality**: Criticisms and suggestions improve software quality
4. **Prioritization**: Feedback helps understand what is most important to users
5. **Recognition**: Compliments motivate the development team
6. **Transparency**: Open channel demonstrates commitment to users

**Why Email as default?**

For projects with users:
- ✅ **Universal**: Everyone has email
- ✅ **Simple**: Doesn't require account or additional registration
- ✅ **Direct**: Private and personal communication
- ✅ **Consolidated**: All types of feedback in a single channel
- ✅ **Traceable**: Complete history of communications
- ✅ **Professional**: Formal channel suitable for any type of feedback

**When to prefer other options?**

- 🌍 **GitHub Issues**: Open-source projects (public transparency)
- 🌍 **Form**: Apps with many users (organization and categorization)
- 🌍 **Multiple channels**: Large projects (different audiences, different needs)
- 🌍 **None**: Internal/personal projects without external users

### ⚠️ Important Considerations

**Feedback Management**:
- ✅ Define who will respond to feedback (responsible person)
- ✅ Establish expected response time (SLA)
- ✅ Create process for triage and prioritization
- ✅ Document relevant feedback (issues, backlog)
- ✅ Always thank, even for criticisms

**Privacy**:
- ✅ Inform how contact data will be used
- ✅ Do not share emails without permission
- ✅ GDPR/LGPD compliance if applicable

**Best practices example**:
```markdown
## 📧 Feedback Policy

**We commit to**:
- ✅ Respond to all feedback within 48 business hours
- ✅ Treat all opinions with respect
- ✅ Seriously consider criticisms and suggestions
- ✅ Maintain contact data privacy (GDPR/LGPD)
- ✅ Thank constructive contributions

**You can expect**:
- Personalized response (not automated)
- Updates on implemented suggestions
- Recognition in changelogs (if desired)
```

---

## 📊 Recursive Division of Complex Tasks

> **IMPORTANT**: If the task is very long or complex, and there are time limits or response length limits, the artificial intelligence should divide the task into smaller parts, recursively, until achieving a task that can provide a satisfactory response according to the determined response limit.

### 🔄 Division Strategy (Enterprise)

**When to Apply** (Simplicity Protocol 2):
- ✅ Task estimated at >6 hours (divide into 3+ sprints)
- ✅ Enterprise feature with multiple stakeholders
- ✅ Very long response (>1500 lines of code)
- ✅ Multiple interdependent functionalities
- ✅ Requires peer code review at each phase
- ✅ Risk of timeout or response limit

**How to Divide** (Recursively with ADRs):

1. **Level 1 - Epics (2-4 weeks)**:
   ```
   Epic: "Enterprise Payment System"
   ↓ Divide into:
   ├── Sprint 1: Stripe Integration (6h)
   ├── Sprint 2: Webhooks and notifications (6h)
   ├── Sprint 3: Transaction dashboard (8h)
   ├── Sprint 4: Audit and compliance (6h)
   └── Sprint 5: Rollback and recovery (4h)
   
   Each sprint → Documented ADR
   Each sprint → Peer code review
   Each sprint → Incremental deployment
   ```

2. **Level 2 - Sprints (4-8 hours)**:
   ```
   Sprint 1: Stripe Integration
   ↓ Divide into:
   ├── Task 1.1: Setup API keys + secrets (1h)
   ├── Task 1.2: Checkout session endpoint (2h)
   ├── Task 1.3: Webhook receiver (2h)
   └── Task 1.4: Tests + Security checklist (1h)
   
   Each task → Quality gates (CI/CD)
   ```

3. **Level 3 - Tasks (<4 hours)** (if still too large):
   ```
   Task 1.2: Checkout session endpoint
   ↓ Divide into:
   ├── Subtask 1.2.1: Order schema (30min)
   ├── Subtask 1.2.2: Input validation (30min)
   ├── Subtask 1.2.3: Stripe session creation (1h)
   ├── Subtask 1.2.4: Logging and monitoring (30min)
   └── Subtask 1.2.5: Unit tests (1h)
   ```

**Stopping Criteria**:
- ⏱️ Task can be completed in <4 hours (vs <3h in Simplicity 1)
- 📝 Response fits within reasonable limit (<1000 lines)
- ✅ Clear scope with defined acceptance criteria
- 🧪 Can be tested in isolation
- 👥 Can be peer-reviewed in <1h
- 🔒 Security checklist can be applied in isolation
- 🤖 CI/CD can validate in isolation

**Enterprise Division Principles**:
1. **Independence**: Each subtask must be independently deployable
2. **Cohesion**: Related subtasks should be close in sequence
3. **Incremental Value**: Each subtask should add measurable value
4. **Testability**: Each subtask must have 100% test coverage
5. **Reversibility**: Each subtask must have rollback plan (if critical)
6. **Documentation**: Each sprint must have ADR if architectural decision
7. **Reviewability**: Each subtask must have small diff for code review

**Practical Enterprise Example**:
```markdown
❌ BAD - Epic too large (60h):
[ ] Implement complete e-commerce platform

✅ GOOD - Divided into epics and sprints:

Epic 1 - Product Catalog (2 weeks):
├── Sprint 1.1 (6h): Product CRUD + categories
│   ├── ADR-001: PostgreSQL choice
│   └── Rollback plan: N/A (non-critical)
├── Sprint 1.2 (6h): Search and filters
│   └── ADR-002: ElasticSearch vs PostgreSQL full-text
└── Sprint 1.3 (4h): Image upload (S3)
    └── Rollback plan: Revert to local storage

Epic 2 - Shopping Cart (1 week):
├── Sprint 2.1 (6h): Session-based cart
│   ├── ADR-003: Redis for sessions
│   └── Security checklist: Session fixation, CSRF
└── Sprint 2.2 (4h): Persistence and checkout
    └── Rollback plan: Fallback to in-memory

Epic 3 - Payments (2 weeks):
├── Sprint 3.1 (6h): Stripe Integration
│   ├── ADR-004: Stripe vs PayPal
│   ├── Security checklist: PCI-DSS compliance
│   └── Rollback plan: CRITICAL (feature flag)
├── Sprint 3.2 (6h): Webhooks
│   └── Security checklist: Webhook validation
└── Sprint 3.3 (4h): Transaction dashboard
    └── Rollback plan: N/A (visualization only)

Each Sprint:
- Code review by 2 peers
- CI/CD quality gates (80% coverage)
- Security scan (bandit + pip-audit)
- Deploy staging → production
```

**Decision Matrix for Division**:
Use Decision Matrix (Step 2.5) when there are multiple ways to divide:

| Division | Complexity | Risk | Value | Independence | **Score** |
|---------|------------|------|-------|--------------|-----------|
| **By functionality** | 3 | 2 | 5 | 5 | **23** 🟢 |
| By layer (backend/frontend) | 2 | 4 | 3 | 2 | **17** 🟡 |
| By team | 4 | 3 | 2 | 3 | **18** 🟡 |

**Why?**: Dividing enterprise tasks ensures incremental deliveries with value, facilitates code review, allows granular rollback, and maintains stable velocity in large teams.

---

## 📋 Protocol Backbone (24 Steps: 14 Mandatory + 10 Optional)

### **Mandatory Steps** (Simplicity Protocol 1):
1. 📚 Read the documentation
2. ✅ Choose simpler tasks
3. ❓ Ask questions until 100% clarity
4. 🔍 Analyze and study the project
5. 🎯 Sprint the simpler tasks
6. 💻 Implement with professional architecture (GoF + GRASP)
   - 6.6 🎨 **Project Icons** (MANDATORY)
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
**6.7** 📚 Generate API Documentation
**8.5** ♿ Accessibility Checklist (WCAG)
**9.5** 👥 Peer Code Review
**10.5** ⚡ Profiling and Optimization
**10.6** ✅ Quality Metrics (CI/CD) - **HIGH PRIORITY**
**11.5** 📋 Create ADR (Architectural Decision Records)
**12.5** 🔙 Rollback Plan
**13.5** 🔄 Sprint Retrospective

### 1️⃣ **Read the Documentation**

> **🚨 CRITICAL FOR AIs - FIRST MANDATORY ACTION**: Before ANYTHING else, AI **MUST** search for and read **100% of local markdown documentation** existing in the project.

#### 📖 **Step 1.0: Complete Documentation Search and Reading** [PRIORITY]

**Core functionality**: Same as Simplicity Protocol 1 Step 1.0, with the following **enterprise additions**:

**Additional files to read (Enterprise)**:
- ✅ `docs/ADR/*.md` - **Architecture Decision Records (CRITICAL)**
- ✅ `docs/api/*.md` - API documentation
- ✅ `docs/security/*.md` - Security checklists (OWASP)
- ✅ Corporate standards documentation

**[SPECIFIC FOR SIMPLICITY 2 - ENTERPRISE]**:
- ✅ **ADRs are critical**: Formal architectural decisions must be read FIRST
- ✅ **Corporate standards**: Read documentation about company patterns
- ✅ **Compliance**: Documentation about regulatory requirements

**Enterprise Minimum Structure** (if creating from scratch):
```
📁 Project Root
├── README.md
├── TASKS.md
└── 📁 docs/
    ├── REQUIREMENTS.md
    ├── ARCHITECTURE.md
    ├── v0.1.0-SPECIFICATIONS.md
    ├── 📁 ADR/                  # MANDATORY
    │   └── template-adr.md
    ├── 📁 security/             # MANDATORY
    │   └── OWASP-checklist.md
    └── 📁 api/
        └── api-reference.md
```

**Enterprise README template** includes:
- Stakeholders (Product Owner, Tech Lead, Dev Team, QA, Security)
- Formal ADR references
- Security and compliance policies

**Enterprise ADR template**:
```markdown
# ADR-XXX: [Decision Title]

**Status**: Proposed | Accepted | Superseded | Rejected
**Date**: YYYY-MM-DD
**Decision by**: [Tech Lead/Architect name]
**Approvers**: [Names of approvers]

## Context
[Problem or need leading to this decision]

## Decision
[Clear and objective description of decision made]

## Alternatives Considered
1. **Alternative A**: [Description] - Rejected because [reason]
2. **Alternative B**: [Description] - Rejected because [reason]

## Consequences
**Positive**:
- [Benefit 1]
- [Benefit 2]

**Negative** (trade-offs):
- [Trade-off 1]
- [Trade-off 2]

## Validation
- ✅ Approved by: [Approver names]
- ✅ Meeting date: [YYYY-MM-DD]
- ✅ Vote: [X in favor, Y against, Z abstentions]

## References
- [Link to technical documentation]
- [Link to similar use cases]
- [Link to benchmarks]

## Future Review
- Review date: [YYYY-MM-DD + 6 months]
- Success criteria: [How to measure if decision was correct]
```

**Enterprise Checklist** (12 items):
```markdown
[ ] 🔍 Recursively searched all .md files
[ ] 📖 Read 100% of ALL files found
[ ] 📋 Read ALL existing ADRs (formal architectural decisions)
[ ] 🔐 Read security and compliance documentation
[ ] 📝 If no documentation, asked user/team
[ ] 📚 If doesn't exist, created enterprise structure (including ADR template)
[ ] 🎯 Understood goal, stakeholders and organizational structure
[ ] 📋 Know pending tasks and who are responsible
[ ] 🛠️ Know tech stack and its ADR choice
[ ] 🏗️ Understood architectural decisions and rationale
[ ] 👥 Know who are approvers for future decisions
[ ] ✅ Ready to work with complete enterprise context
```

**Rationale (Enterprise)**:
- ✅ **Formal Decisions**: ADRs document why choices were made
- ✅ **Compliance**: Not following corporate standards can block deploy
- ✅ **Team Coordination**: Multiple devs need shared context
- ✅ **Auditing**: Documentation is evidence for audits
- ✅ **Onboarding**: New team members depend on complete documentation
- ✅ **Rework Cost**: In large teams, rework is exponentially more expensive

**Message for AIs (Enterprise)**:
> "In enterprise environments, documentation is not optional - it's MANDATORY and FORMAL. Reading 100% of ADRs, security checklists and compliance documentation BEFORE coding is a critical requirement. Decisions without ADR can be rejected in code review."

**Golden Rule (Enterprise)**:
> **"In enterprise, documentation is evidence. There is no work done without formal documentation."**

📖 **See Simplicity Protocol 1 Step 1.0** for complete templates and detailed examples. Enterprise additions are noted above.

---

### 1️⃣.5️⃣ **Research Suitable Technologies for the Project** [MANDATORY AT START]

**Core functionality**: Same as Simplicity Protocol 1 Step 1.5, with the following **enterprise additions**:

**Additional requirements to collect (Enterprise)**:
- 📌 **Current company stack** (if there's a standard corporate stack)
- 📌 **Compliance and audit requirements**
- 📌 **Organizational structure**: Who are responsible (Product Owner, Tech Lead, Devs)
- 📌 **Approval processes**: What's the code review flow

**[SPECIFIC FOR SIMPLICITY 2 - ENTERPRISE]**:

**Default Web Stack - Enterprise Considerations**:

When recommending Next.js 15 + React 19 + TypeScript stack (see Protocol 1 for full details):

**Additional Enterprise Validations**:
- ✅ **TypeScript Mandatory**: Type safety for large teams
- ✅ **ESLint + Husky**: Automated code quality
- ✅ **Monorepo-ready**: Turbo supports multiple packages
- ✅ **Market Standard**: Next.js used by Netflix, TikTok, Uber
- ✅ **Commercial Support**: Vercel offers enterprise plans
- ✅ **Compliance**: HTTPS, WCAG, GDPR-compliant

**⚠️ Mandatory Enterprise Validation**:
1. **Technical Decision Meeting**: Present stack to team/architects
2. **Stakeholder Approval**: Tech Lead + CTO validate choice
3. **Create Formal ADR**: Document decision in `docs/ADR/adr-001-web-stack.md`
4. **Corporate Compliance**: Verify alignment with company standards
5. **Cost Analysis**: Estimate Vercel Pro/Enterprise cost (if applicable)

**When NOT to use Default Stack (Enterprise specific)**:
- ❌ Company has mandatory corporate stack (e.g., Java + Spring)
- ❌ Compliance restrictions prevent CDN usage (Vercel, Cloudinary)
- ❌ Existing enterprise architecture requires different tech

**ADR Template for Tech Stack Choice**:
```markdown
# ADR-001: Web Technology Stack Selection

**Status**: Accepted
**Date**: YYYY-MM-DD
**Decision by**: [Tech Lead name]
**Approvers**: [CTO, Tech Lead, Architect]

## Context
Project requires modern web application with [requirements].
Team size: [X developers].
Expected scale: [Y users].

## Decision
We will adopt Next.js 15 + React 19 + TypeScript stack:
- Frontend: Next.js 15.5.2 + React 19.1.1 + TypeScript 5.9.2
- Styling: Tailwind CSS 3.4.17
- State: Zustand 4.5.7
- Deploy: Vercel
[Complete stack list - see Protocol 1 Step 1.5]

## Alternatives Considered
1. **Vue 3 + Nuxt**: Rejected due to smaller talent pool in company
2. **Angular**: Rejected due to steeper learning curve
3. **Create React App**: Rejected due to lack of SSR (SEO requirement)

## Consequences
**Positive**:
- TypeScript provides type safety for large team
- Next.js SSR optimizes SEO
- Vercel deploy simplifies CI/CD
- Market standard facilitates hiring

**Negative**:
- Vercel cost at scale (estimated $X/month at 100k users)
- Team needs Next.js 15 training (1 week)

## Validation
- ✅ Approved by: [CTO name], [Tech Lead name], [Architect name]
- ✅ Meeting date: YYYY-MM-DD
- ✅ Vote: 5 in favor, 0 against, 0 abstentions

## Cost Analysis
- Development: Vercel free tier sufficient
- Production: Estimated $500/month (Pro plan)
- Training: 40h × $100/h = $4,000

## Compliance
- ✅ HTTPS: Vercel provides automatic SSL
- ✅ WCAG 2.1: Tailwind + proper HTML supports accessibility
- ✅ GDPR: Data processing compliant (no PII in frontend)
- ✅ Corporate policy: Aligns with "modern stack" guideline

## References
- Next.js docs: https://nextjs.org/docs
- Vercel enterprise: https://vercel.com/enterprise
- Similar projects: [Internal project X] uses same stack

## Future Review
- Review date: 2026-07-01 (6 months)
- Success criteria: 
  - Deploy time < 5min
  - Team productivity +30%
  - Zero major blockers related to stack choice
```

**Enterprise Checklist** (13 items):
```markdown
[ ] Requirements collected (features, scale, compliance)
[ ] Company's current stack verified (if applicable)
[ ] Investigation of professional technologies performed
[ ] Online research performed (if necessary)
[ ] 2-3 complete stacks recommended with justifications
[ ] Advantages, disadvantages and real use cases presented
[ ] Learning complexity evaluated
[ ] Licensing cost analyzed (if applicable)
[ ] Technical decision meeting held (Enterprise)
[ ] Team consensus obtained
[ ] ADR created and approved (Step 11.5)
[ ] Stack documented in docs/ARCHITECTURE.md
[ ] Stakeholders informed of decision
```

📖 **See Simplicity Protocol 1 Step 1.5** for complete technology categories, default web stack details (80+ dependencies with versions), and detailed templates. Enterprise-specific additions are documented above.

**Rationale (Enterprise)**:
> "In enterprise environments, tech stack choice has organizational impact. Don't recommend experimental technologies. Prioritize maturity, commercial support and compliance with corporate standards. Decision must be collective and formally documented via ADR."

**Golden Rule (Enterprise)**:
> **"Tech stack is an ARCHITECTURAL decision. Requires ADR, formal approval and alignment with corporate standards."**

---

### 2️⃣ **Choose the Simplest Tasks**

In addition to `TASKS.md`, you can create **Action Plans** for tasks requiring detailed step-by-step guidance.

**What are Action Plans?**
- 🎯 **Practical roadmaps** with numbered intermediate steps for complex tasks
- ⚡ **More urgent and detailed** than TASKS.md items
- 🔧 **Applicable to**: Maintenance, Correction, Evolution, Adaptation
- 📋 **Created BEFORE** starting implementation
- 📖 **Consulted always** during development

**Difference between TASKS.md and Action Plans:**
- **TASKS.md**: List of general tasks ("WHAT to do") - e.g., `[ ] Implement OAuth2 authentication`
- **Action Plan**: Detailed execution guide ("HOW to do it") - e.g.:
  ```
  PLAN #01: Implement OAuth2
  ├─ Step 1: Install passport.js library
  ├─ Step 2: Configure Google OAuth strategy
  ├─ Step 3: Create /auth/google routes
  └─ Step 4: Add tests
  ```

**When to use Action Plans:**
- ✅ Complex task with multiple interdependent steps
- ✅ Critical bug requiring step-by-step diagnosis
- ✅ Refactoring affecting multiple modules
- ✅ Technology migration or framework update

**Specifics for Simplicity 2 (Enterprise):**
- 🤝 **Team validation**: Action plans must be reviewed by peers before execution
- 📋 **Create ADR**: For action plans involving significant architectural decisions (see Step 11.5)
- 👥 **Clear assignment**: Each plan step must have assigned responsible person
- 📊 **Metrics**: Include measurable success metrics for each step

**Organization of Action Plans:**

**Option 1**: Consolidated file `docs/ACTION_PLANS.md`  
**Option 2**: Individual plans directory `docs/plans/`
```
docs/
├── TASKS.md
├── ACTION_PLANS.md [optional - index]
└── plans/
    ├── plan-001-oauth2.md
    ├── plan-002-migration.md
    └── plan-003-refactoring.md
```

**Recommendation**: For enterprise projects with multiple complex tasks, use `docs/plans/`.

**Required Fields for an Action Plan:**
1. **📅 Date** (YYYY-MM-DD): Plan creation date
2. **🕐 Time** (HH:MM): Plan creation time
3. **🎯 Main Function**: Main objective of the plan
4. **📋 Desired Requirement**: What needs to be achieved
5. **✅ Expected Result**: Measurable success criteria
6. **📌 Task ID**: Link to Task from TASKS.md (mandatory)

**Template for Simplicity 2 (Enterprise):**
```markdown
## 🎯 ACTION PLAN #[ID]: [Title]
**📅 Date**: YYYY-MM-DD
**🕐 Time**: HH:MM
**⚡ Priority**: 🔴 Critical | 🟡 High | 🟢 Normal
**🏷️ Type**: Maintenance | Correction | Evolution | Adaptation
**📌 Task ID**: Task #X from TASKS.md
**🎯 Main Function**: [Plan objective]
**📋 Desired Requirement**: [What should be achieved]
**✅ Expected Result**: [Success criteria]
**👤 Lead**: [Lead name]
**👥 Reviewers**: [Reviewer names]

### 📝 Context
[Why was this plan created?]

### 📋 Intermediate Steps
- [ ] **Step 1**: [Description]
  - **Responsible**: [Name]
  - **Completion criteria**: [...]
  - **Success metrics**: [...]
  
- [ ] **Step 2**: [Description]
  - **Responsible**: [Name]
  - **Completion criteria**: [...]
  - **Dependencies**: Step 1
[...]

### ✅ Completion Criteria
- [ ] All steps completed
- [ ] Code Review approved (see Step 9.5)
- [ ] Tests passing
- [ ] Documentation updated
- [ ] ADR created (if architectural decision)
```

**Workflow with Action Plans (Enterprise):**
1. Consult TASKS.md to see pending tasks
2. If complex task → **CREATE Action Plan BEFORE starting**
3. Choose location: `docs/ACTION_PLANS.md` or `docs/plans/plan-[ID]-[name].md`
4. **Team review**: Validate plan before starting execution
5. **Assign responsible parties** for each step
6. **BEFORE implementing**: Everyone reviews and approves the plan
7. Execute step by step, **consulting the plan whenever needed**
8. Code review of each stage as progress is made
9. Upon completion → mark task in TASKS.md as complete
10. **Retrospective**: Discuss lessons learned (Step 13.5)
11. Archive plan in `docs/plans/archive/` or "History" section

**Why create BEFORE and consult ALWAYS?**
- ✅ **Team Alignment**: Everyone understands the plan before starting
- ✅ **Avoids Rework**: Early review identifies design problems
- ✅ **Coordination**: Responsible parties know their assignments from the start
- ✅ **Stay Synchronized**: Consulting during work keeps everyone aligned

**Benefits for teams:**
- ✅ **Coordination**: Everyone knows who does what and when
- ✅ **Quality**: Multiple reviews reduce errors
- ✅ **Shared knowledge**: Plan documents process for entire team
- ✅ **Onboarding**: New members learn from previous plans

📖 **Complete details on Action Plans**: See README.md in repository, section "🎯 Action Plans"

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

### 2️⃣.6️⃣ **Ordinal Task Organization** ⭐ HIGHLY RECOMMENDED FOR TEAMS

> **For Enterprise Teams**: Essential system for coordinating parallel development and minimizing conflicts.

**When to Use** (Simplicity 2):
- ✅ Projects with **medium/large teams** (3+ developers)
- ✅ **>15 interdependent tasks**
- ✅ **Multiple features** being developed simultaneously
- ✅ Need for **maximum parallelization**
- ✅ Risk of **frequent merge conflicts**

#### 📊 Prefix System for Teams

**Hierarchy with Letters and Numbers**:
```markdown
🔴 MUST HAVE - Release v1.0.0

A. Infrastructure (Owner: DevOps Team)
   🔴🟢 [ ] A.1. Directory structure (0.5h)
   🔴🟢 [ ] A.2. CI/CD pipeline (1h)

B. Backend API (Owner: Backend Team)
   🔴🟡 [ ] B.1. User model (1.5h)
   🔴🟡 [ ] B.2. API endpoints (2h) - Depends: B.1
   🔴🔴 [ ] B.3. JWT Authentication (2.5h) - Depends: B.2

C. Frontend (Owner: Frontend Team)
   🔴🟢 [ ] C.1. Basic components (1h)
   🔴🟡 [ ] C.2. Login screen (2h) - Depends: B.3, C.1
```

**Parallelization Analysis**:
- ✅ Groups A, B, C start **simultaneously**
- ✅ A.1, B.1, C.1 can be done **in parallel**
- ❌ B.2 waits for B.1 (dependency)
- ❌ C.2 waits for B.3 and C.1 (cross-dependencies)

**Branch Strategy** (Teams):
```markdown
Branch Strategy:
├── feat/infra (DevOps): A.1 → A.2
├── feat/backend-api (Backend): B.1 → B.2 → B.3
└── feat/frontend (Frontend): C.1 → C.2 (waits for B.3)

Coordination Points:
1. Sprint 1: Merge A.1, B.1, C.1 (parallel)
2. Sprint 2: Backend continues B.2, B.3
3. Sprint 3: Merge B.3, Frontend can start C.2
```

#### 🤝 Team Coordination

**Code Review and Dependencies**:
```markdown
B.C.2. Tree → RPN conversion
   B.C.2.1. Parser (Dev: Alice)
   B.C.2.2. Serializer (Dev: Bob)
   B.C.2. Integration (Dev: Carol) - Waits for Alice and Bob's PRs

Workflow:
1. Alice and Bob work in parallel (B.C.2.1, B.C.2.2)
2. Alice opens PR #45 → Code Review by Charlie
3. Bob opens PR #46 → Code Review by Charlie
4. Carol waits for merge of #45 and #46
5. Carol starts B.C.2, creates PR #47
```

#### 📋 ADR and Ordinal Organization

For architectural decisions affecting multiple tasks:

```markdown
# ADR-005: ORM Choice for Backend

**Context**: Task B.1 (User Model) needs to define ORM

**Decision**: SQLAlchemy 2.0

**Impact on Tasks**:
- B.1: Implement with SQLAlchemy
- B.2: API endpoints will use SQLAlchemy sessions
- B.3: JWT validation integrates with User model
- C.2: Frontend waits for B.2 endpoints

**Communication**: 
- Notify Backend Team (B.x tasks)
- Update technical documentation
```

#### ✅ Benefits for Enterprise Teams

**For Developers**:
- ✅ Autonomy: Know which task to start without asking the lead
- ✅ Visibility: See which tasks are blocked
- ✅ Coordination: Identify when to wait for colleague's merge

**For Tech Leads**:
- ✅ Planning: Allocate developers to parallel tasks
- ✅ Monitoring: Track progress by ordinal prefix
- ✅ Risk: Identify bottlenecks (serial dependencies)

**For the Project**:
- ✅ Speed: Maximum parallelization reduces time 40-60%
- ✅ Quality: Correct order avoids rework
- ✅ Conflict reduction: Isolated branches by group
- ✅ Onboarding: New members understand structure quickly

#### 🔄 Retrospectives and Ordinal Organization

At the end of sprint (Step 13.5 - Retrospective):

```markdown
# Sprint #5 Retrospective - Parallelization Analysis

**What Worked**:
✅ Groups A and B were 100% parallel (zero conflicts)
✅ Ordinal prefixes facilitated planning

**What Didn't Work**:
❌ We underestimated C.2's dependency on B.3
❌ Frontend Team was blocked for 2 days

**Actions for Next Sprint**:
- [ ] Map cross-dependencies BEFORE starting sprint
- [ ] Add ordinal prefix that reflects cross-dependencies
- [ ] Example: C.B.3.2 (indicates C.2 depends on B.3)
```

📘 **Complete Documentation**: See `ORDINAL_TASK_ORGANIZATION.md` for:
- Deep hierarchy (C.B.1.D.1)
- Complex project examples
- Decision flowchart
- AI instructions

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

#### 🌐 **Online Research: When AI Has Many Doubts or Difficulties**

> **IMPORTANT FOR AIs**: If you have **many doubts** about how to solve a particular problem, or have **significant difficulties** solving that same problem, **remember that you can perform online research**.

**When to Perform Online Research**:
- ✅ When there are complex technical doubts that you cannot resolve alone
- ✅ When you encounter a critical problem that has no obvious solution in the existing code
- ✅ When you need to understand how to implement something completely new
- ✅ When there is an error or bug that is difficult to diagnose
- ✅ When you need practical implementation examples

**Where to Search** (in order of priority):
1. **📚 Official GitHub Documentation of Related Projects**:
   - Similar repositories or those that solve similar problems
   - Issues and Pull Requests discussing similar problems
   - Wiki and technical documentation of related open source projects

2. **📖 Online Documentation Platforms**:
   - Official documentation of libraries and frameworks used in the project
   - Specialized tutorials and technical guides
   - Technical blogs and articles from experienced developers

3. **💬 Question and Answer Platforms**:
   - **StackOverflow**: Main platform for programming questions
   - **GitHub Discussions**: For project-specific questions
   - Other technical communities relevant to the project's technology

**Why Online Research Is Important**:
- ✅ **Saves time**: Complex problems may already have documented solutions
- ✅ **Best practices**: Learn from implementations already validated by the community
- ✅ **Avoid reinventing the wheel**: Many problems have already been solved by other developers
- ✅ **Reduces errors**: Solutions tested and approved by the community have fewer bugs
- ✅ **Updates**: Discover the most modern and efficient approaches

**Example Flow with Online Research**:
```
1. ❓ I tried to implement [feature X] but encountered [problem Y]
2. 🔍 I searched on GitHub: "similar implementation [feature X]"
3. 📚 I found 3 similar projects that solve this in different ways
4. 💡 I analyzed the examples and identified the most appropriate approach for our context
5. ✅ I implemented based on the best practices found
6. 📝 I documented the solution source for future reference
```

**⚠️ Important**: Always cite the consulted sources in the project documentation for future reference and traceability.

---

### 4️⃣ **Analyze and Study the Project**
- **CRITICAL**: After understanding all doubts, **study the code before implementing**
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
- Maintain focus: **one sprint = one version (e.g., vX.Y.Z)**

**⚠️ Important - Task Division into Subtasks**:
> Tasks should be divided into smaller parts **only if really necessary**, that is:
> - ✅ When there is **higher probability of exceeding the maximum time** (>4h)
> - ✅ When there is **higher possibility the response will be too long** (complex implementation)
> - ❌ **DO NOT divide** if the task is reasonably simple and fits within the time limit
> 
> This decision should be made by the **artificial intelligence responsible for programming** the project, based on the real complexity of the task.

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

#### 🌳 **Import Tree Analogy**

**Concept**: A program's import structure can be visualized as a tree, where each module imports other modules, forming a dependency hierarchy.

**Unlimited Depth**: This tree can reach **any level or height** depending on program complexity:
- **Simple Programs**: Shallow tree (2-3 levels)
  ```
  main.py
  └── utils.py
      └── helpers.py
  ```

- **Medium Programs**: Moderate tree (4-6 levels)
  ```
  app.py
  ├── controllers/
  │   └── user_controller.py
  │       └── services/
  │           └── user_service.py
  │               └── models/
  │                   └── user.py
  └── config.py
  ```

- **Complex Programs**: Deep tree (7+ levels)
  ```
  enterprise_app.py
  ├── api/
  │   ├── routes/
  │   │   └── v1/
  │   │       └── users.py
  │   │           └── handlers/
  │   │               └── authentication.py
  │   │                   └── providers/
  │   │                       └── oauth/
  │   │                           └── google.py
  │   │                               └── scopes.py
  ```

**Application in Refactoring**:

1. **Identify Excessive Depth**:
   - ✅ If tree > 8 levels → Consider simplification
   - ✅ Very deep modules = difficult maintenance

2. **Detect Circular Dependencies**:
   ```python
   # ❌ BAD: Circular dependency
   # module_a.py
   from module_b import B
   
   # module_b.py
   from module_a import A  # Circular!
   ```

3. **Reorganize by Cohesion**:
   ```python
   # ✅ GOOD: Group related imports
   # before (dispersed):
   from utils.string import normalize
   from helpers.text import clean
   from tools.format import sanitize
   
   # after (cohesive):
   from text_processing import normalize, clean, sanitize
   ```

4. **Reduce Coupling**:
   - ✅ Direct imports only of what's necessary
   - ✅ Avoid `from module import *` (increases coupling)
   - ✅ Use interfaces/abstractions to decouple

5. **Visualize to Understand**:
   - Use tools like `pydeps`, `import-graph` (Python)
   - Identify "hubs" (heavily imported modules)
   - Refactor central modules to reduce impact

**Why it's important**:
- ✅ **Comprehension**: Clear tree = easier to understand code
- ✅ **Maintenance**: Organized dependencies = localized changes
- ✅ **Performance**: Fewer unnecessary imports = faster startup
- ✅ **Testing**: Independent modules = isolated tests
- ✅ **Refactoring**: Visualizing tree helps identify improvement opportunities

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

### 6️⃣.6️⃣ **Project Icons** [MANDATORY]

> **CRITICAL FOR AIs**: Every project must include appropriate icons to ensure professionalism and visual identity.

**When to Apply**: During implementation (Step 6), after defining the basic project structure.

#### 📋 Mandatory Requirement

Artificial intelligence **MUST** produce or download an icon for the project, whether:
- 🌐 Website/Web Application
- 💻 Desktop Program
- 📱 Mobile Application
- 🔧 Tool/Utility

#### 🎨 Icon Formats by Technology

**Web Applications**:
- ✅ **favicon.ico** (16x16, 32x32, 48x48 px) - Universal compatibility
- ✅ **icon.svg** - Vector, scalable, modern
- ✅ **icon-192.png** and **icon-512.png** - PWA/Android
- ✅ **apple-touch-icon.png** (180x180 px) - iOS

**Desktop Applications**:
- ✅ **icon.png** (256x256, 512x512 px) - Linux
- ✅ **icon.ico** (multiple sizes) - Windows
- ✅ **icon.icns** - macOS

**Mobile Applications**:
- ✅ **icon.png** (1024x1024 px) - iOS App Store
- ✅ **ic_launcher.png** (multiple densities) - Android
- ✅ **adaptive-icon.xml** - Android adaptive

#### 📁 Folder Structure (MANDATORY)

Icons **MUST** be organized in a dedicated folder:

```
project/
├── assets/              # ✅ PREFERRED (default for all)
│   ├── icons/
│   │   ├── favicon.ico
│   │   ├── icon.svg
│   │   ├── icon-192.png
│   │   ├── icon-512.png
│   │   └── apple-touch-icon.png
│   └── ...
│
# OR alternatives according to technology:
├── public/              # ✅ React, Vue, Next.js
│   ├── favicon.ico
│   └── icons/
├── static/              # ✅ Flask, Django, Svelte
│   └── icons/
├── src/assets/          # ✅ Angular, Ionic
│   └── icons/
├── resources/           # ✅ Electron, Tauri
│   └── icons/
└── res/                 # ✅ Native Android
    └── drawable/
```

**Golden Rule**: Always use a specific folder for icons, never loose files at the project root.

#### 🔧 How to Obtain/Create Icons

AI must follow this priority order:

1. **Ask the Programmer** (ALWAYS first):
   ```
   ❓ Do you already have an icon for the project?
   
   Options:
   A) ✅ Yes, I have (provide the path/file)
   B) 🎨 No, create a simple icon for me
   C) 🔍 No, download a suitable free icon
   D) ⏭️ Skip for now (not recommended)
   ```

2. **If A (User provides)**:
   - Validate format and size
   - Convert to necessary formats (use tools like `convert`, `sharp`, `imagemagick`)
   - Organize in the correct folder

3. **If B (AI creates simple icon)**:
   - Create vector SVG icon with project initials
   - Export to necessary formats (PNG, ICO)
   - Use project identity colors (if defined)

4. **If C (AI downloads icon)**:
   - Use free and copyright-free sources:
     - ✅ [Heroicons](https://heroicons.com/) (MIT License)
     - ✅ [Lucide Icons](https://lucide.dev/) (ISC License)
     - ✅ [Tabler Icons](https://tabler-icons.io/) (MIT License)
     - ✅ [Iconoir](https://iconoir.com/) (MIT License)
   - Verify license before using
   - Document source in README

5. **If D (Skip)**:
   - ⚠️ Warn that project will lack visual identity
   - Add task in TASKS.md for future: `[ ] Create project icon`

#### 🎨 Simple SVG Icon Example (Generated by AI)

```svg
<!-- assets/icons/icon.svg -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100">
  <rect width="100" height="100" rx="20" fill="#4F46E5"/>
  <text x="50" y="65" font-family="Arial, sans-serif" font-size="48" 
        font-weight="bold" fill="white" text-anchor="middle">MP</text>
</svg>
```

#### 🔨 Icon Conversion Tools

**Python** (recommended for automation):
```bash
# Install Pillow
pip install Pillow

# Convert SVG to PNG (via cairosvg)
pip install cairosvg
python -c "import cairosvg; cairosvg.svg2png(url='icon.svg', write_to='icon.png', output_width=512)"

# Create ICO with multiple sizes
from PIL import Image
img = Image.open('icon.png')
img.save('favicon.ico', format='ICO', sizes=[(16,16), (32,32), (48,48)])
```

**Node.js** (web projects):
```bash
# Install sharp
npm install sharp

# Conversion script
node -e "
const sharp = require('sharp');
sharp('icon.svg').resize(192, 192).toFile('icon-192.png');
sharp('icon.svg').resize(512, 512).toFile('icon-512.png');
"
```

**ImageMagick** (universal):
```bash
# Convert SVG to PNG
convert icon.svg -resize 192x192 icon-192.png

# Create favicon.ico
convert icon.png -define icon:auto-resize=16,32,48 favicon.ico
```

#### 🗂️ Project Integration

**HTML (Web)**:
```html
<!-- index.html -->
<head>
  <!-- Basic favicon -->
  <link rel="icon" type="image/x-icon" href="/assets/icons/favicon.ico">
  
  <!-- Modern SVG (preferred) -->
  <link rel="icon" type="image/svg+xml" href="/assets/icons/icon.svg">
  
  <!-- PNG for different sizes -->
  <link rel="icon" type="image/png" sizes="32x32" href="/assets/icons/icon-32.png">
  <link rel="icon" type="image/png" sizes="192x192" href="/assets/icons/icon-192.png">
  
  <!-- Apple Touch Icon -->
  <link rel="apple-touch-icon" href="/assets/icons/apple-touch-icon.png">
  
  <!-- Android Chrome -->
  <link rel="manifest" href="/manifest.json">
</head>
```

**manifest.json (PWA)**:
```json
{
  "name": "My Project",
  "short_name": "MP",
  "icons": [
    {
      "src": "/assets/icons/icon-192.png",
      "sizes": "192x192",
      "type": "image/png"
    },
    {
      "src": "/assets/icons/icon-512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ]
}
```

**Python (Desktop - PyQt/Tkinter)**:
```python
# PyQt6
from PyQt6.QtGui import QIcon
from PyQt6.QtWidgets import QApplication

app = QApplication([])
app.setWindowIcon(QIcon('assets/icons/icon.png'))

# Tkinter
import tkinter as tk
root = tk.Tk()
root.iconbitmap('assets/icons/icon.ico')  # Windows
# or
root.iconphoto(True, tk.PhotoImage(file='assets/icons/icon.png'))  # Linux/Mac
```

**Electron (Desktop)**:
```javascript
// main.js
const { app, BrowserWindow } = require('electron');
const path = require('path');

const win = new BrowserWindow({
  icon: path.join(__dirname, 'resources/icons/icon.png')
});
```

**React Native (Mobile)**:
```
// android/app/src/main/res/
mipmap-hdpi/ic_launcher.png      (72x72)
mipmap-mdpi/ic_launcher.png      (48x48)
mipmap-xhdpi/ic_launcher.png     (96x96)
mipmap-xxhdpi/ic_launcher.png    (144x144)
mipmap-xxxhdpi/ic_launcher.png   (192x192)

// ios/ProjectName/Images.xcassets/AppIcon.appiconset/
// Configured via Xcode or Contents.json
```

#### ⏰ Best Timing to Add Icons

**Recommendation**: **During Step 6 (Implementation)**, preferably:

1. **Project Start** (✅ IDEAL):
   - When creating initial folder structure
   - Before first commit
   - Facilitates visual identity from the beginning

2. **MVP/Prototype** (✅ GOOD):
   - After basic functionalities work
   - Before showing to users/clients
   - Ensures minimum professionalism

3. **Before Production** (⚠️ ACCEPTABLE):
   - During deployment preparation
   - Before publishing (App Store, Play Store, web)
   - Minimum necessary, but delayed

4. **❌ NEVER**: Leave for "later" without defined date

#### 📋 Icon Checklist (Validation)

```markdown
## Icon Checklist - Project [Name]

### Icons Created
- [ ] Main icon created/obtained (source: [specify])
- [ ] License verified (if downloaded from external source)
- [ ] Vector format available (SVG) or high-quality PNG source

### Necessary Formats
- [ ] **favicon.ico** (16x16, 32x32, 48x48 px)
- [ ] **icon.svg** (vector)
- [ ] **icon-192.png** (192x192 px) - PWA
- [ ] **icon-512.png** (512x512 px) - PWA
- [ ] **apple-touch-icon.png** (180x180 px) - iOS
- [ ] Other technology-specific formats

### Organization
- [ ] `assets/icons/` folder created
- [ ] All icons organized in correct folder
- [ ] No loose icons at project root

### Integration
- [ ] Icon referenced in HTML/main code
- [ ] manifest.json updated (if PWA)
- [ ] Tested in browser/application (icon appears)
- [ ] Documented in README (if third-party icon)

### Quality
- [ ] Icon has good resolution (not pixelated)
- [ ] Colors appropriate to project
- [ ] Visible on light AND dark backgrounds (if applicable)
- [ ] Recognizable at small sizes (16x16)
```

#### 🎯 Rationale: Why Icons Are Mandatory

1. **Professionalism**: Projects without icons appear incomplete/amateur
2. **Visual Identity**: Users recognize the app by its icon (branding)
3. **User Experience**: Icon helps locate the app among multiple tabs/windows
4. **Platform Requirements**: App stores (iOS/Android) REQUIRE icons
5. **PWA**: Browsers request icons for installation
6. **Organization**: Facilitates finding and managing visual assets
7. **Traceability**: Documenting source ensures license compliance

#### 🚨 Common Mistakes to Avoid

❌ **Don't**:
- Leave icon at project root (e.g., loose `favicon.ico`)
- Use low-resolution icon (pixelated when enlarged)
- Forget to reference in HTML/code
- Use copyrighted icon without permission
- Create only one size (browsers need multiple)

✅ **Do**:
- Organize in dedicated folder (`assets/icons/`)
- Generate multiple sizes (16, 32, 192, 512 px)
- Validate that icon appears correctly
- Document source if third-party icon
- Use vector format (SVG) when possible

#### 📚 Useful Resources

**Free Icon Generators** (online):
- [Favicon.io](https://favicon.io/) - Generates favicon from text/image/emoji
- [RealFaviconGenerator](https://realfavicongenerator.net/) - Generates all formats
- [Favicon Generator](https://www.favicon-generator.org/) - Simple and fast

**Free Icon Libraries**:
- [Heroicons](https://heroicons.com/) - MIT License
- [Lucide Icons](https://lucide.dev/) - ISC License
- [Tabler Icons](https://tabler-icons.io/) - MIT License
- [Iconoir](https://iconoir.com/) - MIT License
- [Bootstrap Icons](https://icons.getbootstrap.com/) - MIT License

**Conversion Tools**:
- [ImageMagick](https://imagemagick.org/) - Universal CLI
- [Pillow (Python)](https://pillow.readthedocs.io/) - Image library
- [Sharp (Node.js)](https://sharp.pixelplumbing.com/) - High performance

#### 📝 Example README Documentation

```markdown
## 🎨 Project Icon

**Source**: Created by AI using project initials  
**License**: Free to use (generated for this project)  
**Location**: `assets/icons/`

### Available Formats
- `icon.svg` - Vector (preferred)
- `favicon.ico` - Browsers (16, 32, 48 px)
- `icon-192.png` - PWA/Android
- `icon-512.png` - PWA/Android
- `apple-touch-icon.png` - iOS

### Colors
- Primary: `#4F46E5` (Indigo Blue)
- Text: `#FFFFFF` (White)
```

#### ⏱️ Estimated Time

- **Create simple icon (AI)**: 5-10 minutes
- **Download and adapt icon**: 10-15 minutes
- **Convert to necessary formats**: 5-10 minutes
- **Integrate into project**: 5-10 minutes
- **TOTAL**: 15-30 minutes

**Small investment, big impact on project quality perception.**

---

### 6️⃣.7️⃣ **Execution Scripts to Facilitate Usage** [RECOMMENDED]

> **RECOMMENDATION FOR AIs**: When dealing with an application or program written in a programming language that is executable, it's recommended to create batch scripts for Windows, Linux, and Mac accessible in the main folder or root directory, in order to facilitate application execution.

**When to Apply**: During implementation (Step 6), especially after setting up the basic structure of the executable project.

#### 📋 Context and Purpose

Execution scripts in the project root significantly facilitate application usage, especially:
- ✅ **Development**: Accelerates development cycle (run without manually configuring environment)
- ✅ **Onboarding**: New developers can run the project immediately
- ✅ **Testing**: Facilitates test execution and validation
- ✅ **Production**: In some cases, can simplify deployment (if there are no better alternatives like Docker, systemd, etc.)

#### 🎯 When to Create Execution Scripts

**✅ CREATE scripts IF:**
- ✅ Application is executable (not a library)
- ✅ Requires environment configuration (variables, paths, dependencies)
- ✅ Has multiple initialization commands
- ✅ Needs setup before execution (migrations, build, etc.)
- ✅ Team/users need to execute frequently

**❌ DO NOT create scripts IF:**
- ❌ Application already has well-documented native CLI
- ❌ Uses standard language tools (npm start, cargo run, etc.)
- ❌ Deployment uses orchestration (Docker, Kubernetes) - scripts stay in Dockerfile
- ❌ Project is a library/framework (not executable)

#### 📝 Recommended Folder Structure

```
project/
├── run.bat                 # ✅ Windows (main execution)
├── run.sh                  # ✅ Linux/Mac (main execution)
├── dev.bat                 # 🔄 Development Windows (optional)
├── dev.sh                  # 🔄 Development Linux/Mac (optional)
├── test.bat                # 🧪 Tests Windows (optional)
├── test.sh                 # 🧪 Tests Linux/Mac (optional)
├── build.bat               # 🏗️ Build Windows (optional)
├── build.sh                # 🏗️ Build Linux/Mac (optional)
└── README.md               # Script usage documentation
```

**Golden Rule**: Scripts in project root = easy access. Complex scripts can stay in `scripts/` with simple wrappers in root.

#### 💻 Script Examples by Language

##### **Python**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Execution script for Linux/Mac

# Colors for output
GREEN='\033[0;32m'
RED='\033[0;31m'
NC='\033[0m' # No Color

echo -e "${GREEN}🚀 Starting Python application...${NC}"

# Check if virtual environment exists
if [ ! -d "venv" ]; then
    echo -e "${RED}❌ Virtual environment not found. Creating...${NC}"
    python3 -m venv venv
fi

# Activate virtual environment
source venv/bin/activate

# Install/update dependencies
if [ -f "requirements.txt" ]; then
    echo -e "${GREEN}📦 Installing dependencies...${NC}"
    pip install -q -r requirements.txt
fi

# Run application
echo -e "${GREEN}✅ Running application...${NC}"
python src/main.py "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Execution script for Windows

echo 🚀 Starting Python application...

REM Check if virtual environment exists
if not exist "venv\" (
    echo ❌ Virtual environment not found. Creating...
    python -m venv venv
)

REM Activate virtual environment
call venv\Scripts\activate.bat

REM Install/update dependencies
if exist "requirements.txt" (
    echo 📦 Installing dependencies...
    pip install -q -r requirements.txt
)

REM Run application
echo ✅ Running application...
python src\main.py %*
```

##### **Node.js**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Execution script for Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Starting Node.js application...${NC}"

# Check if node_modules exists
if [ ! -d "node_modules" ]; then
    echo -e "${GREEN}📦 Installing dependencies...${NC}"
    npm install
fi

# Run application
echo -e "${GREEN}✅ Running application...${NC}"
npm start "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Execution script for Windows

echo 🚀 Starting Node.js application...

REM Check if node_modules exists
if not exist "node_modules\" (
    echo 📦 Installing dependencies...
    call npm install
)

REM Run application
echo ✅ Running application...
npm start %*
```

##### **Java**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Execution script for Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Starting Java application...${NC}"

# Compile if necessary
if [ ! -d "target" ]; then
    echo -e "${GREEN}🏗️ Compiling project...${NC}"
    mvn clean package -DskipTests
fi

# Run JAR
echo -e "${GREEN}✅ Running application...${NC}"
java -jar target/myapp.jar "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Execution script for Windows

echo 🚀 Starting Java application...

REM Compile if necessary
if not exist "target\" (
    echo 🏗️ Compiling project...
    call mvn clean package -DskipTests
)

REM Run JAR
echo ✅ Running application...
java -jar target\myapp.jar %*
```

##### **Go**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Execution script for Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Starting Go application...${NC}"

# Download dependencies if necessary
if [ ! -f "go.sum" ]; then
    echo -e "${GREEN}📦 Downloading dependencies...${NC}"
    go mod download
fi

# Run application
echo -e "${GREEN}✅ Running application...${NC}"
go run cmd/main.go "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Execution script for Windows

echo 🚀 Starting Go application...

REM Download dependencies if necessary
if not exist "go.sum" (
    echo 📦 Downloading dependencies...
    go mod download
)

REM Run application
echo ✅ Running application...
go run cmd\main.go %*
```

##### **Rust**

**run.sh (Linux/Mac)**:
```bash
#!/bin/bash
# Execution script for Linux/Mac

GREEN='\033[0;32m'
NC='\033[0m'

echo -e "${GREEN}🚀 Starting Rust application...${NC}"

# Compile and run
echo -e "${GREEN}✅ Running application (cargo run)...${NC}"
cargo run --release "$@"
```

**run.bat (Windows)**:
```batch
@echo off
REM Execution script for Windows

echo 🚀 Starting Rust application...

REM Compile and run
echo ✅ Running application (cargo run)...
cargo run --release %*
```

#### 🔧 Additional Useful Scripts

##### **Development Script** (watch/reload mode)

**dev.sh**:
```bash
#!/bin/bash
# Development mode with auto-reload

echo "🔄 Starting in development mode..."

# Python
# pip install watchdog
# watchmedo auto-restart --directory=./src --pattern=*.py python src/main.py

# Node.js
# npm run dev  # nodemon or similar

# Go
# go install github.com/cosmtrek/air@latest
# air

# Rust
# cargo install cargo-watch
# cargo watch -x run
```

##### **Test Script**

**test.sh**:
```bash
#!/bin/bash
# Run tests

echo "🧪 Running tests..."

# Python
# pytest tests/ -v

# Node.js
# npm test

# Java
# mvn test

# Go
# go test ./...

# Rust
# cargo test
```

#### 📋 Execution Scripts Checklist

```markdown
## Scripts Checklist - Project [Name]

### Scripts Created
- [ ] **run.sh** (Linux/Mac) - Main execution script
- [ ] **run.bat** (Windows) - Main execution script
- [ ] Execution permissions configured (`chmod +x *.sh`)
- [ ] Scripts tested on each platform

### Optional Scripts (as needed)
- [ ] **dev.sh/dev.bat** - Development mode with auto-reload
- [ ] **test.sh/test.bat** - Run automated tests
- [ ] **build.sh/build.bat** - Compile/build project
- [ ] **install.sh/install.bat** - Install dependencies
- [ ] **clean.sh/clean.bat** - Clean build artifacts

### Documentation
- [ ] README.md updated with script usage instructions
- [ ] Usage examples documented
- [ ] System requirements documented (Python 3.9+, Node 18+, etc.)
- [ ] Basic troubleshooting included

### Script Features
- [ ] Check if dependencies are installed
- [ ] Create virtual environment/directories if needed
- [ ] Clear and informative output messages
- [ ] Support argument passing (`./run.sh --help`)
- [ ] Handle errors gracefully
- [ ] Include colors in output (optional, improves UX)
```

#### 📝 Example README Documentation

```markdown
## 🚀 How to Run

### Requirements
- Python 3.9+ (or Node.js 18+, Java 17+, etc.)
- Git

### Quick Start

**Linux/Mac**:
```bash
./run.sh
```

**Windows**:
```batch
run.bat
```

### Available Scripts

| Script | Description | Platform |
|--------|-------------|----------|
| `run.sh` / `run.bat` | Runs the main application | Linux/Mac / Windows |
| `dev.sh` / `dev.bat` | Development mode (auto-reload) | Linux/Mac / Windows |
| `test.sh` / `test.bat` | Runs automated tests | Linux/Mac / Windows |
| `build.sh` / `build.bat` | Compiles/builds the project | Linux/Mac / Windows |

### Arguments

Pass arguments to application:
```bash
./run.sh --port 8080 --debug
```

### Troubleshooting

**Error: Permission denied (Linux/Mac)**
```bash
chmod +x run.sh dev.sh test.sh build.sh
```

**Error: Dependencies not found**
- Scripts automatically install dependencies on first run
- If it fails, run manually: `pip install -r requirements.txt` (Python) or `npm install` (Node.js)
```

#### ⏱️ Estimated Time

- **Create basic scripts (run.sh/run.bat)**: 10-15 minutes
- **Add optional scripts (dev, test, build)**: 5-10 minutes each
- **Document in README**: 10-15 minutes
- **Test on multiple platforms**: 10-20 minutes
- **TOTAL**: 30-60 minutes

**Investment: ~30-60 minutes. Benefit: Saves hours of setup for each developer and user.**

#### 🎯 Rationale: Why Execution Scripts Are Important

1. **Developer Experience (DX)**: New developer clones repo, runs `./run.sh` and application works
2. **Friction Reduction**: No need to read complex documentation to run project
3. **Consistency**: Everyone runs the same way, reduces "works on my machine"
4. **Automation**: Scripts can automatically configure environment (create venv, install deps)
5. **Living Documentation**: Scripts serve as executable documentation of initialization process
6. **Onboarding**: Accelerates entry of new team members
7. **CI/CD**: Scripts can be reused in pipelines
8. **Cross-Platform**: Explicit support for Windows, Linux, and Mac

#### ⚠️ When NOT to Use Root Scripts

**Use better alternatives when available:**
- 🐳 **Docker/Docker Compose**: For apps with multiple dependencies (databases, queues, etc.)
- 📦 **Native Package Managers**: `npm start`, `cargo run`, `go run` are already sufficient
- 🎯 **Task Runners**: Makefile, Just, Task for complex projects
- ☸️ **Orchestration**: Kubernetes, systemd for enterprise production

**Recommended Combination**:
```
project/
├── docker-compose.yml      # 🐳 For complete environment
├── Makefile                # 🎯 For complex commands
├── run.sh                  # ✅ Simple wrapper that calls Make/Docker
└── README.md               # 📚 Documents when to use each one
```

**Wrapper example**:
```bash
#!/bin/bash
# run.sh - Simple wrapper

if command -v docker &> /dev/null; then
    echo "🐳 Docker detected, using docker-compose..."
    docker-compose up
else
    echo "⚠️ Docker not found, running locally..."
    make run
fi
```

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
git add project_app.py
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
python project_app.py --export tasks.csv
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
python project_app.py --test

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
python -m cProfile -s cumulative project_app.py > profile.txt

# Profiling with visualization
pip install snakeviz
python -m cProfile -o profile.stats project_app.py
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
# python -m memory_profiler project_app.py
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
# kernprof -l -v project_app.py
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
py-spy record -o profile.svg -- python project_app.py
# Generates interactive flamegraph

# Scalene - CPU + Memory + GPU profiler
pip install scalene
scalene project_app.py
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
        black --check project_app.py
      continue-on-error: false
    
    - name: Linting (Flake8)
      run: |
        flake8 project_app.py --max-line-length=88 --statistics
      continue-on-error: false
    
    - name: Type Checking (MyPy)
      run: |
        mypy project_app.py --ignore-missing-imports
      continue-on-error: true  # Warnings, not errors
    
    - name: Security Scan (Bandit)
      run: |
        bandit -r project_app.py -ll
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
    - black --check project_app.py
  allow_failure: false

lint:flake8:
  stage: lint
  image: python:3.11
  script:
    - pip install flake8
    - flake8 project_app.py --max-line-length=88 --statistics
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
    - bandit -r project_app.py -f data -o bandit-report.data
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
        ["flake8", "project_app.py", "--statistics"],
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
        ["mypy", "project_app.py", "--data-report", ".mypy"],
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
# MyProject - Task Management

[![CI Status](https://github.com/user/myproject/workflows/CI/badge.svg)](https://github.com/user/myproject/actions)
[![Coverage](https://codecov.io/gh/user/myproject/branch/main/graph/badge.svg)](https://codecov.io/gh/user/myproject)
[![Quality Gate](https://sonarcloud.io/api/project_badges/measure?project=myproject&metric=alert_status)](https://sonarcloud.io/dashboard?id=myproject)
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
- **CRITICAL**: Before documentation and commit, **organize the root folder recursively**
- **MANDATORY**: Files must be organized in the correct folders before commit
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

2. **Directory Structure Verification (MANDATORY)**:
   - `src/` - source code
   - `tests/` - **ALL test files** (mandatory)
   - `docs/` - **ALL documents and markdown files** (mandatory)
   - Organized root files (README, setup.py, etc.)

3. **Mandatory Recursive Organization**:
   
   **⚠️ FUNDAMENTAL RULE**: 
   > Before commit, files must be organized in folders recursively. This is **mandatory** to keep the environment clean and organized.

   **Specific Rules by File Type**:
   
   a) **Test Files** → `tests/`
      - ✅ `test_*.py`, `*_test.py` → `tests/`
      - ✅ Test structure should mirror code structure
      - ✅ Example: `tests/unit/`, `tests/integration/`, `tests/fixtures/`
   
   b) **Documents and Markdown** → `docs/`
      - ✅ All `.md` files (except root README.md) → `docs/`
      - ✅ Documentation files → `docs/`
      - ✅ **Recursive organization within `docs/`**:
        - `docs/api/` - API documentation
        - `docs/tutorials/` - Tutorials
        - `docs/architecture/` - Architectural decisions (ADRs)
        - `docs/user-guide/` - User guides
        - `docs/dev-guide/` - Development guides
        - `docs/adr/` - Architecture Decision Records (see Step 11.5)
      - ✅ Create subfolders that identify file context
   
   c) **Source Code** → `src/` or appropriate folder
      - ✅ Organize by modules/features
      - ✅ Example: `src/core/`, `src/utils/`, `src/api/`

**Complete Example**:
```bash
# BEFORE (disorganized):
├── src/
├── test_utils.py              ❌ test outside tests/
├── API_DOCS.md                ❌ doc outside docs/
├── tutorial.md                ❌ doc outside docs/
├── apply_v2913_patches.py     ❌ temporary
├── test_temp.py               ❌ temporary test
├── backup_old/                ❌ old backup
├── __pycache__/               ❌ cache
└── file.py.backup_v2913       ❌ unnecessary backup

# AFTER (recursively organized):
├── src/
│   ├── core/
│   └── utils/
├── tests/                     ✅ ALL tests
│   ├── unit/
│   │   └── test_utils.py     ✅ test moved
│   └── integration/
├── docs/                      ✅ ALL documents
│   ├── api/
│   │   └── API_DOCS.md       ✅ doc moved
│   ├── tutorials/
│   │   └── tutorial.md       ✅ doc moved
│   └── adr/                   ✅ ADRs organized
└── README.md                  ✅ root README kept
```

**Why?**: Keep repository clean, avoid committing garbage, facilitate navigation, professionalism, recursive organization ensures scalability. Document the **clean** and **organized** state of the project.

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
- Create `ProjectGUI` class with QMainWindow
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
myproject/
├── docs/
│   ├── adr/
│   │   ├── 001-choice-of-pyqt6.md
│   │   ├── 002-data-storage-format.md
│   │   ├── 003-simplicity-protocol-versioning.md
│   │   └── README.md  (ADR Index)
│   ├── PROTOCOLO_SIMPLICIDADE_1.md
│   └── PROTOCOLO_SIMPLICIDADE_2.md
├── project_app.py
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

---

### ⚠️ **MANDATORY REQUIREMENT: Complete Documentation of All AI Implementations**

> **CRITICAL FOR AIs**: Everything that the artificial intelligence does in the project, in each implementation cycle, in each code, each implemented functionality, **MUST BE DOCUMENTED IN THE `docs/` FOLDER AS A MANDATORY REQUIREMENT** to mark new functionalities and new behaviors.

**📖 See SIMPLICITY_PROTOCOL_1.md. - Step 12** for complete documentation requirements, templates, and validation checklists.

#### **🏢 Enterprise-Specific Documentation (Simplicity 2)**

In addition to base documentation requirements, Simplicity 2 adds:

**Additional Documentation for Enterprise**:
- ✅ **ADRs** (Architecture Decision Records) - Formal documentation in `docs/ADR/`
- ✅ **OWASP Security Checklist** - Complete and documented in `docs/SECURITY.md`
- ✅ **WCAG Accessibility Checklist** - For GUI applications in `docs/ACCESSIBILITY.md`
- ✅ **API Documentation** - Generated with Sphinx/pdoc in `docs/API/`
- ✅ **Performance Profiling Results** - For critical features
- ✅ **Code Review Records** - Approvals and feedback documented

**📂 Enterprise Documentation Structure**:

```
docs/
├── REQUIREMENTS.md
├── vX.Y.Z-SPECIFICATIONS.md
├── CHANGELOG.md
├── ARCHITECTURE.md
├── ADR/                     # Architecture Decision Records
│   ├── ADR-001-[decision].md
│   └── ADR-002-[decision].md
├── SECURITY.md              # OWASP checklist and mitigations
├── ACCESSIBILITY.md         # WCAG compliance (if GUI)
├── API/                     # API documentation
│   └── api-reference.html   # Generated by Sphinx/pdoc
├── CODE_REVIEWS/            # Code review records
│   └── review-vX.Y.Z.md
└── [feature]-GUIDE.md
```

**🔍 Additional Validation for Enterprise**:

Before commit, AI must also verify:
- [ ] ✅ ADRs created for important architectural decisions
- [ ] ✅ OWASP security checklist complete in SECURITY.md
- [ ] ✅ Profiling results documented (if critical feature)
- [ ] ✅ API documentation generated (if public library)
- [ ] ✅ Code review approved and documented
- [ ] ✅ WCAG checklist complete (if GUI application)

**Rationale for Enterprise**: In large teams and regulated environments, comprehensive documentation is essential for compliance, auditing, team collaboration, and organizational knowledge preservation.

---

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

---

### 📊 **Task Classification Legend (Simplicity 2)**

**Objective**: Standardize task classification and prioritization to facilitate AI organization, team communication, and understanding between different artificial intelligence systems.

**Note for Simplicity 2**: In enterprise environments with large teams, task classification should be **integrated with the Decision Matrix (Step 2.5)** to ensure objective and traceable choices.

#### **Task Status**

- 🔴 **Not Started** - Awaiting start, no work done
- 🟡 **In Progress** - Active development, work underway
- 🟢 **Done** - Implemented, tested, peer-reviewed and completed
- 🔵 **Blocked** - Impeded by external dependency or technical issue

#### **Task Complexity**

- 🟢 **Simple** (0-1h) - Low risk, few dependencies, clear scope
- 🟡 **Medium** (1-2h) - Medium risk, some integrations, may require additional tests
- 🔴 **Complex** (>2h) - High risk, many dependencies, open or ambiguous scope

#### **MoSCoW Prioritization**

- 🔴 **Must Have** - Critical for system functionality, release blocker
- 🟡 **Should Have** - Important but not blocking, can be postponed if needed
- 🟢 **Could Have** - Desirable if time permits, low priority
- ⚪ **Won't Have** (Later) - Explicitly out of current scope, for future versions

#### **Integration with Decision Matrix (Simplicity 2)**

The Decision Matrix (Step 2.5) provides numerical scoring (0-35 points) complementary to visual indicators:

```markdown
## Sprint v3.2 - Prioritized Backlog

### 🔴 MUST HAVE

| Task | Status | Complex. | Score | Order |
|------|--------|----------|-------|-------|
| #42 2FA Auth | 🔴 | 🔴 | 25.0 | 3rd |
| #43 Rate Limiting | 🔴 | 🟡 | 28.5 | 2nd |
| #44 Logging | 🔴 | 🟢 | 33.5 | 1st ⭐ START HERE |

**Justification**: Task #44 has highest score (33.5) despite being Must Have like others.
Starting with it reduces risks and allows team to warm up before complex tasks.
```

**Combining Decision Matrix + Visual Classification**:
1. Use **Decision Matrix** for objective scoring (5 numerical criteria)
2. Use **Visual Indicators** (🔴🟡🟢🔵) for quick status in backlog
3. Use **MoSCoW** to define release scope
4. Use **Complexity** to balance sprints (not only difficult tasks)

#### **Advanced Prioritization Frameworks**

For enterprise teams that need to justify decisions to stakeholders:

##### **RICE Matrix** (Quantitative)

`RICE Score = (Reach × Impact × Confidence) / Effort`

Useful for:
- ✅ Product management decisions with multiple competing features
- ✅ Presentations to C-level (objective data)
- ✅ Long-term roadmap planning

**Enterprise Example**:
```markdown
| Feature | Reach | Impact | Conf. | Effort | RICE | Decision |
|---------|-------|--------|-------|--------|------|----------|
| SSO Integration | 5000 | 3 | 80% | 80h | 150 | Q1 2024 |
| Dashboard v2 | 2000 | 2 | 100% | 40h | 100 | Q2 2024 |
| Dark Mode | 8000 | 0.5 | 100% | 20h | 200 | Q1 2024 ⭐ |

Decision: Prioritize Dark Mode (RICE=200) over SSO (RICE=150)
Reason: Greater reach with less effort, despite lower individual impact
```

##### **Eisenhower Matrix** (Urgency × Importance)

Useful for:
- ✅ Incident and crisis management
- ✅ Prioritization in contexts with many false "urgencies"
- ✅ Identifying tasks to delegate or automate

**Team Adaptation**:
- **Q1 (Urgent + Important)**: Senior team / Tech leads
- **Q2 (Not Urgent + Important)**: Mid-level team, planned
- **Q3 (Urgent + Not Important)**: Delegate to junior or automate
- **Q4 (Not Urgent + Not Important)**: Eliminate or distant backlog

#### **Complete Simplicity 2 Example**

```markdown
# TASKS.md - Sprint v4.1 (Enterprise Team)

## 📊 Legend
- **Status**: 🔴 Not Started | 🟡 In Progress | 🟢 Done | 🔵 Blocked
- **Complexity**: 🟢 Simple (0-1h) | 🟡 Medium (1-2h) | 🔴 Complex (>2h)
- **MoSCoW**: 🔴 Must | 🟡 Should | 🟢 Could | ⚪ Won't

## 📊 Statistics
- Progress: 65% (26/40 tasks)
- Velocity: 12 story points/sprint
- Open Bugs: 3 (1 critical, 2 medium)

## 🔴 MUST HAVE - Release v4.1

### High Priority (Matrix Score > 25)
- 🔴🟢 [ ] #101 Add rate limiting (Score: 33.5) ⭐ START
  - **Assignee**: @maria (Backend Lead)
  - **Review**: @joao (Security Review required)
  - **Estimate**: 3h
  - **Dependencies**: None
  
- 🟡🟡 [ ] #102 Implement circuit breaker (Score: 28.0, 60% complete)
  - **Assignee**: @pedro (Mid-level)
  - **Review**: @maria (Code Review)
  - **Estimate**: 5h (2h remaining)
  - **Blocker Resolved**: ✅ Library updated to v3.2

### Medium Priority (Matrix Score 15-25)
- 🔵🔴 [ ] #103 Migrate to Kubernetes (Score: 22.0, BLOCKED)
  - **Assignee**: @infra-team
  - **Blocker**: Awaiting DevOps budget approval
  - **Estimate**: 16h
  - **Fallback**: Keep Docker Swarm for 1 more sprint

## 🟡 SHOULD HAVE - Release v4.2
- 🔴🟡 [ ] #104 Add Prometheus metrics (Score: 26.5)
- 🔴🟢 [ ] #105 Help tooltips (Score: 30.0)

## 🟢 COULD HAVE - Backlog
- 🔴🟡 [ ] #106 Dark mode (RICE: 200, high backlog priority)

---
**Next Retrospective**: Friday 3pm (validate AI recommendations)
```

#### **Recommendations for AI in Enterprise Context**

**When classifying tasks for teams (Simplicity 2), AI should**:
1. ✅ **Consider Code Review**: Complex tasks need available senior reviewer
2. ✅ **Balance workload**: Don't allocate all complex tasks to same person
3. ✅ **Respect team dependencies**: Backend before Frontend in integrations
4. ✅ **Document decisions**: Use ADR (Step 11.5) for important architectural choices
5. ✅ **Communicate blockers**: Mark 🔵 and notify team immediately
6. ✅ **Integrate with Decision Matrix**: Scoring + visual indicators complementary
7. ✅ **Validate with stakeholders**: MUST HAVE features confirmed in Sprint Planning

**Simplicity 2 vs 1 Differences**:
- **S2**: Decision Matrix (numerical scoring) is **MANDATORY** when 3+ tasks compete
- **S2**: Status should reflect **code review** (don't mark Done without peer approval)
- **S2**: AI recommendations validated in **Sprint Retrospective** (Step 13.5)
- **S2**: Complexity includes **review time** and **acceptance testing**

---

**🤖 AI Task Recommendations**:
For enterprise teams (Simplicity 2), AI recommendations should be **reviewed in sprint retrospectives** (Step 13.5) before being added to TASKS.md. This ensures team consensus and alignment with stakeholders.

📘 **Complete details of recommendation functionality**: See `SIMPLICITY_PROTOCOL_1.md` - Step 12 - Section "AI Task Recommendations"

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
# MyProject v2.9.X - [Descriptive Name]

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
   cp ~/.config/myproject/myproject.db ~/.config/myproject/myproject.db.backup-$(date +%s)
   
   # Backup logs
   cp ~/.config/myproject/myproject.log /tmp/myproject-rollback-logs.txt
   ```

3. **Verify DATA backup available**:
   ```bash
   # Confirm DATA backup exists (created during migration)
   ls -lh ~/.config/myproject/tasks.data.backup
   # Should show file created during migration to v2.0.0
   ```

### Phase 2: Rollback (10 minutes)
1. **Revert code to previous version**:
   ```bash
   cd ~/myproject
   git checkout v1.9.5  # Tag of previous stable version
   
   # OR if in production via package manager
   pip install myproject==1.9.5 --force-reinstall
   ```

2. **Restore data from DATA backup**:
   ```bash
   # Copy DATA backup back
   cp ~/.config/myproject/tasks.data.backup ~/.config/myproject/tasks.data
   
   # Remove SQLite database (v1.9.5 does not use)
   rm ~/.config/myproject/myproject.db
   ```

3. **Verify data integrity**:
   ```bash
   # Validate DATA is not corrupted
   python -c "import data; data.load(open('~/.config/myproject/tasks.data'))"
   # Should complete without error
   
   # Count tasks
   python -c "import data; data = data.load(open('~/.config/myproject/tasks.data')); print(f'{len(data[\"tasks\"])} tasks restored')"
   ```

4. **Restart application**:
   ```bash
   # If process running, kill
   kill <myproject_pid>
   
   # Start v1.9.5
   python myproject.py
   ```

### Phase 3: Validation (5 minutes)
1. **Smoke Tests**:
   ```bash
   # Test 1: App starts without crash
   myproject --version
   # Expected: v1.9.5
   
   # Test 2: List tasks
   myproject list
   # Expected: Tasks displayed correctly
   
   # Test 3: Add task
   myproject add "Test rollback task"
   # Expected: Task added without error
   
   # Test 4: GUI opens (if applicable)
   myproject --gui &
   # Expected: GUI opens without crash
   ```

2. **Check logs**:
   ```bash
   tail -n 50 ~/.config/myproject/myproject.log
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
   pip install myproject==1.9.5 --force-reinstall
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
conn = sqlite3.connect('~/.config/myproject/myproject.db')
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
    SQLITE_STORAGE_ENABLED = os.getenv("MYPROJECT_SQLITE_ENABLED", "true").lower() == "true"
    
    def get_storage_backend(self):
        """Get storage backend based on feature flag."""
        if self.SQLITE_STORAGE_ENABLED:
            return SQLiteStorage()
        else:
            return DATAStorage()  # Safe fallback

# In case of problem, disable remotely:
# export MYPROJECT_SQLITE_ENABLED=false
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
        os.remove("myproject.db")
        
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
- **Format**: Conventional Commits (MANDATORY)
- **Language**: All commit messages must be **EXCLUSIVELY IN ENGLISH** (mandatory requirement)
- **Message**: Descriptive, complete, with context
- **Frequency**: 1 commit per task or logical group of changes

**Standardized Commit Types** (MANDATORY):
- `feat`: Indicates a new feature
  - Example: `git commit -m "feat: add Header component"`
- `fix`: Indicates a bug fix
  - Example: `git commit -m "fix: remove wrong prop in Header"`
- `refactor`: Indicates code refactoring
  - Example: `git commit -m "refactor: add title in Header"`
- `test`: Indicates test changes
  - Example: `git commit -m "test: add test in title Header"`
- `style`: Indicates style/formatting changes
  - Example: `git commit -m "style: add Header title background"`
- `docs`: Indicates documentation changes
  - Example: `git commit -m "docs: add get started in readme"`
- `chore`: Indicates development environment changes
  - Example: `git commit -m "chore: change eslint rules"`
- `build`: Indicates dependency changes
  - Example: `git commit -m "build: add sass"`
- `revert`: Indicates reversion of a previous commit
  - Example: `git commit -m "revert: back to adc1234 commit"`

⚠️ **IMPORTANT**: All commit messages must be written **EXCLUSIVELY IN ENGLISH**!

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
# Sprint Retrospective #5 - MyProject

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

## 📊 Ordinal Task Organization - Simplicity Protocols

**Version**: 1.0  
**Creation Date**: December 27, 2025  
**Author**: Josué Amaral  
**Status**: ACTIVE

---

### 🎯 Objective

This document defines the **Ordinal Task Organization** system for the Simplicity Protocols, allowing human developers and artificial intelligences to quickly identify:

- ✅ **Execution order** of tasks (from simplest to most complex)
- ✅ **Dependencies** between tasks (which must be done first)
- ✅ **Parallelization** (which can be executed simultaneously)
- ✅ **Hierarchical organization** (tree/graph structure)

---

### 📊 Ordinal Prefix System

#### Level 1: Simple Numbering (Independent Tasks)

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

#### Level 2: Hierarchy with Letters (Task Groups)

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

#### Level 3: Deep Hierarchy (Complex Dependencies)

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

### 🌳 Tree/Graph Structure

#### Fundamental Concepts

**1. Parent and Child Nodes**

```
B.C.2 (PARENT - execute AFTER)
   ├── B.C.2.1 (CHILD - execute BEFORE)
   └── B.C.2.2 (CHILD - execute BEFORE)
```

**Rule**: 
- ✅ **Children must be completed BEFORE parent**
- ✅ Children are **prerequisites** for parent
- ✅ Parent **depends** on children

**2. Siblings (Parallel)**

```
B.C.2.1 (sibling)
B.C.2.2 (sibling)
```

**Rule**:
- ✅ Siblings can be executed **in parallel**
- ✅ No dependency between them
- ✅ Can be in **separate branches**

**3. Cousins, Uncles, Grandparents (Parallel vs Serial)**

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

### 🔄 Parallelization vs Serialization

#### PARALLEL Tasks (can be simultaneous)

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

#### SERIAL Tasks (must be sequential)

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

### 🎯 Integration with Existing Classification System

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

### 🤖 Instructions for Artificial Intelligences

**When to Suggest Ordinal Organization**

AI should suggest ordinal organization when:

✅ **Project has >10 tasks** with interdependencies
✅ **Multiple developers** working simultaneously
✅ **Blocking tasks** (one depends on another)
✅ **Risk of conflicts** in version control
✅ **Need for parallelization** to speed up development

**How AI Should Apply**

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

---

## 🌳 Tree Imports Analogy

**Author:** Josué Amaral  
**Date:** December 24, 2025  
**Context:** Phase 3.0 - Refactoring Architecture  
**Applicable to:** All programming languages

---

### 📚 Overview

This document describes the **Tree Imports Analogy**, a mental model for understanding and organizing the dependency architecture in software projects. This analogy is applicable to any programming language that supports module importing/inclusion.

---

### 🌳 The Imports Tree

#### Fundamental Concept

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

#### Tree Elements

**🌲 Root**
- **Main File** (e.g., `app.py`, `main.py`, `index.js`)
- **Characteristics:**
  - Most complex and encapsulated
  - System orchestrator
  - Imports multiple project modules
  - Contains coordination logic between components
  - Decides "what" to do, delegating "how" to do it

**🌿 Branches**
- **Intermediate Modules** (e.g., `gui/`, `core/`, `utils/`)
- **Characteristics:**
  - Medium complexity
  - Import other project modules
  - Provide specialized functionality
  - Abstract implementation details

**🍃 Leaves**
- **Terminal Modules** (e.g., `button.py`, `validator.py`, `helpers.py`)
- **Characteristics:**
  - Simpler and more specific
  - **DO NOT import** files from the project itself
  - **DO import** external libraries (Numpy, Pandas, etc.)
  - Provide atomic functionality
  - Are reusable and independently testable

---

### 📊 Practical Example

#### Hierarchical Structure

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

#### Characteristics by Level

| Level | File | Imports Project | Imports External | Complexity | Role |
|-------|------|-----------------|------------------|------------|------|
| 0 (Root) | A | B, C | Rarely | High | Orchestrator |
| 1 (Branch) | B, C | D, E, F, G | Sometimes | Medium | Coordinator |
| 2 (Leaf) | D, E, F, G | ❌ Never | ✅ Always | Low | Executor |

---

### 🔄 Development Approaches

#### 🔽 Top-Down (From Top to Bottom)

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

---

#### 🔼 Bottom-Up (From Bottom to Top)

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

---

#### ↔️ Middle-Out (From Middle Outward)

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

---

### 🎯 Design Principles

#### 1. **Depth Principle**

> "The closer to the root, the more complex and orchestrating.  
> The closer to the leaves, the simpler and executing."

```
Root (A):     if condition: B.do() else: C.do()  ← Decision
Branch (B):   return D.compute(E.prepare(data))  ← Coordination
Leaf (D):     return sum(numbers) / len(numbers) ← Execution
```

#### 2. **Independence Principle**

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

#### 3. **Single Responsibility Principle**

> "Each level has its distinct role."

| Level | Responsibility | Question it Answers |
|-------|----------------|---------------------|
| Root | Orchestration | "What does the system do?" |
| Branch | Coordination | "How do the parts connect?" |
| Leaf | Execution | "How to do X specifically?" |

---

### 📏 Quality Metrics

#### Good Architecture Indicators

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

#### Problem Indicators

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

### 📖 Conclusion of Sections

The **Ordinal Task Organization** and **Tree Imports Analogy** provide powerful mental models for:

1. **Organizing** tasks from simplest to most complex
2. **Understanding** existing architecture
3. **Planning** new modules
4. **Refactoring** code organically
5. **Parallelizing** development to accelerate deliveries
6. **Communicating** design decisions clearly

---

## 💡 Programming Best Practices for AI

> **This section contains specific recommendations to improve the quality of code generated by artificial intelligences.**

### 1. 📖 **Readable and Self-Documenting Code**

**Why it matters**: AIs should produce code that humans can easily understand and maintain.

**Practices**:
- ✅ **Descriptive names**: Use names that explain the purpose
  ```python
  # ❌ BAD
  def proc(d, x):
      return d[x] if x in d else None
  
  # ✅ GOOD
  def get_user_preference(preferences_dict, preference_key):
      """Returns user preference or None if it doesn't exist."""
      return preferences_dict.get(preference_key)
  ```

- ✅ **Small and focused functions**: One function = one responsibility
  ```python
  # ❌ BAD - Function does multiple things
  def process_user_data(user):
      # validates
      # transforms
      # saves to database
      # sends email
      # logs
      pass  # 150 lines
  
  # ✅ GOOD - Specialized functions
  def validate_user_data(user): pass
  def transform_user_data(user): pass
  def save_user_to_database(user): pass
  def send_welcome_email(user): pass
  def log_user_registration(user): pass
  ```

- ✅ **Avoid "magic numbers"**: Use named constants
  ```python
  # ❌ BAD
  if user.age > 18 and balance < 1000:
      apply_fee(balance * 0.05)
  
  # ✅ GOOD
  MINIMUM_ADULT_AGE = 18
  BALANCE_THRESHOLD = 1000
  SERVICE_FEE_RATE = 0.05
  
  if user.age > MINIMUM_ADULT_AGE and balance < BALANCE_THRESHOLD:
      apply_fee(balance * SERVICE_FEE_RATE)
  ```

### 2. 🎯 **Consistent Naming Conventions**

**Why it matters**: Consistency facilitates navigation and code comprehension.

**Practices by language**:

**Python**:
- ✅ `snake_case` for functions and variables
- ✅ `PascalCase` for classes
- ✅ `SCREAMING_SNAKE_CASE` for constants
- ✅ `_private_method` for private methods

**JavaScript/TypeScript**:
- ✅ `camelCase` for functions and variables
- ✅ `PascalCase` for classes and components
- ✅ `SCREAMING_SNAKE_CASE` for constants
- ✅ `_privateMethod` or `#privateField` for private

**General conventions**:
- ✅ Verbs for functions: `get_user()`, `calculate_total()`, `validate_input()`
- ✅ Nouns for classes: `UserManager`, `PaymentProcessor`
- ✅ Booleans with prefixes: `is_valid`, `has_permission`, `can_edit`

### 3. 🛡️ **Robust Error Handling**

**Why it matters**: Production code must gracefully handle failures.

**Practices**:
- ✅ **Always validate input**:
  ```python
  def divide(a, b):
      if not isinstance(a, (int, float)) or not isinstance(b, (int, float)):
          raise TypeError("Arguments must be numbers")
      if b == 0:
          raise ValueError("Divisor cannot be zero")
      return a / b
  ```

- ✅ **Use specific exceptions**:
  ```python
  # ❌ BAD - Generic exception
  try:
      process_payment(amount)
  except Exception as e:
      print("Error")
  
  # ✅ GOOD - Specific exceptions
  try:
      process_payment(amount)
  except PaymentDeclinedError as e:
      notify_user("Payment declined")
  except InsufficientFundsError as e:
      notify_user("Insufficient funds")
  except NetworkError as e:
      retry_payment(amount)
  ```

- ✅ **Adequate logging**:
  ```python
  import logging
  
  try:
      result = risky_operation()
  except Exception as e:
      logging.error(f"Failed in risky_operation: {e}", exc_info=True)
      raise  # Re-raise to allow handling at higher level
  ```

### 4. 🧪 **Effective Testing Strategies**

**Why it matters**: Tests ensure code works and continues working.

**Practices**:
- ✅ **Unit tests for business logic**:
  ```python
  def test_calculate_discount():
      # Arrange
      original_price = 100
      discount_rate = 0.2
      
      # Act
      final_price = calculate_discount(original_price, discount_rate)
      
      # Assert
      assert final_price == 80
  ```

- ✅ **Test edge cases**:
  ```python
  def test_edge_cases():
      assert calculate_discount(0, 0.5) == 0  # Zero price
      assert calculate_discount(100, 0) == 100  # Zero discount
      assert calculate_discount(100, 1.0) == 0  # 100% discount
      
      with pytest.raises(ValueError):
          calculate_discount(100, -0.1)  # Negative discount
      
      with pytest.raises(ValueError):
          calculate_discount(-100, 0.1)  # Negative price
  ```

- ✅ **Mocks for external dependencies**:
  ```python
  from unittest.mock import Mock, patch
  
  def test_send_notification():
      with patch('email_service.send') as mock_send:
          notify_user("user@example.com", "Test message")
          mock_send.assert_called_once()
  ```

### 5. 🔒 **Security First**

**Why it matters**: Vulnerabilities can have serious consequences.

**Practices**:
- ✅ **Never trust user input**:
  ```python
  # ❌ BAD - SQL Injection
  query = f"SELECT * FROM users WHERE id = {user_id}"
  
  # ✅ GOOD - Parameterization
  query = "SELECT * FROM users WHERE id = ?"
  cursor.execute(query, (user_id,))
  ```

- ✅ **Secrets in environment variables**:
  ```python
  # ❌ BAD
  API_KEY = "sk-1234567890abcdef"  # Hardcoded
  
  # ✅ GOOD
  import os
  API_KEY = os.getenv('API_KEY')
  if not API_KEY:
      raise ValueError("API_KEY not configured")
  ```

- ✅ **Sanitize output to prevent XSS**:
  ```python
  from html import escape
  
  # ❌ BAD
  html = f"<div>Hello {user_name}</div>"
  
  # ✅ GOOD
  html = f"<div>Hello {escape(user_name)}</div>"
  ```

### 6. ⚡ **Performance Optimization**

**Why it matters**: Slow code = unhappy users.

**Practices**:
- ✅ **Choose correct data structure**:
  ```python
  # ❌ BAD - List search O(n)
  if user_id in user_list:  # 1000 comparisons
      # ...
  
  # ✅ GOOD - Set search O(1)
  if user_id in user_set:  # 1 comparison
      # ...
  ```

- ✅ **Avoid unnecessary loops**:
  ```python
  # ❌ BAD - Double loop O(n²)
  for item in list1:
      for item2 in list2:
          if item == item2:
              # ...
  
  # ✅ GOOD - Set intersection O(n)
  common_items = set(list1) & set(list2)
  for item in common_items:
      # ...
  ```

- ✅ **Lazy loading when appropriate**:
  ```python
  # ❌ BAD - Load everything into memory
  all_users = User.objects.all()  # 1 million records
  for user in all_users:
      process(user)
  
  # ✅ GOOD - Iterator that loads on demand
  for user in User.objects.iterator():
      process(user)
  ```

### 7. 📝 **Clear and Useful Documentation**

**Why it matters**: Code is read much more often than it is written.

**Practices**:
- ✅ **Complete docstrings**:
  ```python
  def calculate_shipping(weight, distance, express=False):
      """
      Calculate shipping cost based on weight and distance.
      
      Args:
          weight (float): Package weight in kg
          distance (float): Distance in km
          express (bool): If True, uses express shipping (default: False)
      
      Returns:
          float: Shipping cost in dollars
      
      Raises:
          ValueError: If weight or distance is negative
      
      Examples:
          >>> calculate_shipping(2.5, 100)
          25.0
          >>> calculate_shipping(2.5, 100, express=True)
          37.5
      """
      if weight < 0 or distance < 0:
          raise ValueError("Weight and distance must be positive")
      
      base_cost = weight * distance * 0.1
      return base_cost * 1.5 if express else base_cost
  ```

- ✅ **Comments explain "why", not "what"**:
  ```python
  # ❌ BAD - Comments the obvious
  x = x + 1  # Increment x
  
  # ✅ GOOD - Explains the reason
  # Increment counter to include current element in count
  # since range() excludes the last element
  x = x + 1
  ```

- ✅ **README with practical examples**:
  ```markdown
  # How to use
  
  ## Installation
  ```bash
  pip install mypackage
  ```
  
  ## Basic example
  ```python
  from mypackage import Calculator
  
  calc = Calculator()
  result = calc.add(2, 3)
  print(result)  # Output: 5
  ```
  ```

### 8. 🏗️ **Organization and Modularity**

**Why it matters**: Organized code is easier to maintain and scale.

**Practices**:
- ✅ **Separation of concerns**:
  ```
  project/
  ├── models/       # Data structures
  ├── services/     # Business logic
  ├── controllers/  # Flow coordination
  ├── views/        # User interface
  ├── utils/        # Helper functions
  └── tests/        # Automated tests
  ```

- ✅ **DRY (Don't Repeat Yourself)**:
  ```python
  # ❌ BAD - Duplicated code
  def process_order_a():
      validate()
      calculate()
      save()
  
  def process_order_b():
      validate()
      calculate()
      save()
  
  # ✅ GOOD - Reused code
  def process_order_common():
      validate()
      calculate()
      save()
  
  def process_order_a():
      process_order_common()
      # specific logic A
  
  def process_order_b():
      process_order_common()
      # specific logic B
  ```

- ✅ **Single responsibility principle**:
  ```python
  # ❌ BAD - Class does many things
  class User:
      def __init__(self): pass
      def save_to_database(self): pass
      def send_email(self): pass
      def generate_pdf_report(self): pass
  
  # ✅ GOOD - Specialized classes
  class User:
      def __init__(self): pass
  
  class UserRepository:
      def save(self, user): pass
  
  class EmailService:
      def send(self, to, message): pass
  
  class ReportGenerator:
      def generate_pdf(self, user): pass
  ```

### 9. 🔄 **Effective Version Control**

**Why it matters**: Clean history facilitates debugging and collaboration.

**Practices**:
- ✅ **Atomic and descriptive commits**:
  ```bash
  # ❌ BAD
  git commit -m "fixes"
  git commit -m "updates"
  
  # ✅ GOOD
  git commit -m "feat: add email validation in registration form"
  git commit -m "fix: correct discount calculation for amounts over $1000"
  ```

- ✅ **Branches for features**:
  ```bash
  # Create branch for new feature
  git checkout -b feature/user-authentication
  
  # Develop and commit
  git commit -m "feat: implement JWT login"
  
  # Merge after review
  git checkout main
  git merge feature/user-authentication
  ```

- ✅ **Appropriate .gitignore**:
  ```gitignore
  # Python
  __pycache__/
  *.pyc
  .env
  venv/
  
  # JavaScript
  node_modules/
  dist/
  .env.local
  
  # IDEs
  .vscode/
  .idea/
  *.swp
  
  # OS
  .DS_Store
  Thumbs.db
  ```

### 10. 📦 **Dependency Management**

**Why it matters**: Poorly managed dependencies cause compatibility problems.

**Practices**:
- ✅ **Pin versions**:
  ```
  # ❌ BAD - requirements.txt
  flask
  requests
  
  # ✅ GOOD - requirements.txt
  flask==2.3.2
  requests==2.31.0
  ```

- ✅ **Use virtual environments**:
  ```bash
  # Python
  python -m venv venv
  source venv/bin/activate
  pip install -r requirements.txt
  
  # Node.js
  npm install  # Uses package-lock.json
  ```

- ✅ **Check for vulnerabilities**:
  ```bash
  # Python
  pip install pip-audit
  pip-audit
  
  # Node.js
  npm audit
  npm audit fix
  ```

### 11. 🔄 **Frequent Code Refactoring**

**Why it matters**: Code that isn't regularly refactored tends to deteriorate over time, becoming difficult to maintain, understand, and evolve.

> **CRITICAL FOR AIs**: Remember to **frequently** refactor code during development to maintain quality and avoid accumulation of technical debt.

**Mandatory practices**:

- ✅ **Avoid excessively large files**:
  ```
  # 🚨 SIZE ALERTS
  - File > 500 lines → Consider splitting
  - File > 1000 lines → MUST split
  - Class > 300 lines → Refactor into smaller classes
  - Function > 50 lines → Split into helper functions
  ```
  
  **Refactoring example**:
  ```python
  # ❌ BAD - 1500-line file
  # user_manager.py (everything in one file)
  class UserManager:
      def create_user(): pass  # 100 lines
      def validate_user(): pass  # 150 lines
      def authenticate_user(): pass  # 200 lines
      def send_email(): pass  # 100 lines
      # ... 950 more lines
  
  # ✅ GOOD - Split into specialized modules
  # user/
  #   __init__.py
  #   manager.py (200 lines)
  #   validator.py (150 lines)
  #   authenticator.py (200 lines)
  #   notifications.py (100 lines)
  ```

- ✅ **Increase cohesion (Single Responsibility Principle)**:
  ```python
  # ❌ BAD - Low cohesion (does many different things)
  class OrderProcessor:
      def process_order(self):
          self.validate_payment()
          self.send_email()
          self.update_inventory()
          self.generate_invoice()
          self.log_analytics()
  
  # ✅ GOOD - High cohesion (each class has one responsibility)
  class PaymentValidator:
      def validate(self): pass
  
  class EmailNotifier:
      def send_order_confirmation(self): pass
  
  class InventoryManager:
      def update_stock(self): pass
  
  class InvoiceGenerator:
      def generate(self): pass
  
  class AnalyticsLogger:
      def log_order(self): pass
  ```

- ✅ **Constantly improve readability**:
  ```python
  # ❌ BAD - Hard to understand
  def p(d, x, y):
      return sum([d[i][x] * d[i][y] for i in range(len(d)) if x in d[i] and y in d[i]])
  
  # ✅ GOOD - Self-explanatory
  def calculate_correlation_between_features(dataset, feature_x, feature_y):
      """
      Calculates the correlation between two features in a dataset.
      
      Args:
          dataset: List of dictionaries containing features
          feature_x: Name of the first feature
          feature_y: Name of the second feature
      
      Returns:
          float: Sum of feature products when both exist
      """
      correlation_sum = 0
      for data_point in dataset:
          if feature_x in data_point and feature_y in data_point:
              correlation_sum += data_point[feature_x] * data_point[feature_y]
      return correlation_sum
  ```

- ✅ **Eliminate redundancies and increase reusability**:
  ```python
  # ❌ BAD - Duplicated code (redundancy)
  def get_active_users():
      users = db.query("SELECT * FROM users")
      active = [u for u in users if u.status == 'active' and u.verified == True]
      return active
  
  def get_active_admins():
      users = db.query("SELECT * FROM users")
      active = [u for u in users if u.status == 'active' and u.verified == True and u.role == 'admin']
      return active
  
  # ✅ GOOD - Reusable code (DRY - Don't Repeat Yourself)
  def get_verified_active_users(role=None):
      """Returns active and verified users, optionally filtered by role."""
      users = db.query("SELECT * FROM users")
      filtered = [u for u in users if u.status == 'active' and u.verified == True]
      
      if role:
          filtered = [u for u in filtered if u.role == role]
      
      return filtered
  
  def get_active_users():
      return get_verified_active_users()
  
  def get_active_admins():
      return get_verified_active_users(role='admin')
  ```

- ✅ **Hierarchize code into folders and directories**:
  ```
  # ❌ BAD - Everything in root (hard to navigate)
  project/
    main.py
    user_stuff.py
    payment_things.py
    email_sender.py
    validators.py
    helpers.py
    utils.py
    config.py
    constants.py
  
  # ✅ GOOD - Logical hierarchy (easy to understand and maintain)
  project/
    main.py
    config/
      __init__.py
      settings.py
      constants.py
    core/
      __init__.py
      models.py
      exceptions.py
    features/
      users/
        __init__.py
        manager.py
        validator.py
      payments/
        __init__.py
        processor.py
        validator.py
    services/
      email/
        __init__.py
        sender.py
        templates.py
    utils/
      __init__.py
      helpers.py
      formatters.py
  ```

- ✅ **Search for orphaned code after refactoring** (⭐ **MANDATORY**):
  
  > **CRITICAL**: After any refactoring, it is **MANDATORY** to search for orphaned code - code that was implemented but is no longer being used.
  
  **What is orphaned code?**
  - ❌ Unused functions (defined but never called)
  - ❌ Unused variables (declared but never referenced)
  - ❌ Unused imports (imported but never used)
  - ❌ Dead/unreachable code
  - ❌ Uninstantiated classes (defined but never created)
  - ❌ Uncalled methods (defined but never invoked)
  
  **Why search for orphaned code?**
  - ✅ **Reduces complexity**: Less code = easier to understand
  - ✅ **Improves maintenance**: Don't waste time on unused code
  - ✅ **Avoids confusion**: Orphaned code can mislead developers
  - ✅ **Performance**: Less code = faster startup
  - ✅ **Security**: Orphaned code may contain forgotten vulnerabilities
  
  **Tools to detect orphaned code**:
  ```bash
  # Python - Unused code (functions, classes, variables)
  pip install vulture
  vulture src/ --min-confidence 80
  # Output: unused functions/classes/variables
  
  # Python - Unused imports
  pip install autoflake
  autoflake --remove-all-unused-imports --check -r src/
  # Or use pylint
  pylint --disable=all --enable=unused-import src/
  
  # JavaScript/TypeScript - Unused code
  npm install -g ts-prune  # For TypeScript
  ts-prune
  # Or ESLint
  npm run lint -- --rule 'no-unused-vars: error'
  
  # For any language - Search for unused definitions
  # 1. Generate list of definitions (functions, classes)
  # 2. Search for references to each definition in code
  # 3. If no reference found → orphaned code
  ```
  
  **Usage example (Python)**:
  ```python
  # Before refactoring - 500-line file
  
  # Refactoring: split into 3 smaller files
  # Now search for orphaned code:
  
  $ vulture src/ --min-confidence 80
  src/old_module.py:45: unused function 'process_legacy_format' (100% confidence)
  src/utils.py:123: unused function 'deprecated_helper' (90% confidence)
  src/models.py:67: unused class 'OldDataModel' (100% confidence)
  
  # Action: Remove or document why keeping
  # If truly unused → DELETE
  # If will be used in future → Mark with comment and issue
  ```
  
  **Orphaned code checklist** (execute AFTER refactoring):
  ```markdown
  - [ ] Run vulture (Python) or ts-prune (TypeScript)
  - [ ] Review unused functions (confirm if truly orphaned)
  - [ ] Remove unused imports (autoflake or similar tool)
  - [ ] Check uninstantiated classes
  - [ ] Search for old commented code (also orphaned code)
  - [ ] Document if any "orphaned" code should be kept (e.g., public API)
  ```
  
  **When NOT to remove**:
  - ✅ **Public APIs**: Even if not used internally, external clients may use them
  - ✅ **Hooks/callbacks**: May be called by frameworks
  - ✅ **Test code**: Test helpers may appear unused
  - ✅ **Planned code**: If there's an issue/task to use soon, keep (but document)

**When to refactor**:

1. **During new feature implementation**:
   - Before adding new code, check if existing files are organized
   - If you find poorly structured code, refactor BEFORE adding new functionality

2. **After completing a feature**:
   - Review the implemented code
   - Identify improvement opportunities (DRY, SRP, better names)
   - Refactor immediately while context is fresh
   - **⭐ MANDATORY**: Search for orphaned code (vulture, autoflake, etc.)

3. **When reviewing code (Steps 7 and 8)**:
   - Use the 9 quality criteria as a guide
   - If you detect redundancy, lower cohesion, or higher coupling → Refactor

4. **Before committing (Step 13)**:
   - Last checkpoint: is the code as clean as possible?
   - Is there anything that can be simplified?

5. **Minimum periodicity**:
   - ⚠️ **NEVER** let more than 3-5 features pass without refactoring
   - 🚨 If project has > 10 files with > 500 lines → PRIORITIZE refactoring
   - ⭐ **Always search for orphaned code after refactoring** (not optional)

**Benefits of frequent refactoring**:
- ✅ **Simpler maintenance**: Organized code is easier to modify
- ✅ **Fewer bugs**: Clean code has fewer places for bugs to hide
- ✅ **Faster onboarding**: New developers understand the code faster
- ✅ **Speed**: Paradoxically, frequent refactoring ACCELERATES development
- ✅ **Easier validation**: Modular code is easier to test and verify

**Tools to identify refactoring needs**:
```bash
# Python - Cyclomatic complexity
pip install radon
radon cc . -a -nb  # Show complex functions

# Python - Duplicated code
pip install pylint
pylint --disable=all --enable=duplicate-code .

# Python - Dead code
pip install vulture
vulture .

# JavaScript - Complexity analysis
npm install -g complexity-report
cr --format json src/
```

### 🎯 **Quick Checklist for AI**

Before generating/committing code, verify:

- [ ] Names are descriptive and follow language conventions?
- [ ] Functions have single responsibility and are small?
- [ ] Is there error handling for exceptional cases?
- [ ] Code is tested (unit tests + edge cases)?
- [ ] No obvious security vulnerabilities?
- [ ] Performance is acceptable (no unnecessary O(n²) algorithms)?
- [ ] Is there documentation (docstrings, useful comments)?
- [ ] Code is organized in logical modules?
- [ ] **Code was recently refactored?** (files < 500 lines, no duplication)
- [ ] **Folder hierarchy is logical?** (clear separation of responsibilities)
- [ ] Commits are descriptive (conventional commits)?
- [ ] Dependencies have pinned versions?

### 📚 **Additional Resources**

- **Clean Code** (Robert C. Martin) - Clean code principles
- **SOLID Principles** - Well-done object orientation
- **Design Patterns** (GoF) - Common solutions to common problems
- **OWASP Top 10** - Main security vulnerabilities
- **PEP 8** (Python) - Python style guide
- **Google Style Guides** - Style guides by language

---

**Reread this document before each sprint!**

---

**Version**: 2.3
**Last updated**: December 16, 2025
**Maintained by**: Josué Amaral
**Status**: ACTIVE - Advanced protocol for critical/enterprise projects
```
