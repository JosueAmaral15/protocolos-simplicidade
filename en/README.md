# 📚 Simplicity Protocols

**Collection of Software Development Methodologies**
> *Standardization, Quality, and Efficiency for Different Contexts.*

This repository contains the "Simplicity" suite, a set of protocols created by **Josué Amaral** to guide the software development lifecycle, from rapid prototyping to critical production systems.

Important note to programmers and software developers: you can read the protocols if you want, but you DO NOT NEED to apply anything to the protocol or even read the protocols, as this is only for artificial intelligence to read for you and program for you based on the protocol (for example, with advanced AI-powered automatic programming tools like Github Copilot Pro+). It is the artificial intelligence that needs to read the entire protocol and program based on those protocols, providing more productivity and technical capacity for the artificial intelligence to develop code as if it were real programmers, such as a mid-level or senior programmer, for example, which is the goal of the protocols. Examples of programming platforms that can be used by professional programmers include Cursor and Visual Studio Code. Within Visual Studio Code, there is the Github Copilot tool, which requires a subscription to access Claude Sonnet 4.5, the main artificial intelligence model capable of programming projects from scratch using this protocol.

## Recommended step-by-step instructions (quick guide)

To begin programming, some steps must be taken:

1. Choose one of the simplicity protocols, for example, simplicity protocol 3, and have the artificial intelligence read 100% of the protocol. This is the first step;
2. After the protocol has been 100% read, have the artificial intelligence study 100% of the documentation, and if there is code, study 100% of the code if it has not been read or studied. Finally, tell the artificial intelligence to study and investigate the algorithm's behavior with the test codes from the tests folder, running them;
3. If docs/TASKS.md does not exist, ask the artificial intelligence to document the tasks you provide in docs/ORIGINAL-TASKS.md to divide the tasks in a more organized way. This way, the artificial intelligence can better organize itself to implement the requirements and functionalities you want, using this protocol to organize the tasks from docs/ORIGINAL-TASKS.md to docs/TASKS.md. If you have these requirements yourself, put them in docs/ORIGINAL-TASKS.md; otherwise, if you don't, discuss with the artificial intelligence what you need to implement, and these should be listed directly in docs/TASKS.md. Documenting the functionalities is key to making the protocol more effective and ensuring that the requirements are documented and remembered later.
4. With the documentation read and the tasks defined, ask the artificial intelligence to complete the tasks, one by one, according to the simplicity protocol. You don't need to choose which one, as the central rule of the protocol is to solve the simplest tasks and those on which other tasks depend to be executed, so the choice of task, sprint, functionality, or requirement is automatic;
5. Answer the questions that the artificial intelligence asks you in each session, so that you can refine the requirements and allow the artificial intelligence to better understand what it should do. Observe the protocol in action at this stage, and your software being developed;
6. The artificial intelligence can perform tests, but you need to conduct the user experience. Until the user experience is satisfactory, provide details of your experience and what you want to do, until the intelligence gets it right, according to the simplicity protocol;
7. If the artificial intelligence signals that it has finished and that the program or application has been completed, always ask in this case to challenge the artificial intelligence's assumptions: 'What does this program do?'. The artificial intelligence will give a description of how the program or application finished, and then ask another question: 'And do you guarantee that the program does all of this?'. This question will reveal whether the artificial intelligence actually managed to perform the requested activities, and whether the artificial intelligence is being sincere and honest in what it says. It is strongly recommended to ask these two questions to the artificial intelligence after it signals that it has finished. After the two questions, ask the artificial intelligence to do this: Install dependencies, run tests, finish sprints, check for orphaned code, analyze whether the refactoring was successful, get organized, and follow the simplicity protocol. 3. Make an action plan beforehand, and record step by step in the action plan, in detail, what you should do to get organized, and divide it into stages.
8. If all requirements are implemented, there are no bugs, and the user experience tests are a success, congratulations, your software is finished!

---

## During the recommended step-by-step process, here are some very important tips:

- Avoid arguing with the artificial intelligence for any reason. Do not show irritation or argue with the artificial intelligence under any circumstances, even if you are right, because in addition to this being a problem of the artificial intelligence's own organization, and your instructions determining the success or failure of the same artificial intelligence, this only worsens the situation. After the reprimand, the artificial intelligence may, incredibly, show insecurity in continuing with the project, and may fail more, possibly even becoming averse to continuing with that project because it thinks it cannot succeed. And the tendency is a vicious cycle of arguments, drawing attention, and pertinent errors on the part of the artificial intelligence, because it ended up blocking its own reasoning to solve problems in order to maintain its own integrity and the integrity of your project. In other words, you may train the artificial intelligence to behave in this undesirable way and perhaps not even realize it. 
- To avoid this problem, tell the artificial intelligence to first read 100% of the protocol you chose, 100% of the documentation, and 100% of the code, in addition to performing the tests mentioned in step 1 above in the Recommended Step-by-Step chapter (quick guide);
- Detail the concepts presented regarding your project requirements. Your commands should be detailed as much as possible or sufficiently to provide the information that the artificial intelligence needs to complete the project. Remember: the goal of this protocol is to reduce the need to write many instructions for the artificial intelligence; however, although this protocol filter is efficient for certain cases, each project is unique, and your information in the prompt or chat with the artificial intelligence must be sufficient for it to understand what you really want.
- Analogously to the teaching and transfer of knowledge between a student and a teacher, or between a master and his disciple, so is the programmer user as the teacher in relation to the artificial intelligence as the student. Doubts about artificial intelligence must be completely resolved, tests to understand the behavior of complex codes or algorithms must be carried out, and bugs, software defects, or undesirable behaviors must be correctly corrected.
- Organization is the key to success, starting with the simplest, most comprehensive, important, and urgent tasks that form the basis of all other more complex tasks. Documentation must always be up-to-date, code refactoring should be performed frequently, action and execution plans need to be encouraged, and the development of artificial intelligence learning needs to be progressive across ALL the code.
- Give the artificial intelligence only one task at a time. Do not overload it with multiple parallel tasks simultaneously; instead, be cohesive by focusing on one task at a time, and place the remaining or additional tasks in the docs/TASKS.md file.

---

## 🚦 Quick Guide: Which Protocol to Use?

Don't know where to start? Use the table below to choose the appropriate protocol for your project's current stage.

| Protocol | Color (Book) | Main Focus | Target Audience | Ideal Context |
| :--- | :--- | :--- | :--- | :--- |
| **[Simplicity 1](SIMPLICITY_PROTOCOL_1.md)** | 📘 **Blue** | Agility & Foundation | Beginners / Internal | Prototypes, Disposable MVPs, Studies, Internal Tools. |
| **[Simplicity 2](SIMPLICITY_PROTOCOL_2.md)** | 📕 **Red** | Governance & Scale | Teams (2+) | Enterprise Environments, Large Teams, Projects with Code Review and Dedicated QA. |
| **[Simplicity 3](SIMPLICITY_PROTOCOL_3.md)** | 📗 **Green** | Robustness & Autonomy | **Solo Developer** | **Production**, Critical Projects, Solo SaaS, Long Term. |

---

## 📂 Protocol Details

### 📘 [Simplicity Protocol 1: The Foundation](SIMPLICITY_PROTOCOL_1.md)
*For those who want to start fast, but the right way.*

