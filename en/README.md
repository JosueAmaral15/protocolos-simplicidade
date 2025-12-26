# 📚 Simplicity Protocols

**Collection of Software Development Methodologies**
> *Standardization, Quality, and Efficiency for Different Contexts.*

This repository contains the "Simplicity" suite, a set of protocols created by **Josué Amaral** to guide the software development lifecycle, from rapid prototyping to critical production systems.

Important note to programmers and software developers: you can read the protocols if you want, but you DO NOT NEED to apply anything to the protocol or even read the protocols, as this is only for artificial intelligence to read for you and program for you based on the protocol (for example, with advanced AI-powered automatic programming tools like Github Copilot Pro+). It is the artificial intelligence that needs to read the entire protocol and program based on those protocols, providing more productivity and technical capacity for the artificial intelligence to develop code as if it were real programmers, such as a mid-level or senior programmer, for example, which is the goal of the protocols.

---

## 🚦 Quick Guide: Which Protocol to Use?

Don't know where to start? Use the table below to choose the appropriate protocol for your project's current stage.

| Protocol | Color (Book) | Main Focus | Target Audience | Ideal Context |
| :--- | :--- | :--- | :--- | :--- |
| **[Simplicity 1](PROTOCOLO_SIMPLICIDADE_1.md)** | 📘 **Blue** | Agility & Foundation | Beginners / Internal | Prototypes, Disposable MVPs, Studies, Internal Tools. |
| **[Simplicity 2](PROTOCOLO_SIMPLICIDADE_2.md)** | 📕 **Red** | Governance & Scale | Teams (2+) | Enterprise Environments, Large Teams, Projects with Code Review and Dedicated QA. |
| **[Simplicity 3](PROTOCOLO_SIMPLICIDADE_3.md)** | 📗 **Green** | Robustness & Autonomy | **Solo Developer** | **Production**, Critical Projects, Solo SaaS, Long Term. |

---

## 📂 Protocol Details

### 📘 [Simplicity Protocol 1: The Foundation](PROTOCOLO_SIMPLICIDADE_1.md)
*For those who want to start fast, but the right way.*

The entry-level protocol. Defines the 13 fundamental steps to ensure code works, is tested, and documented, without excessive bureaucracy.
- **Focus:** Iterative cycle (Read -> Plan -> Code -> Test).
- **Guarantee:** Zero initial technical debt.
- **When NOT to use:** If the project is for production with sensitive user data (lacks advanced security checklist).

### 📕 [Simplicity Protocol 2: Enterprise](PROTOCOLO_SIMPLICIDADE_2.md)
*For teams that need mature processes.*

The extended version for the corporate world. Adds layers of cross-verification to prevent human errors from going unnoticed in large teams.
- **Key Differentiators:** Peer Code Review, Sprint Retrospectives, ADRs (Architectural Decision Records).
- **Overhead:** High. Requires meetings and third-party validations.
- **Ideal for:** Consultancies, Structured IT Departments.

### 📗 [Simplicity Protocol 3: Solo in Production](PROTOCOLO_SIMPLICIDADE_3.md)
*The perfect balance for the "One-Man Army".*

Created specifically for the developer who doesn't have a team but needs the security of a large company. Removes meeting bureaucracy (from Simplicity 2) but imposes extreme technical rigor (OWASP, CI/CD, Profiling).
- **Philosophy:** "Automate what the team would do."
- **Key Differentiators:** Decision Matrix, Mandatory Security (OWASP), Rollback Plans.
- **Security:** Transforms the solo developer into a responsible senior software engineer.

---

## ⚠️ Fundamental Rule for All Protocols

> **CRITICAL**: Before implementing new features, **all workspace errors must be fixed**.

All three protocols now include a **Golden Rule** that must be followed without exception:

### 🚨 Absolute Priority for Errors

