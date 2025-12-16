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
## 📋 Task Management (TASKS.md)

All Simplicity protocols now include integrated support for task management through a `TASKS.md` file (or alternative file of your choice).

### Task System Features:
- ✅ **Default File**: `TASKS.md` in project root (ASCII format: `.md`, `.txt`)
- 🔄 **Flexible**: Use any file name/location (as long as it's ASCII)
- 🤖 **AI Recommendations (Optional)**: Intelligent system for suggesting new tasks
- 📊 **Growth Curve**: Recommendations follow quadratic pattern (grow, peak, then decrease)
- 🎯 **Scope Control**: Only project-relevant suggestions
- 🔢 **Configurable Limit**: Default of 30 new recommended tasks (customizable)

### How AI Recommendations Work:
AI can dynamically suggest new tasks as the project evolves, following a 5-phase pattern:
1. **Phase 1 (0-20%)**: Initial growth - few essential tasks
2. **Phase 2 (20-40%)**: Acceleration - main features
3. **Phase 3 (40-70%)**: Maximum peak - maximum ideas and opportunities
4. **Phase 4 (70-90%)**: Deceleration - only critical tasks
5. **Phase 5 (90-100%)**: Exhaustion - stop adding features

📖 **Complete details**: See "AI Task Recommendations" section in Step 12 of each protocol.

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

## 📝 Credits and Versioning

- **Author:** Josué Amaral
- **License:** Internal and educational use.
- **Status:**
    - Simplicity 1: `v2.0`
    - Simplicity 2: `v2.2`
    - Simplicity 3: `v3.1`

> *"I want complete and professional work!"*