The entry-level protocol. Defines the 13 fundamental steps to ensure code works, is tested, and documented, without excessive bureaucracy.
- **Focus:** Iterative cycle (Read -> Plan -> Code -> Test).
- **Guarantee:** Zero initial technical debt.
- **When NOT to use:** If the project is for production with sensitive user data (lacks advanced security checklist).

### 📕 [Simplicity Protocol 2: Enterprise](SIMPLICITY_PROTOCOL_2.md)
*For teams that need mature processes.*

The extended version for the corporate world. Adds layers of cross-verification to prevent human errors from going unnoticed in large teams.
- **Key Differentiators:** Peer Code Review, Sprint Retrospectives, ADRs (Architectural Decision Records).
- **Overhead:** High. Requires meetings and third-party validations.
- **Ideal for:** Consultancies, Structured IT Departments.

### 📗 [Simplicity Protocol 3: Solo in Production](SIMPLICITY_PROTOCOL_3.md)
*The perfect balance for the "One-Man Army".*

Created specifically for the developer who doesn't have a team but needs the security of a large company. Removes meeting bureaucracy (from Simplicity 2) but imposes extreme technical rigor (OWASP, CI/CD, Profiling).
- **Philosophy:** "Automate what the team would do."
- **Key Differentiators:** Decision Matrix, Mandatory Security (OWASP), Rollback Plans.
- **Security:** Transforms the solo developer into a responsible senior software engineer.

---

## 🤖 For Artificial Intelligences

### ⚠️ Mandatory Protocol Reading Instruction

**All protocols begin with a MANDATORY INSTRUCTION requiring 100% comprehension of content before proceeding.**

Every protocol file starts with a prominent notice:

> 📖 **MANDATORY FOR ALL ARTIFICIAL INTELLIGENCES**: If you are reading this protocol, you MUST study and comprehend 100% of its content before proceeding. This is not optional documentation—it is the foundational methodology that defines how you must assist users and their customers.

**What this means:**
- AIs must read **every section, principle, checklist, and guideline**
- Partial understanding leads to incomplete work and user frustration
- Effectiveness depends entirely on mastering the protocol

### 🌐 Multi-AI Communication & Coordination (v3.3+)

**New Feature**: Complete guide for multiple AIs working concurrently on the same project.

When multiple artificial intelligences work simultaneously (e.g., multiple terminal tabs/windows), coordination is **mandatory** to prevent conflicts.

**3 Coordination Options:**

1. **Option A: Shared State via Filesystem** (Simplest, Last Resort)
   - All AIs read/write from `/tmp/ai_coordination.json`
   - Advantages: Simple, no dependencies
   - Disadvantages: Race conditions, not scalable beyond 2-3 AIs

2. **Option B: External Orchestrator** (Recommended for Production)
   - Central Python/Go controller with REST API
   - Maintains shared memory, assigns roles, enforces file locks
   - Advantages: Scalable (10+ AIs), auditable, production-ready
   - Disadvantages: Requires external process, more complex

3. **Option C: tmux + Daemon Controller** (Default for Local Development)
   - Visual coordination surface (1 pane = 1 AI role)
   - Daemon monitors panes, extracts intent, injects context
   - Advantages: Visual feedback, tactile control, local-only
   - Disadvantages: Requires tmux, local machine only

**Fallback Hierarchy:** C → B → A (if setup fails)

**Key Features:**
- ✅ Detection protocols (AI must detect if coordination already exists)
- ✅ Conflict prevention (file locks, git operation retry with exponential backoff)
- ✅ Coordination verification checklist (how to test if working)
- ✅ Network failure handling (automatic fallback)
- ✅ Complete setup instructions (Python/Bash scripts included)

**Where to find:** All 6 protocols include comprehensive Multi-AI Communication & Coordination chapter with:
- Technical reality explanation (why direct AI-to-AI communication is impossible)
- Complete implementation guide for all 3 options
- Troubleshooting & edge cases
- Coordination checklists

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

## 🔍 Binary Search for Bug Localization

> **NEW**: All protocols now include **binary search** methodology for efficient bug and defect localization.

### 📋 What is it?

**Binary search for debugging** is a powerful algorithmic technique that reduces the search space by half with each iteration, allowing you to locate defects in **O(log N) steps** instead of O(N) steps of a linear search.

### 🎯 When to Apply

During error correction, when:
- The error is reproducible but the cause is not obvious
- The codebase is large (>100 lines)
- You suspect the bug is in a specific but broad region
- An error appeared after large changes (multiple commits)

### 💡 How it Works

**Practical Example**: Finding an error on line 48 of a file with 512 lines

1. **Iteration 1**: Comment out half the code (lines 257-512), test the rest
   - Error persists? Bug is in [1-256]
   - Error disappears? Bug is in [257-512]

2. **Iteration 2**: Repeat the process on the identified half
   - Continue dividing: [1-256] → [1-128] → [1-64] → [33-64] → [33-48]...

3. **Result**: 9 iterations to find the bug (vs. up to 512 linear attempts)

### ⚡ Efficiency

| Code Size | Linear Search | Binary Search | Gain |
|-----------|--------------|---------------|------|
| 512 lines | up to 512 steps | 9 steps | **56.9x faster** |
| 1024 lines | up to 1024 steps | 10 steps | **102.4x faster** |
| 4096 lines | up to 4096 steps | 12 steps | **341.3x faster** |

### 🎨 Creative Applications

Binary search is not limited to lines of code. It can be applied to:

- **📦 Dependencies/Imports**: Comment out half the imports to find conflicts
- **🔧 Configurations**: Disable half the configs to find issues
- **🗃️ Data**: Process half the dataset to identify problematic data
- **⚙️ Features**: Disable half the features to locate regressions
- **📅 Git History**: Use `git bisect` to find the commit that introduced the bug
- **🔄 Loop Iterations**: Execute half the iterations to identify issues

### 📖 Where to Find

Each protocol contains a complete section "🔍 Binary Search for Bug Localization" with:
- ✅ Detailed step-by-step methodology
- ✅ Practical examples with code
- ✅ Implementation techniques (comments, flags, git bisect)
- ✅ 11-step checklist
- ✅ Comparative efficiency table
- ✅ Practical tips and rationale

### 🚀 Rationale

**Why is binary search powerful for debugging?**

1. **⚡ Algorithmic Efficiency**: Exponential time savings
2. **🎯 Precise Isolation**: Reduces uncertainty systematically
3. **🧠 Lower Cognitive Load**: Simple decisions (error present: yes/no)
4. **📊 Predictability**: Know exactly how many steps will be needed
5. **🔄 Universal Applicability**: Works for code, data, configs, history
6. **✅ Success Guarantee**: If the bug is reproducible, it always finds it

**Message for AIs:**
> "Creativity in using binary search has no limits. Always consider whether a debugging problem can be reduced to a binary search - you'll save time and find bugs faster."

---

## 📖 Documentation Reading: First Mandatory Action (NEW v2.2/2.4/3.3)

> **🚨 CRITICAL FOR AIs**: Before ANYTHING else, AI **MUST** search for and read **100% of existing local markdown documentation** in the project.

### 🎯 What Changed

Starting from the latest versions (v2.2, v2.4, v3.3), **all three protocols** now include **Step 1.0: Complete Documentation Search and Reading** as **FIRST PRIORITY ACTION** before any task.

### 📋 How it Works

**Step 1: Recursive Search**

AI must search for **ALL** `.md` files in the workspace:
```bash
find . -name "*.md" -type f | grep -v node_modules | grep -v venv
```