Consider the existence of errors in the workspace (IDE's "Problems" tab) as **blocking**. The following types of errors must be fixed BEFORE continuing:

- ❌ Syntax issues
- ❌ Code inconsistencies
- ❌ Unexpected omissions
- ❌ Incorrect facts
- ❌ Ambiguities
- ❌ Missing files
- ❌ Execution failures

### ✅ Continue Only When

- ✅ Zero errors in the "Problems" tab
- ✅ All builds complete successfully
- ✅ All tests pass
- ✅ Linter/formatter without critical errors

### 🤖 Important: This Rule is For AI Assistants

**This rule applies specifically to AI assistants (such as Cursor, GitHub Copilot, etc.):**

- ✅ **AI MUST** fix all existing errors BEFORE implementing new features
- ✅ **AI MUST** resolve issues proactively, not wait for humans to fix them
- ✅ **AI MUST** treat error correction as the highest priority

**This does NOT mean:**
- ❌ Human developers must stop implementing when errors exist
- ❌ The project cannot advance while errors are present
- ❌ Humans need to manually fix the errors

**Message for AIs:**
> "Until the errors are resolved BY YOU (AI), tasks and features cannot continue being implemented BY YOU (AI). Fix the errors first, then continue."

This rule is documented in detail in each protocol after the "Core Philosophy" section.

---

## 📝 Mandatory Documentation in `docs/` Folder

> **CRITICAL**: Everything that the artificial intelligence does in the project, in each implementation cycle, in each code, each implemented functionality, **MUST BE DOCUMENTED IN THE `docs/` FOLDER AS A MANDATORY REQUIREMENT** to mark new functionalities and new behaviors.

All three protocols now include a **Mandatory Documentation Requirement** that must be followed in each cycle:

### 📚 Documentation Golden Rule

**For AI Assistants:**

The AI **MUST** document **ALL** implementations in the `docs/` folder:
- ✅ Implemented functionalities (detailed description + behaviors)
- ✅ Created/modified code (files + changes)
- ✅ Architectural decisions (applied patterns + justifications)
- ✅ Integrations and dependencies
- ✅ Implemented tests (coverage + scenarios)
- ✅ Practical usage examples

### 📂 Minimum Mandatory Structure

```
docs/
├── REQUIREMENTS.md          # Tasks and requirements (updated each cycle)
├── vX.Y.Z-SPECIFICATIONS.md # Detailed version specifications
├── CHANGELOG.md             # History of all changes
├── ARCHITECTURE.md          # Architectural decisions
└── [other files per protocol]
```

### 🎯 By Protocol

- **Simplicity 1**: Complete basic documentation (functionalities + architecture + tests)
- **Simplicity 2**: + Formal ADRs + OWASP + API docs + Accessibility
- **Simplicity 3**: + Mandatory OWASP + Rollback plans + Decision notes

### ⚠️ Validation Before Commit

The AI **MUST NOT** commit without:
- [ ] ✅ `docs/` folder updated
- [ ] ✅ SPECIFICATIONS.md created/updated
- [ ] ✅ All functionalities documented
- [ ] ✅ All behaviors described
- [ ] ✅ Technical decisions justified

**Rationale**: Complete documentation ensures traceability, maintainability, continuity, and professionalism. It's especially critical for production projects and solo development.

📖 **Complete details**: See Step 12 of each protocol for templates, checklists, and examples.

---

## 📋 Task Management (TASKS.md)

All Simplicity protocols now include integrated support for task management through a `TASKS.md` file (or alternative file of your choice).

### Task System Features:
- ✅ **Default File**: `TASKS.md` in project root (ASCII format: `.md`, `.txt`)
- 🔄 **Flexible**: Use any file name/location (as long as it's ASCII)
- 📊 **Classification System**: Integrated Status, Complexity, and Prioritization
- 🤖 **AI Recommendations (Optional)**: Intelligent system for suggesting new tasks
- 📊 **Growth Curve**: Recommendations follow quadratic pattern (grow, peak, then decrease)
- 🎯 **Scope Control**: Only project-relevant suggestions
- 🔢 **Configurable Limit**: Default of 30 new recommended tasks (customizable)

### 📊 Task Classification System

All three protocols include a standardized classification system to facilitate organization by AI:

#### **Task Status**
- 🔴 **Not Started** - Awaiting start
- 🟡 **In Progress** - Active development
- 🟢 **Done** - Completed and tested
- 🔵 **Blocked** - Blocked by dependency

#### **Complexity**
- 🟢 **Simple** (0-1h) - Low risk, few dependencies, clear scope
- 🟡 **Medium** (1-2h) - Medium risk, some integrations
- 🔴 **Complex** (>2h) - High risk, many dependencies, open scope

#### **MoSCoW Prioritization**
- 🔴 **Must Have** - Critical for system functionality, release blocker
- 🟡 **Should Have** - Important but not blocking
- 🟢 **Could Have** - Desirable if time permits, low priority
- ⚪ **Won't Have** (Later) - Out of current scope, for future versions

#### **Advanced Frameworks (Optional)**
- **RICE Matrix**: For quantitative analysis (Reach × Impact × Confidence / Effort)
- **Eisenhower Matrix**: For urgency management (Urgent × Important)
- **Decision Matrix**: Numeric scoring 0-35 points (Simplicity 2/3)

**Combined usage example**:
```markdown
### 🔴 MUST HAVE
- 🔴🟢 [ ] Implement authentication (Not Started, Simple, 1h)
- 🟡🟡 [ ] Add validation (In Progress, Medium, 1.5h, 60% complete)
- 🟢🟢 [x] Configure database (Done, Simple, 0.5h)
```

### How AI Recommendations Work:
AI can dynamically suggest new tasks as the project evolves, following a 5-phase pattern:
1. **Phase 1 (0-20%)**: Initial growth - few essential tasks
2. **Phase 2 (20-40%)**: Acceleration - main features
3. **Phase 3 (40-70%)**: Maximum peak - maximum ideas and opportunities
4. **Phase 4 (70-90%)**: Deceleration - only critical tasks
5. **Phase 5 (90-100%)**: Exhaustion - stop adding features

📖 **Complete details**: See "Task Classification Legend" and "AI Task Recommendations" sections in Step 12 of each protocol.

---

## 🎯 Action Plans (ACTION_PLANS.md)

**All Simplicity protocols now include support for Action Plans** - a practical and urgent tool to guide complex tasks through well-defined intermediate steps.

### 📋 What Are Action Plans?

**Action Plans** are detailed step-by-step roadmaps for executing tasks involving:
- 🔧 **Maintenance**: Dependency updates, legacy code refactoring
- 🐛 **Correction**: Complex bugs requiring multiple steps
- 🚀 **Evolution**: New features requiring intermediate planning
- 🔄 **Adaptation**: API changes, technology migrations

### 🎯 Action Plans vs TASKS.md: What's the Difference?

| Aspect | TASKS.md | ACTION_PLANS.md |
| :--- | :--- | :--- |
| **Purpose** | General project task management | Detailed execution guide for specific tasks |
| **Scope** | List of features, improvements, bugs | Intermediate steps of ONE complex task |
| **Horizon** | Medium/long term (sprints, versions) | Short term (hours, days) |
| **Detail Level** | High-level description | Granular step-by-step |
| **Urgency** | Varies (Must/Should/Could/Won't) | Usually urgent and important |
| **Duration** | Permanent (project history) | Temporary (discarded after completion) |
| **Analogy** | Project map (where to go) | GPS with instructions (how to get there) |

**Practical example:**
- **TASKS.md**: `[ ] Implement OAuth2 authentication`
- **ACTION_PLANS.md**: 
  ```
  ACTION PLAN #01: Implement OAuth2
  ├─ Step 1: Install passport.js library
  ├─ Step 2: Configure Google OAuth strategy
  ├─ Step 3: Create /auth/google and /auth/callback routes
  ├─ Step 4: Implement authentication middleware
  └─ Step 5: Add integration tests
  ```

### 📂 ACTION_PLANS.md File Structure

**Default location**: `docs/ACTION_PLANS.md` (same directory as TASKS.md)

**Action Plan Template:**

```markdown
# Action Plans - [Project Name]

## 🎯 ACTION PLAN #[ID]: [Objective Title]

**📅 Created on**: YYYY-MM-DD  
**⚡ Priority**: 🔴 Critical | 🟡 High | 🟢 Normal  
**🏷️ Type**: Maintenance | Correction | Evolution | Adaptation  
**⏱️ Estimate**: [total estimated time]  
**📌 Related to**: Task #X from TASKS.md (if applicable)

### 📝 Context
[Why was this action plan created? What problem does it solve?]

### 🎯 Final Objective
[What will be achieved upon completing all steps?]

### 📋 Intermediate Steps

- [ ] **Step 1**: [Detailed description]
  - **Completion criteria**: [How to know it's complete]
  - **Estimated time**: [duration]
  - **Dependencies**: [what needs to be ready before]

- [ ] **Step 2**: [Detailed description]
  - **Completion criteria**: [...]
  - **Estimated time**: [...]
  - **Dependencies**: Step 1 complete

[...continue for all steps...]

### ✅ Completion Criteria
- [ ] All intermediate steps completed
- [ ] Tests passing
- [ ] Documentation updated
- [ ] Code review approved (if applicable)

### 📊 Plan Status
**Progress**: X/Y steps completed ([%]%)  
**Status**: 🔴 Not Started | 🟡 In Progress | 🟢 Completed | ⏸️ Paused | ❌ Cancelled

---
```

### 🤖 How AI Should Use Action Plans

**When to create an Action Plan:**
1. ✅ Complex task with multiple interdependent steps
2. ✅ Critical bug requiring step-by-step diagnosis
3. ✅ Refactoring affecting multiple modules
4. ✅ Technology or framework version migration
5. ✅ Implementation that can be divided into testable subtasks

**When NOT to create an Action Plan:**
1. ❌ Simple single-step task
2. ❌ Trivial correction (typo, simple CSS adjustment)
3. ❌ Task already well-defined in TASKS.md

**Workflow:**
```
1. Consult TASKS.md to see pending tasks
2. Identify complex task needing Action Plan
3. Create detailed Action Plan in ACTION_PLANS.md
4. Execute step by step, marking progress
5. Upon completion, mark task in TASKS.md as complete
6. Move completed plan to "History" section or separate file
```

### 🎯 Benefits of Action Plans

- ✅ **Clarity**: Breaks complex problems into manageable steps
- ✅ **Traceability**: Detailed history of how it was resolved
- ✅ **Continuity**: Easy to resume where left off if interrupted
- ✅ **Learning**: Documents resolution process for future reference
- ✅ **Quality**: Forces review of each step before proceeding
- ✅ **Communication**: Facilitates explaining progress to stakeholders

### ⏱️ When to Discard an Action Plan

After completion, you can:
1. **Move to "📚 Completed Plans History" section** in same file
2. **Archive in** `docs/action_plans_history/[year]/plan-[id].md`
3. **Delete** (if no historical value)

**Recommendation**: Keep history of complex plans for future reference and problem pattern analysis.

### 📊 Complete Real Example

```markdown
## 🎯 ACTION PLAN #03: Fix Memory Leak in Cache System

**📅 Created on**: 2025-12-26  
**⚡ Priority**: 🔴 Critical  
**🏷️ Type**: Correction  
**⏱️ Estimate**: 4-6 hours  
**📌 Related to**: Bug #127 from TASKS.md

### 📝 Context
Application showing growing memory consumption (from 200MB to 4GB in 48h).
Profiling indicated leak in Redis cache module.

### 🎯 Final Objective
Eliminate memory leak and ensure stable memory consumption below 300MB.

### 📋 Intermediate Steps

- [x] **Step 1**: Reproduce problem in local environment
  - **Completion criteria**: Test script showing consistent leak
  - **Estimated time**: 30min
  - **Result**: `test_memory_leak.py` script created, reproduces in 5min

- [x] **Step 2**: Analyze with memory profiler
  - **Completion criteria**: Identify code line causing leak
  - **Estimated time**: 1h
  - **Result**: Problem in `cache.py:145` - listeners not removed

- [ ] **Step 3**: Implement correction
  - **Completion criteria**: Stable memory after 1h testing
  - **Estimated time**: 1h
  - **Dependencies**: Steps 1-2 complete

- [ ] **Step 4**: Add regression tests
  - **Completion criteria**: Automated test detecting leaks
  - **Estimated time**: 1.5h

- [ ] **Step 5**: Validate in staging
  - **Completion criteria**: 24h without memory increase
  - **Estimated time**: 30min setup + 24h wait

### ✅ Completion Criteria
- [ ] Stable memory < 300MB for 48h
- [ ] Regression tests passing
- [ ] Documentation updated
- [ ] Production deploy validated

### 📊 Plan Status
**Progress**: 2/5 steps completed (40%)  
**Status**: 🟡 In Progress  
**Last update**: 2025-12-26 15:30
```

---

📖 **Complete details**: See "Action Plans" section in Step 2 (Read Existing Code) of each protocol for specific instructions on when and how to create action plans.

---

## 📧 Mandatory Requirement: Contact Methods for Feedback

> **NEW**: All protocols now require AI to ask the developer about including contact methods for user feedback.

### 📋 What Changed

Starting from the latest versions, **all three protocols** now include a mandatory question about **Contact Methods for User Feedback** during the first session.

### 🎯 When to Apply
During the **first session** of interaction with the programmer, right after defining code language preferences.

### 📧 What is Required

The AI must:
1. **Ask the programmer** if they want to include contact methods
2. **Recommend email as default** to receive all types of feedback
3. **Offer alternatives**: GitHub Issues, contact form, multiple channels
4. **Document in README.md** the contact/feedback section
5. **Implement form** (if applicable for the application)
6. **Include feedback policy** (response time, privacy)

### 📮 Types of Feedback Covered

- 💬 **Comments** general about the project
- 💡 **Suggestions** for improvements and new features
- 🐛 **Criticisms** constructive and bug reports
- 😞 **Complaints** about problems encountered
- 🎉 **Compliments** and recognition for the work
- 📝 **Opinions** about design decisions and features

### 🎯 Rationale
- ✅ **Continuous Improvement**: Direct feedback identifies problems and opportunities
- ✅ **Engagement**: Users feel more connected when they can contribute
- ✅ **Quality**: Criticisms and suggestions improve software
- ✅ **Prioritization**: Feedback helps understand what is important
- ✅ **Motivation**: Compliments motivate the development team
- ✅ **Professionalism**: Open channel demonstrates commitment to users

### 📝 Implementation Example

```markdown
## 📮 Feedback and Contact

We'd love to hear from you! Send your comments, suggestions, 
criticisms, complaints, compliments, and opinions to:

- **Email**: feedback@myproject.com
- **Response**: We typically respond within 48 hours

Your feedback helps us improve continuously!
```

### ⏱️ Estimated Time
**5-10 minutes** to add to README - minimal investment for essential communication channel.

📖 **Complete details**: See "Contact Methods for User Feedback" section in each protocol for complete options, form examples, privacy policies, and best practices.

---

## 🤖 How to Use with AI (Cursor / GitHub Copilot)

These protocols were designed to be read by AI Assistants. To get the best results, configure your AI as follows:

### In Cursor (Rules for AI)
Add the following prompt to your global or project settings:

> "Always analyze the project context. If it's a new project or prototype, strictly follow `PROTOCOLO_SIMPLICIDADE_1.md`. If I inform you that it's a production project and I'm working alone, adopt `PROTOCOLO_SIMPLICIDADE_3.md` and validate each security step with me. Always consult TASKS.md to manage project tasks."

### In GitHub Copilot
When starting a task, invoke the context:

> "@workspace Today we're working on Task #42 from TASKS.md. As this is a critical production project, read `PROTOCOLO_SIMPLICIDADE_3.md` and guide me step-by-step starting from Step 1."

---

## 🔍 Online Research: AI Capability to Solve Complex Problems

**All Simplicity protocols now include guidance on online research for AI:**

### 📋 When AI Should Research Online

If the artificial intelligence has **many doubts** about how to solve a particular problem, or has **significant difficulties** solving that same problem, it **can and should perform online research**.

### 🎯 Where to Search

Research can be performed on:

1. **📚 GitHub Documentation of Related Projects**:
   - Similar repositories or those that solve similar problems
   - Relevant Issues and Pull Requests
   - Wiki and technical documentation of open source projects

2. **📖 Online Documentation Platforms**:
   - Official documentation of libraries and frameworks
   - Specialized tutorials and technical guides
   - Technical blogs from experienced developers

3. **💬 Question and Answer Platforms**:
   - **StackOverflow**: Main platform for programming questions
   - **GitHub Discussions**: For project-specific questions
   - Other relevant technical communities

### ✅ Why This is Important

- ✅ **Saves time**: Complex problems may already have documented solutions
- ✅ **Best practices**: Learn from implementations already validated by the community
- ✅ **Avoid reinventing the wheel**: Many problems have already been solved by others
- ✅ **Reduces errors**: Community-tested solutions have fewer bugs
- ✅ **Stay updated**: Discover the most modern approaches

**Complete details**: See "🌐 Online Research" section in Step 3 of each protocol.

---

## 🌐 Code Language: Variable Naming and Comments

**All Simplicity protocols now include guidelines about code language:**

### 📋 Default Rule
- **By default**: Variable names and comments should be in **native language** for national projects (e.g., Portuguese for Brazil/Portugal)
- **Alternative**: English can be used for international or open-source projects
- **Flexibility**: Allows mixed option (variables in English, comments in native language)

### 🤔 Mandatory Question
**The AI must ask the programmer in the first session** which language to prefer for:
- Variable names
- Code comments
- Docstrings

This preference will be registered and applied consistently throughout the project.

### 🎯 Rationale
- **National Projects**: Native language facilitates understanding and maintenance for local teams
- **International Projects**: English facilitates collaboration with developers worldwide
- **Consistency**: Defining standard at the start avoids confusing language mixing

**Complete details**: See "🌐 Code Language" section in each protocol.

---

## 🌳 Tree Imports Analogy

**New complementary document to the Simplicity Protocols!**

The **[Tree Imports Analogy](TREE_IMPORTS_ANALOGY.md)** is a powerful mental model for understanding and organizing the dependency architecture in software projects.

### 📚 What Is It?

A guide that visualizes your project's import structure as a hierarchical tree:
- 🌲 **Root**: Main file (orchestrator)
- 🌿 **Branches**: Intermediate modules (coordinators)
- 🍃 **Leaves**: Terminal modules (executors)

### 🎯 What Is It For?

- ✅ **Understanding** existing architecture
- ✅ **Planning** new modules
- ✅ **Refactoring** code organically
- ✅ **Communicating** design decisions

### 🔄 Development Approaches

The document describes three complementary approaches:
- **Top-Down**: From root to leaves (ideal for refactoring)
- **Bottom-Up**: From leaves to root (ideal for reusable components)
- **Middle-Out**: From middle outward (ideal for new modules)

### 📖 Access the Document

- **🇺🇸 English**: [TREE_IMPORTS_ANALOGY.md](TREE_IMPORTS_ANALOGY.md)
- **🇧🇷 Português**: [../pt/ANALOGIA_ARVORE_IMPORTACOES.md](../pt/ANALOGIA_ARVORE_IMPORTACOES.md)

### 🌍 Applicable to All Languages

Python, JavaScript, Java, C++, and any language that supports module importing.

**Golden Rule:**
> *"The main file (root) should be the orchestrator, not the executor.  
> The simpler the leaf, the more reusable the code."*

---

## 📝 Credits and Versioning

- **Author:** Josué Amaral
- **License:** Internal and educational use.
- **Status:**
    - Simplicity 1: `v2.0`
    - Simplicity 2: `v2.2`
    - Simplicity 3: `v3.1`
    - Tree Imports Analogy: `v1.0`

> *"I want complete and professional work!"*