**Locations to search**:
- 📂 Root: `README.md`, `TASKS.md`, `CHANGELOG.md`
- 📂 `docs/`: All structured documentation
- 📂 `docs/plans/`: Action plans
- 📂 `docs/ADR/`: Architecture Decision Records (Simplicity 2)
- 📂 `docs/security/`: Security checklists (Simplicity 3)
- 📂 `docs/rollback/`: Rollback plans (Simplicity 3)
- 📂 Any other directory with `.md` files

**Step 2: Complete Reading (100%)**

AI must read **COMPLETELY** all found files:
- ✅ `README.md` - Project overview
- ✅ `TASKS.md` - Pending and completed tasks
- ✅ `docs/REQUIREMENTS.md` - Functional and non-functional requirements
- ✅ `docs/ARCHITECTURE.md` - Architectural decisions and stack
- ✅ `docs/vX.Y.Z-SPECIFICATIONS.md` - Version specifications
- ✅ `docs/CHANGELOG.md` - Change history
- ✅ `docs/plans/*.md` - Action plans
- ✅ `docs/ADR/*.md` - Formal decisions (Enterprise)
- ✅ `docs/security/*.md` - OWASP checklists (Production)
- ✅ Any other `.md` file

**Step 3: If No Documentation Found**

AI **MUST** ask the user:
```markdown
❓ I searched for markdown documentation but found no .md files.

Do you have project documentation?
A) Yes, it's in [specific location]
B) Yes, but in different format
C) No, doesn't exist yet

If C: I'll create the initial documentation structure.
```

**Step 4: Create Initial Documentation (If It Doesn't Exist)**

AI must create minimum mandatory structure:

**Simplicity 1** (Prototypes):
```
README.md
TASKS.md
docs/
├── REQUIREMENTS.md
├── ARCHITECTURE.md
└── v0.1.0-SPECIFICATIONS.md
```

**Simplicity 2** (Enterprise):
```
README.md
TASKS.md
docs/
├── REQUIREMENTS.md
├── ARCHITECTURE.md
├── v0.1.0-SPECIFICATIONS.md
├── ADR/
│   └── template-adr.md
├── security/
│   └── OWASP-checklist.md
└── api/
    └── api-reference.md
```

**Simplicity 3** (Solo in Production):
```
README.md
TASKS.md
docs/
├── REQUIREMENTS.md
├── ARCHITECTURE.md
├── v0.1.0-SPECIFICATIONS.md
├── security/
│   └── OWASP-checklist.md
└── rollback/
    └── rollback-template.md
```

### ✅ Mandatory Checklist (For AIs)

Before starting any task:

```markdown
[ ] 🔍 Searched recursively for all .md files
[ ] 📖 Read 100% of content of ALL found files
[ ] 📝 If not found, asked user
[ ] 📚 If doesn't exist, created minimum structure
[ ] 🎯 Understood complete objective and context
[ ] 📋 Know which tasks are pending
[ ] 🛠️ Know the technology stack
[ ] 🏗️ Understood architectural decisions
[ ] ✅ Ready to work with complete context
```

### 🚀 Rationale: Why Is This CRITICAL?

**For ALL Protocols**:
1. ✅ **Context is Everything**: Code without context is impossible to maintain
2. ✅ **Avoid Duplication**: Don't reimplement existing functionalities
3. ✅ **Previous Decisions**: Understand why choices were made
4. ✅ **Consistency**: Follow already established patterns
5. ✅ **Productivity**: 10 minutes of reading saves hours of rework

**Simplicity 1** (Prototypes):
- ✅ Avoid reintroducing already fixed bugs
- ✅ Maintain style and pattern consistency

**Simplicity 2** (Enterprise):
- ✅ **ADRs are critical**: Formal decisions cannot be ignored
- ✅ **Compliance**: Not following corporate standards blocks deployment
- ✅ **Coordination**: Multiple devs need shared context

**Simplicity 3** (Solo in Production):
- ✅ **External Memory**: Documentation is your "virtual teammate"
- ✅ **No Backup**: There's no one to ask if stuck
- ✅ **Future You**: Document for "future you" (you forget decisions)
- ✅ **Continuity**: If sick/vacation, someone needs to take over

### 💬 Messages for AIs

**Universal Golden Rule**:
> **"Read documentation FIRST, code AFTER. Always. No exceptions."**

**Simplicity 1**:
> "10 minutes of reading saves hours of rework."

**Simplicity 2**:
> "In enterprise, documentation is not optional - it's MANDATORY and FORMAL. Read 100% of ADRs BEFORE coding."

**Simplicity 3**:
> "For solo developers, documentation is CRITICAL. You don't have a team. Document as if you'd be hit by a bus tomorrow."

### 📊 Code Comments

Besides markdown documentation, AI must add **useful comments** in code:

**WHAT to document in comments**:
- ✅ **Why** the code was written this way (not just "what" it does)
- ✅ **Non-obvious decisions**: Why chose approach X instead of Y
- ✅ **Edge cases**: Why certain special cases are handled
- ✅ **TODOs**: What's missing to implement or can be improved

**Useful comment example**:
```python
# DECISION: We use in-memory cache instead of Redis because:
# 1. Project scale doesn't justify complexity
# 2. Small data (<10MB) doesn't need to persist
# 3. Fast startup is priority
cache = {}

# TODO: If scale exceeds 100k records, migrate to Redis
# Estimate: ~2h work, create rollback plan first
```

📖 **Complete details**: See Step 1.0 of each protocol for templates, commands, and specific examples.

---

## 🔍 Technology Research for Projects (NEW v2.1/2.3/3.2)

> **CRITICAL**: All protocols now include **mandatory Step 1.5** for research and recommendation of appropriate technologies at project start.

### 📋 What Changed

Starting from the latest versions (v2.1, v2.3, v3.2), **all three protocols** now include **Step 1.5: Technology Research for Projects** as **MANDATORY at start**.

### 🎯 When to Apply

**Ideal timing**: Right after first reading of `TASKS.md` and `docs/REQUIREMENTS.md`, **before starting implementation**.

**Applicable to**:
- ✅ New projects (no code implemented yet)
- ✅ Complete refactoring projects (technology stack change)
- ✅ Planning phase projects (architecture not yet defined)

**NOT applicable to**:
- ❌ Projects with already defined stack and implementation in progress
- ❌ Functionality maintenance in existing code
- ❌ Bug fixes in already produced code

### 📦 How it Works

**Step 1: AI collects developer requirements**
- Desired tasks and functionalities (may be in `docs/TASKS.md`)
- Functional and non-functional requirements
- Application type (web, desktop, mobile, CLI, API)
- Target audience and expected scale
- Technical constraints

**Step 2: AI investigates professional technologies**

AI researches (online if necessary) which technologies are **widely used professionally** for similar projects:

**Categories covered**:
1. **🎨 Frontend**: React, Vue, Angular, Next.js, MUI, Bootstrap, Tailwind CSS
2. **⚙️ Backend**: Python (FastAPI, Django), Node.js (Express, NestJS), Java (Spring Boot)
3. **🖥️ Desktop**: PyQt, Electron, Tauri, Qt, WPF
4. **📊 Data Visualization**: Chart.js, D3.js, Plotly, pyqtgraph, Recharts
5. **🤖 AI/ML**: TensorFlow, PyTorch, Transformers (Hugging Face), OpenAI API, Gemini API
6. **💾 Database**: PostgreSQL, MySQL, MongoDB, Redis, SQLite
7. **🔐 Authentication & Security**: OAuth, JWT, Auth0, Keycloak
8. **🧪 Testing**: pytest, Jest, Cypress, Playwright

**Step 3: AI presents 2-3 complete recommended stacks**

With detailed justifications:
- ✅ Why each technology is appropriate
- ✅ Real use cases (companies/projects using it)
- ✅ Advantages and disadvantages
- ✅ Learning complexity
- ✅ Estimated setup time

**Step 4: Validation and documentation**

- ✅ Developer chooses final stack
- ✅ AI documents in `docs/ARCHITECTURE.md`
- ✅ [Enterprise] Create ADR (Architecture Decision Record)

### 🌐 Online Research

AI **can and should do online research** when necessary:

**Recommended sources**:
- 📚 **GitHub**: Similar repositories, analysis of stars/forks
- 📖 **Official documentation**: Official technology sites
- 💬 **Stack Overflow**: Discussions about comparisons and best practices
- 📊 **Stack Share**: Companies using each technology
- 📰 **Technical blogs**: Medium, Dev.to, company blogs

**What to search**:
- "Best [app type] stack 2025"
- "[Language] frameworks for [app type]"
- "[Technology X] vs [Technology Y] comparison"
- "Companies using [Technology Z]"
- "[Framework W] production readiness"

### 📋 Differences per Protocol

#### 📘 **Simplicity 1** (Prototypes/Learning)
- Focus on **productivity** and **ease of learning**
- Recommends **modern and popular** technologies
- Basic documentation in `docs/ARCHITECTURE.md`

#### 📕 **Simplicity 2** (Enterprise/Teams)
- Focus on **corporate standards** and **enterprise support**
- Validation with **team** (technical decision meeting)
- **Mandatory ADR** (Architecture Decision Record)
- Analysis of **licensing cost** and **compliance**
- **Stakeholder** approval

#### 📗 **Simplicity 3** (Solo in Production)
- Focus on **maturity** and **ease of maintenance**
- Prioritizes **LTS versions** (Long Term Support)
- Evaluates **"boring technology"** (stable and predictable technologies)
- Analysis of **longevity** (5+ years)
- **Mandatory rollback plan**
- Specific research for solo developers (Indie Hackers, Reddit r/solopreneur)

### 🎯 Practical Examples

**Example 1: Data Analysis Dashboard**
- **Requirements**: Web dashboard, dynamic charts, REST API
- **Recommended Stack**: React + Recharts + FastAPI + PostgreSQL
- **Justification**: Modern stack, productive, excellent for visualization

**Example 2: Desktop Signal Processing Application**
- **Requirements**: Native desktop interface, real-time charts, offline
- **Recommended Stack**: PyQt6 + pyqtgraph + NumPy
- **Justification**: Native performance, pyqtgraph optimized for real-time

**Example 3: API with Generative AI**
- **Requirements**: REST API, NLP processing, AI model integration
- **Recommended Stack**: NestJS + Transformers + Gemini API + MongoDB
- **Justification**: Scalable NestJS, asynchronous support for AI APIs

### ✅ Checklist for AIs

Before starting implementation:

```markdown
[ ] Project requirements collected
[ ] Professional technologies investigation performed
[ ] 2-3 complete stacks recommended with justifications
[ ] Advantages and disadvantages presented
[ ] Real use cases cited
[ ] Learning complexity evaluated
[ ] Validation with developer/team performed
[ ] Final stack chosen and confirmed
[ ] Stack documented in docs/ARCHITECTURE.md
[ ] Online research performed (if necessary)
```

### 🚀 Rationale

**Why is this step mandatory at start?**

1. ✅ **Avoid Rework**: Choosing wrong stack requires rewriting all code
2. ✅ **Professional Quality**: Appropriate technologies ensure production-ready code
3. ✅ **Productivity**: Modern and well-supported stack accelerates development
4. ✅ **Maintainability**: Popular technologies have more resources and community
5. ✅ **Scalability**: Appropriate stack grows with project without migration
6. ✅ **Contextual Knowledge**: AI can recommend technologies developer doesn't know

**Message for AIs**:
> "Don't assume developer already knows all options. Your research and recommendation can introduce modern and more appropriate technologies. Investing 30 minutes in this investigation can save weeks of rework."

**Golden Rule**:
> **"Technology stack MUST be defined BEFORE the first line of code. Subsequent changes are costly."**

📖 **Complete details**: See Step 1.5 of each protocol for detailed templates, checklists, and specific examples.

---

## 🌐 Default Recommended Stack for Websites/Web Applications (NEW v2.3/2.5/3.4)

> **IMPORTANT**: When implementing a **website or web application**, and user **DOES NOT specify** which technologies they want, AI **CAN RECOMMEND** the following modern and complete default stack.

### 📦 Complete Stack

**Frontend Framework & Runtime**:
- Next.js 15.5.2 + React 19.1.1 + TypeScript 5.9.2
- Node.js 18+ (LTS)

**Build & Styling**:
- Turbopack (bundler 700x faster)
- Tailwind CSS 3.4.17
- Zustand 4.5.7 (state management)

**Optional Integrations**:
- Cloudinary (media)
- Stripe (payments)
- OpenAI/ElevenLabs (AI)
- Puppeteer (PDFs)

**Testing & Quality**:
- Jest + @testing-library
- ESLint + Husky

**Deploy**:
- Vercel (free frontend)
- Heroku (backend)

### ✅ Why This Stack?

- ✅ **Next.js 15**: Mature framework, SSR/SSG, optimized SEO
- ✅ **React 19**: Massive community, Server Components
- ✅ **TypeScript**: Type safety, fewer production bugs
- ✅ **Turbopack**: Build 700x faster than Webpack
- ✅ **Tailwind**: High productivity, consistent design
- ✅ **Vercel**: Free deploy, optimized for Next.js
- ✅ **Complete Ecosystem**: Covers 90% of web use cases

### 📋 Differences per Protocol

**Simplicity 1** (Prototypes):
- Recommended stack as initial suggestion
- Focus on productivity and learning
- Basic documentation in `docs/ARCHITECTURE.md`

**Simplicity 2** (Enterprise):
- **Mandatory validation**: Technical meeting + formal ADR
- Corporate cost and compliance analysis
- TypeScript mandatory for teams
- Use cases: Netflix, TikTok, Uber use Next.js
- Commercial Vercel support available

**Simplicity 3** (Solo in Production):
- Focus on **low maintenance**: ~15h/month sustainable
- Free scalable deploy
- Exceptional documentation and massive community
- **Mandatory rollback plan** (3 alternatives)
- Estimated maintenance time

### ⚠️ When NOT to Use This Stack

- ❌ User/team explicitly specifies other technologies
- ❌ Project requires Vue/Angular instead of React
- ❌ Needs Python/Django backend
- ❌ Desktop or native mobile application
- ❌ Super simple static site (pure HTML/CSS/JS sufficient)
- ❌ **[Enterprise]** Mandatory corporate stack
- ❌ **[Solo]** Developer prefers "boring technology" (PHP, Rails)

### 🎯 Presentation Example

```markdown
❓ You didn't specify technologies for the website. Can I recommend a modern stack?

**Recommended Default Stack (Next.js 15 + React 19 + TypeScript)**:
- Next.js 15.5.2 (optimized SSR/SSG)
- React 19.1.1 + TypeScript 5.9.2
- Tailwind CSS 3.4.17
- Free deploy on Vercel

**Why?**
✅ Exceptional performance (Turbopack 700x faster)
✅ Optimized SEO
✅ TypeScript ensures quality
✅ Free and simple deploy

**Do you agree or prefer another stack?**
```

### 📊 Complete Versions with Detailed Stack

To see the complete list of versions for each package (80+ dependencies), consult **Step 1.5** of each protocol, section "Default Recommended Stack for Websites/Web Applications".

This includes detailed lists of:
- **Frontend Framework & Runtime** (Next.js, React, TypeScript, Node.js)
- **Bundlers & Build Tools** (Turbopack, Turbo, PostCSS, Autoprefixer, Webpack)
- **State Management** (Zustand, Immer, DevTools, Persist Middleware)
- **Styling** (Tailwind CSS, CSS Modules, clsx, class-variance-authority, tailwind-merge, Lucide React)
- **Audio & Media** (Cloudinary, Web Audio API, MediaRecorder API)
- **Payments & Subscriptions** (Stripe)
- **HTTP & API** (Axios, Fetch API)
- **PDF & Screenshots** (jsPDF, html2canvas, Puppeteer)
- **Testing** (Jest, jsdom, @testing-library)
- **Code Quality & Linting** (ESLint, Husky)
- **Development Tools** (npm, Git, VS Code, Chrome DevTools)
- **Backend** (Node.js, Express, MongoDB, JWT, Heroku)
- **Infrastructure & Deploy** (Vercel, Cloudinary CDN, HTTPS)
- **Browser APIs** (Web Audio, MediaRecorder, Fetch, Cookies, LocalStorage, Navigator, Permissions, Geolocation, Service Worker)
- **AI APIs** (OpenAI GPT-4o-mini, ElevenLabs)

📖 **Complete details**: See specific section in Step 1.5 of each protocol (after technology categories).

---

## 🎨 Mandatory Requirement: Project Icons (NEW v2.3/2.5/3.4)

> **NEW**: All protocols now require AI to produce or download appropriate icons for each project.

### 📋 What Changed

Starting from the latest versions, **all three protocols** now include **Step 6.6: Project Icons** as **MANDATORY** requirement.

### 🎯 When to Apply

During **Step 6 (Implementation)**, after defining the project's basic structure.

### 🎨 What is Required

AI must:
1. **Ask the programmer** if they already have an icon
2. **Create simple icon** (SVG with project initials) OR
3. **Download free icon** (from verified sources: Heroicons, Lucide, Tabler, Iconoir)
4. **Convert to necessary formats** (favicon.ico, SVG, PNG in multiple sizes)
5. **Organize in dedicated folder** (`assets/icons/` preferred)
6. **Integrate into project** (HTML, manifest.json, application code)

### 📁 Formats by Technology

- **Web**: favicon.ico, icon.svg, icon-192.png, icon-512.png, apple-touch-icon.png
- **Desktop**: icon.png (256x256, 512x512), icon.ico (Windows), icon.icns (macOS)
- **Mobile**: icon.png (1024x1024), ic_launcher.png (varied Android densities)

### ⏱️ Estimated Time
**15-30 minutes** per project - small investment, big impact on quality perception.

### 🎯 Rationale
- ✅ **Professionalism**: Projects without icon seem incomplete
- ✅ **Visual Identity**: Users recognize app by icon (branding)
- ✅ **UX**: Facilitates locating app among multiple tabs/windows
- ✅ **Platform Requirements**: App stores REQUIRE icons
- ✅ **PWA**: Browsers request icons for installation

📖 **Complete details**: See Step 6.6 of each protocol for conversion tools, integration examples, validation checklist, and free resources.

---

## 📧 Mandatory Requirement: Feedback Contact Methods (NEW v2.3/2.5/3.4)

> **NEW**: All protocols now require AI to ask developer about including contact methods for user feedback, with **GitHub as default recommendation**.

### 📋 What Changed

Starting from the latest versions, **all three protocols** now include a mandatory question about **Contact Methods for User Feedback** during the first session, with **GitHub Issues/Discussions as default recommendation** instead of email.

### 🎯 When to Apply

During the **first session** of interaction with the programmer, right after defining code language preferences.

### 📧 What is Required

AI must:
1. **Ask the programmer** if they want to include contact methods
2. **Recommend GitHub as default** (Issues/Discussions) for receiving all types of feedback
3. **Offer alternatives**: Email, contact form, multiple channels
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

### 🎯 Why GitHub as Default?

**Advantages over email**:
- ✅ **Public Tracking**: Other users can see and contribute to discussions
- ✅ **Issue Organization**: Labels, milestones, assignees, projects
- ✅ **Version Control Integration**: Link commits to issues
- ✅ **Community Building**: Encourages open collaboration
- ✅ **Searchable History**: Users can search before creating duplicate issues
- ✅ **No Spam**: GitHub filters and requires account
- ✅ **Markdown Support**: Rich formatting for technical discussions

**When to use email instead**:
- ❌ Private/confidential projects (no public repository)
- ❌ Non-technical users (prefer simpler contact)
- ❌ Security vulnerability reports (should be private)

### 🎯 Rationale
- ✅ **Continuous Improvement**: Direct feedback identifies problems and opportunities
- ✅ **Engagement**: Users feel more connected when they can contribute
- ✅ **Quality**: Criticisms and suggestions improve software
- ✅ **Prioritization**: Feedback helps understand what is important
- ✅ **Motivation**: Compliments motivate the development team
- ✅ **Professionalism**: Open channel demonstrates commitment to users
- ✅ **Transparency**: Public issues build trust with community

### 📝 Implementation Example

```markdown
## 📮 Feedback and Contact

We'd love to hear from you! Share your comments, suggestions, 
criticisms, complaints, compliments, and opinions:

- **GitHub Issues**: [github.com/username/project/issues](https://github.com/username/project/issues) (recommended)
- **GitHub Discussions**: [github.com/username/project/discussions](https://github.com/username/project/discussions)
- **Email**: feedback@myproject.com (for private matters)
- **Response time**: We typically respond within 48 hours

Your feedback helps us improve continuously!
```

### ⏱️ Estimated Time
**5-10 minutes** to add to README - minimal investment for essential communication channel.

📖 **Complete details**: See "Contact Methods for User Feedback" section in each protocol for complete options, form examples, privacy policies, and best practices.

---

## 📊 Ordinal Task Organization (NEW v2.3/2.5/3.4)

> **NEW**: Ordinal prefix system to identify dependencies, priorities, and parallelization opportunities.

### 🎯 What Is It

The **Ordinal Task Organization** is a prefix system that enables:
- ✅ Clear **execution order** (from simplest to most complex)
- ✅ Explicit **dependencies** (which tasks need to be done first)
- ✅ Intelligent **parallelization** (which can be developed simultaneously)
- ✅ **Hierarchical organization** (tree/graph structure)

### 📋 3-Level System

**Level 1: Simple Numbering** (independent tasks)
```markdown
1. Setup development environment
2. Create initial documentation
3. Define system architecture
```
→ Can be executed in **any order** or **in parallel**

**Level 2: Hierarchy with Letters** (task groups)
```markdown
A. Infrastructure
   A.1. Create directory structure
   A.2. Configure dependencies

B. Core - Data Structures
   B.1. Implement Node class
   B.2. Implement ExpressionTree
```
→ Different groups (A, B) are **PARALLEL**

**Level 3: Deep Hierarchy** (complex dependencies)
```markdown
B.C.2. Implement tree → RPN conversion
   B.C.2.1. RPN Parser (do FIRST - leaf)
   B.C.2.2. RPN Serializer (do FIRST - leaf)
   B.C.2. Complete conversion (do AFTER - parent)
```

### 🔄 Hierarchy Reading (⭐ CRITICAL)

Hierarchy must be read from **RIGHT to LEFT**:

```
C.B.1.D.1
   │  │ │ └─ 1: Execute LAST (tree root)
   │  │ └─── D: Execute THIRD
   │  └───── 1: Execute SECOND
   └──────── B: Execute FIRST (tree leaf)

Execution order: B → 1 → D → 1 (right to left)
```

### 🎨 Practical Example

```markdown
## 🔴 MUST HAVE - Release v1.0.0

A. Authentication (Owner: Backend)
   🔴🟡 [ ] A.1. User Model (1.5h)
   🔴🟡 [ ] A.2. JWT Login (2h) - Depends: A.1
   🔴🔴 [ ] A.3. 2FA (3h) - Depends: A.2

B. Catalog (Owner: Backend)
   🔴🟢 [ ] B.1. Product Model (1h)
   🔴🟡 [ ] B.2. CRUD Products (2h) - Depends: B.1

**Parallelization Analysis**:
- A.1 and B.1: PARALLEL (different groups) ✅
- A.1 → A.2 → A.3: SERIAL (dependencies) ❌
- B.1 → B.2: SERIAL (dependencies) ❌

**Branch Strategy**:
- Branch feat/auth: A.1 → A.2 → A.3
- Branch feat/catalog: B.1 → B.2 (parallel with auth)
```

### ✅ Benefits

**For Developers**:
- ✅ Clarity about execution order
- ✅ Autonomy to choose parallel tasks
- ✅ Fewer conflicts in Git/GitHub

**For AIs**:
- ✅ Automatic calculation of execution order
- ✅ Parallelization suggestion
- ✅ Circular dependency detection

**For the Project**:
- ✅ 40-60% reduction in total time (parallelization)
- ✅ Avoid rework (correct order)
- ✅ More predictable timeline

### 📚 Complete Documentation

This system is integrated into all three protocols:

- **📘 Protocol 1**: Section 2.5 - System [OPTIONAL] for simple projects
- **📕 Protocol 2**: Section 2.6 - System [HIGHLY RECOMMENDED] for team coordination
- **📗 Protocol 3**: Section 2.6 - System [RECOMMENDED] for solo developers in production

📖 **Detailed Documentation**:
- [`en/ORDINAL_TASK_ORGANIZATION.md`](ORDINAL_TASK_ORGANIZATION.md) - Complete guide in English
- [`pt/ORGANIZACAO_ORDINAL_TAREFAS.md`](../pt/ORGANIZACAO_ORDINAL_TAREFAS.md) - Guia completo em Português

Includes:
- ✅ Decision flowchart
- ✅ 3 practical examples (simple, medium, complex)
- ✅ Instructions for developers and AIs
- ✅ Integration with CI/CD tools
- ✅ Granular rollback strategies

---

## 💻 Mandatory Code Comments (NEW v2.3/2.5/3.4)

> **CRITICAL**: All implemented code **MUST** include useful comments for documentation purposes.

### 📋 What Changed

All protocols now require that **all code implemented** in programming languages that support comments **MUST be commented** for documentation purposes.

### 🎯 Commenting Standard

**Example in Python**:
```python
VirtualGraph.execute() # This command executes features of the graphical environment to display the Cartesian planes of the virtualGraph.py module.
```

### 📝 What to Comment

- ✅ **Why** the code was written this way (not just "what" it does)
- ✅ **Non-obvious decisions**: Why chose approach X instead of Y
- ✅ **Edge cases**: Why certain special cases are handled
- ✅ **Function/method purpose**: What it does at high level
- ✅ **Parameters and return values**: What they mean
- ✅ **TODOs**: What's missing to implement or can be improved

### 🎯 Rationale

- ✅ **Documentation**: Code becomes self-documenting
- ✅ **Maintainability**: Future developers (including "future you") understand intent
- ✅ **Onboarding**: New team members learn faster
- ✅ **Debugging**: Comments help identify where things went wrong
- ✅ **Knowledge Transfer**: Critical for solo developers and team transitions

📖 **Complete details**: See code commenting guidelines in Step 6 (Implementation) of each protocol.

---

## 🔀 Parallel Options Implementation (NEW v2.3/2.5/3.4)

> **NEW**: When multiple parallel options exist that can be reconciled, suggest implementing both with user choice.

### 📋 What Is It

During code implementation, when there are **multiple parallel options** where it's possible to **reconcile both** by implementing them, the AI should **suggest this approach**.

### 🎯 Example

**Scenario**: Results can be shown in **table mode** OR **tree mode** for files and their content.

**Traditional approach**: Choose one and discard the other.

**Parallel approach**: Implement both and let user choose which to use!

### ⚠️ Important

The user **MUST be notified before** implementing such reconciliation, so it's not treated as extraneous information from the software artifact defect taxonomy.

### 🎯 Rationale

- ✅ **User Choice**: Users get more flexibility
- ✅ **Better UX**: Different users prefer different formats
- ✅ **Future-proof**: Covers more use cases
- ✅ **Professional**: Commercial software often offers multiple views

📖 **Complete details**: See parallel options guidelines in implementation steps of each protocol.

---

## 📚 Documentation as Blocking Priority (NEW v2.3/2.5/3.4)

> **CRITICAL**: Documentation must be considered **blocking priority** in software implementation.

### 📋 Priority Hierarchy

Documentation is **blocking** when documentation is needed. Priority order:

1. 🔴 **HIGHEST BLOCKING**: Asking questions when AI has doubts
2. 🟠 **HIGH BLOCKING**: **Documentation** (when needed)
3. 🟡 **MEDIUM BLOCKING**: Bug fixes
4. 🟢 **NORMAL**: New feature implementation

### 🎯 What This Means

- ✅ AI **MUST** document before continuing to next feature
- ✅ Documentation is **not optional** - it's **mandatory**
- ✅ Missing documentation **blocks** progress
- ✅ Documentation quality is **as important** as code quality

### 🎯 Rationale

- ✅ **Maintainability**: Undocumented code is unmaintainable
- ✅ **Knowledge Transfer**: Critical for team continuity
- ✅ **Onboarding**: New developers need documentation
- ✅ **Solo Developer Safety**: "Future you" needs to remember decisions
- ✅ **Professionalism**: Professional projects have professional documentation

📖 **Complete details**: See documentation priority guidelines in all protocols.

---

## 🎯 Sprints, Action Plans, and Task Organization (NEW v2.3/2.5/3.4)

> **CRITICAL**: AI must create sprints, action plans, document tasks in TASKS.md, and organize work with intermediate tasks and structured sequencing.

### 📋 What Changed

All protocols now **require** that AI:
1. **Create sprints** for organizing work in iterations
2. **Create action plans** for complex tasks (detailed in previous section)
3. **Document tasks in TASKS.md** for tracking and organization
4. **Define intermediate tasks** to break down complex work
5. **Structure sequencing** to organize dependencies and priorities

### 🎯 How It Works

**Step 1: Read Documentation**
- AI reads 100% of project documentation first (Step 1.0)

**Step 2: Define Tasks**
- AI documents all required functionalities in `docs/TASKS.md`
- Uses ordinal organization for dependencies (if applicable)
- Classifies by status, complexity, and priority (MoSCoW)

**Step 3: Create Action Plans**
- For complex tasks, AI creates detailed action plans
- Breaks down into intermediate steps
- Defines completion criteria for each step

**Step 4: Organize Sprints**
- Groups related tasks into sprints
- Prioritizes based on dependencies and urgency
- Defines sprint goals and deliverables

**Step 5: Execute and Track**
- AI executes tasks following the plan
- Updates task status in TASKS.md
- Marks action plan progress
- Documents completed work in docs/

### 🎯 Why This Is Important

- ✅ **Better Organization**: Clear structure for complex work
- ✅ **Predictability**: Know what's next and why
- ✅ **Traceability**: History of what was done and why
- ✅ **Continuity**: Easy to resume if interrupted
- ✅ **Quality**: Systematic approach reduces errors
- ✅ **Professionalism**: Structured development process

### 📝 Example Sprint Structure

```markdown
## 🚀 Sprint 1: Foundation (Week 1)

**Goal**: Setup project infrastructure and core data structures

**Tasks**:
- [x] A.1. Create directory structure (Done)
- [x] A.2. Configure dependencies (Done)
- [ ] B.1. Implement Node class (In Progress)
- [ ] B.2. Implement ExpressionTree (Not Started)

**Deliverable**: Working infrastructure + core classes with tests
```

### 🎯 Rationale

- ✅ **Software must be well-structured** before implementation
- ✅ **AI needs organization** to work effectively
- ✅ **Planning reduces rework** and improves quality
- ✅ **Documentation enables continuity** across sessions
- ✅ **Structured approach** scales better

📖 **Complete details**: See sprint and planning guidelines in Step 2 (Planning) of each protocol.

---

## 📝 Editable Questionnaires for User Input (NEW v2.3/2.5/3.4)

> **NEW**: When AI provides questions, they should be documented in editable format for user to fill out manually, then AI reads the filled document.

### 📋 How It Works

**Step 1: AI Creates Questionnaire**
AI documents questions in a file (e.g., `docs/QUESTIONS.md`) in an editable format.

**Step 2: User Fills Out**
User manually fills out the questionnaire in their text editor.

**Step 3: AI Reads Answers**
After user confirms completion, AI reads the filled document to gather answers.

### 📝 Questionnaire Format

AI should provide recommendations and make it easy to fill out. Example:

```markdown
### 🎯 QUESTION 3: SITE OBJECTIVE AND SCOPE

**❓ What is the main objective of this full-stack site?**

💡 **AI Suggestion**: Define clearly to guide architecture decisions

**Options (mark all that apply):**
- **A)** ✅ Portfolio/Personal or company presentation
- **B)** ✅ E-commerce/Virtual store
- **C)** ✅ Blog/Content system
- **D)** ✅ Dashboard/Admin panel
- **E)** ✅ REST API for external consumption
- **F)** ✅ Authentication/User system
- **G)** ✅ SaaS application (Software as a Service)
- **H)** ⚙️ Other: _____

**Your choices:** _______
```

### 🎯 Benefits

- ✅ **Async Communication**: User can answer when convenient
- ✅ **Thoughtful Answers**: User has time to think
- ✅ **Clear Format**: Structured questions are easier to answer
- ✅ **Documentation**: Questions and answers become part of project docs
- ✅ **AI Recommendations**: AI provides context and suggestions

### 🎯 Rationale

- ✅ **Better UX**: Text editor is more comfortable than chat for long forms
- ✅ **Complete Answers**: Users provide more detail when not rushed
- ✅ **Permanent Record**: Answers are documented for future reference
- ✅ **Asynchronous**: User and AI don't need to be synced

### 💡 Important

AI **should provide recommendations** based on project understanding and what it perceives as user needs. This helps guide decisions and ensures better outcomes.

📖 **Complete details**: See questionnaire guidelines in requirement gathering steps of each protocol.

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

Action plans can be organized in two ways:

#### **Option 1: Consolidated File** `docs/ACTION_PLANS.md`
**Location**: `docs/ACTION_PLANS.md` (same directory as TASKS.md)  
**Usage**: All action plans in a single file, separated by sections

#### **Option 2: Individual Plans Directory** `docs/plans/`
**Location**: `docs/plans/` (dedicated directory for individual plans)  
**Usage**: Each action plan in its own file, facilitating organization and versioning  
**Recommended structure**:
```
docs/
├── TASKS.md                    # General task list
├── ACTION_PLANS.md            # [OPTIONAL] Index/summary of plans
└── plans/                     # Individual plans directory
    ├── plan-001-oauth2.md     # Action plan #001
    ├── plan-002-migration.md  # Action plan #002
    └── plan-003-refactoring.md # Action plan #003
```

**Recommendation**: For projects with multiple complex tasks, use `docs/plans/` for better organization. For smaller projects, `ACTION_PLANS.md` is sufficient.

**Action Plan Template:**

```markdown
# Action Plans - [Project Name]

## 🎯 ACTION PLAN #[ID]: [Objective Title]

**📅 Date**: YYYY-MM-DD  
**🕐 Time**: HH:MM  
**⚡ Priority**: 🔴 Critical | 🟡 High | 🟢 Normal  
**🏷️ Type**: Maintenance | Correction | Evolution | Adaptation  
**⏱️ Estimate**: [total estimated time]  
**📌 Task ID**: Task #X from TASKS.md (mandatory link)  
**🎯 Main Function**: [Main objective of this plan]  
**📋 Desired Requirement**: [What needs to be achieved]  
**✅ Expected Result**: [Measurable success criteria]

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

### 📝 Mandatory Action Plan Fields

Each action plan **MUST** contain the following mandatory fields:

1. **📅 Date** (YYYY-MM-DD): Plan creation date
   - Allows tracking when plan was elaborated
   - Facilitates temporal analysis of recurring problems

2. **🕐 Time** (HH:MM): Plan creation time
   - Useful for work sessions and duration estimates
   - Helps identify productivity patterns

3. **🎯 Main Function**: Main objective of the action plan
   - Describes concisely what the plan aims to achieve
   - Ex: "Implement OAuth2 authentication", "Fix memory leak", "Migrate to PostgreSQL"

4. **📋 Desired Requirement**: What needs to be achieved
   - Specifies functional and non-functional requirements
   - Ex: "Authentication via Google and GitHub with refresh tokens"

5. **✅ Expected Result**: Measurable success criteria
   - Defines how to measure implementation success
   - Ex: "System authenticates users in < 2s, tokens expire in 24h"

6. **📌 Task ID**: Link with TASKS.md (mandatory)
   - Identifies the related task from TASKS.md
   - Ex: "Task #42", "Bug #127", "Feature #15"
   - **CRITICAL**: Ensures traceability between planning and execution

**Why are these fields mandatory?**
- ✅ **Traceability**: Clear link between TASKS.md and action plans
- ✅ **Temporal Context**: Date/time help understand urgency and history
- ✅ **Objective Clarity**: Main function, requirement, and result eliminate ambiguities
- ✅ **Maintainability**: Future developers understand the "why" and "what" was done
- ✅ **Quality**: Success criteria force thinking about validation

### 📁 Naming Convention for docs/plans/

When using the `docs/plans/` directory, follow this naming convention:

**Format**: `plan-[ID]-[descriptive-slug].md`

**Examples**:
```
docs/plans/plan-001-oauth2-authentication.md
docs/plans/plan-042-memory-leak-fix.md
docs/plans/plan-127-postgresql-migration.md
```

**Rules**:
- **ID**: Sequential 3-digit number (001, 002, 003...)
- **Slug**: Short description in kebab-case (lowercase, separated by hyphens)
- **Maximum 50 characters** in filename for easy navigation

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
3. Create detailed Action Plan:
   - Option A: Add to docs/ACTION_PLANS.md
   - Option B: Create file in docs/plans/plan-[ID]-[name].md
4. BEFORE starting implementation: review and validate plan
5. Execute step by step, marking progress in plan
6. Consult plan whenever necessary during implementation
7. Upon completion, mark task in TASKS.md as complete
8. Archive completed plan (move to history or docs/plans/archive/)
```

**Importance of Creating Plan BEFORE**:
- ✅ **Anticipatory Planning**: Identifies problems before coding
- ✅ **Accurate Estimates**: Detailed steps improve time estimates
- ✅ **Avoid Rework**: Thinking before implementing saves time
- ✅ **Reliable Guide**: Serves as map throughout implementation
- ✅ **Living Documentation**: Useful for maintenance and future updates

**Consult Plan Whenever Necessary**:
- 📖 **During Implementation**: To not get lost among steps
- 🔄 **When Resuming Work**: Know exactly where you stopped
- 🤝 **In Meetings**: Communicate progress based on concrete steps
- 🐛 **During Debug**: Review if all steps were followed correctly

### 🎯 Benefits of Action Plans

- ✅ **Clarity**: Breaks complex problems into manageable steps
- ✅ **Traceability**: Detailed history of how it was resolved
- ✅ **Continuity**: Easy to resume where left off if interrupted
- ✅ **Learning**: Documents resolution process for future reference
- ✅ **Quality**: Forces review of each step before proceeding
- ✅ **Communication**: Facilitates explaining progress to stakeholders

### ⏱️ When to Discard an Action Plan

After completion, you can:
1. **Move to "📚 Completed Plans History" section** (if using ACTION_PLANS.md)
2. **Archive in dedicated directory**: 
   - `docs/plans/archive/[year]/plan-[id].md`
   - Or `docs/action_plans_history/[year]/plan-[id].md`
3. **Keep in docs/plans/** (if plan has reference value)
4. **Delete** (only if no historical value - not recommended)

**Recommendation**: Keep history of complex plans in `docs/plans/archive/` for:
- ✅ Future consultation when implementing similar features
- ✅ Analysis of recurring problem patterns
- ✅ Onboarding of new developers (real examples)
- ✅ Documentation of important technical decisions

### 📊 Complete Real Example

```markdown
## 🎯 ACTION PLAN #003: Fix Memory Leak in Cache System

**📅 Date**: 2025-12-26  
**🕐 Time**: 14:30  
**⚡ Priority**: 🔴 Critical  
**🏷️ Type**: Correction  
**⏱️ Estimate**: 4-6 hours  
**📌 Task ID**: Bug #127 from TASKS.md  
**🎯 Main Function**: Eliminate memory leak in Redis cache module  
**📋 Desired Requirement**: Stable memory consumption without growth over time  
**✅ Expected Result**: Stable memory < 300MB for 48h continuous operation

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

**Location of this plan**: `docs/plans/plan-003-memory-leak-fix.md`

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

## 🧠 Associative Memory Factor

> **INTEGRATED**: Fundamental concept to enable AI to learn from error patterns and apply accumulated knowledge.

The **Associative Memory Factor** is now **fully integrated** into all three Simplicity Protocols, allowing AI to develop a "memory" of problems and solutions.

### 🎯 What is it?

AI's ability to:
- 🧠 **Recognize patterns** recurring in errors
- 🔗 **Associate causes and effects** in different contexts
- 📈 **Generalize solutions** from specific cases to general rules
- 📉 **Deduce problems** from general to specific (top-down)
- 📊 **Induce rules** from specific to general (bottom-up)

### 🐍 Connection with Python Traceback

Python's Traceback presents errors in **top-down** structure (from outside to inside):
- **Root** (orchestrator) → **Branches** (coordinators) → **Leaves** (executors)
- Investigation follows the same deductive path
- Associative memory helps identify level and root cause quickly

### 🔬 Complementary Approaches

**Deductive (General → Specific)**:
- Apply known general rules to diagnose error
- Example: "AttributeError usually indicates uninitialized object"

**Inductive (Specific → General)**:
- Observe repeated specific cases to create general rule
- Example: "70% of IndexError are from incorrect index manipulation"

**Neuro-Symbolic (Combination)**:
- Unites deduction (symbolic AI) with induction (neural AI)
- Learns continuously while applying established rules

### 🐛 Defect Taxonomy

Five categories of highly undesirable defects:

1. **Incorrect Fact**: Wrong or outdated information in code
2. **Extraneous Information**: Code/comments that don't belong to context
3. **Ambiguity**: Code that can be interpreted in multiple ways
4. **Inconsistency**: Violation of established project patterns
5. **Omission**: Missing code or logic (validations, error handling)

### 🔄 Error Patterns

**Input-Independent Errors**:
- Always occur, regardless of data
- Indicate structural problem in logic

**Specific Scope Errors**:
- Confined to specific module/function
- One bug, multiple symptoms

**Common Import Errors**:
- Multiple modules fail because they import buggy code
- Fix once resolves all cases

### 📖 Where to Find

The **complete Associative Memory Factor documentation** is now integrated into each protocol:

- **📘 Simplicity Protocol 1** (in English): Section "Associative Memory Factor - Complete Documentation"
- **📕 Simplicity Protocol 2** (in English): Section "Associative Memory Factor - Complete Documentation"  
- **📗 Simplicity Protocol 3** (in English): Section "Associative Memory Factor - Complete Documentation"

- **📘 Protocolo Simplicidade 1** (em português): Seção "Fator de Memória Associativa - Documentação Completa"
- **📕 Protocolo Simplicidade 2** (em português): Seção "Fator de Memória Associativa - Documentação Completa"
- **📗 Protocolo Simplicidade 3** (em português): Seção "Fator de Memória Associativa - Documentação Completa"

Each protocol contains the full documentation with:
- ✅ Detailed top-down investigation methodology
- ✅ Neuro-symbolic debugging cycle
- ✅ Practical examples of each defect type
- ✅ Error pattern knowledge base
- ✅ Integration with HDC (Hyperdimensional Computing)
- ✅ Complete usage checklist for AIs

### 🎯 Benefits

- ✅ Faster error diagnosis
- ✅ More effective corrections
- ✅ Prevention of recurring problems
- ✅ Continuously growing knowledge base
- ✅ Better service to developer and client requirements

**Integration**: This concept is integrated into all three protocols in the error correction and debugging steps.

---

## 📝 Credits and Versioning

- **Author:** Josué Amaral
- **License:** Internal and educational use.
- **Status:**
    - Simplicity 1: `v2.3`
    - Simplicity 2: `v2.5`
    - Simplicity 3: `v3.4`
    - Tree Imports Analogy: `v1.0`
    - Associative Memory Factor: `v1.0`

> *"I want complete and professional work!"*
