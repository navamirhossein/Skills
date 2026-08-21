# 🧠 AI Skills

A curated collection of reusable, high-quality **AI skills for Claude and other LLMs**, designed to turn AI assistants into structured researchers, teachers, engineers, architects, planners, and productivity partners.

Each skill is a focused instruction set that gives an LLM a specialized role, workflow, and output standard.

---

## ✨ Skills

| Skill                     | Description                                                                                                                                |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| 🎓 **Learning Path**      | Builds structured, dependency-aware learning paths from beginner to mastery.                                                               |
| 🔬 **Research Assistant** | Conducts rigorous research, synthesizes sources, evaluates evidence, and develops research outputs.                                        |
| 🧑‍💻 **Senior Engineer** | Reviews code like a production-grade senior/staff engineer across architecture, bugs, security, performance, testing, and maintainability. |
| 🏗️ **App Spec**          | Converts an app idea into a detailed, implementation-ready software specification.                                                         |
| 🔄 **Handoff**            | Creates a complete `HANDOFF.md` so another LLM can continue a project without losing context.                                              |
| 🧑‍🏫 **Teacher**         | Teaches programming and technical concepts by explaining intuition before implementation so the user understands why an answer is correct. |

More skills will be added over time.

---

## 🚀 Why Skills?

A generic AI assistant can answer questions.

A well-designed skill gives it a **repeatable operating system for a specific job**.

Instead of:

```text
"Help me build this app."
```

you can give an App Spec skill and get:

```text
Requirements
    ↓
Domain Model
    ↓
Architecture
    ↓
Database
    ↓
API
    ↓
Frontend
    ↓
Security
    ↓
Testing
    ↓
Deployment
    ↓
Implementation Roadmap
```

The goal is to make AI interactions more **structured, consistent, and actionable**.

---

## 📁 Repository Structure

```text
skills/
├── app-spec/
│   └── SKILL.md
│
├── handoff/
│   └── SKILL.md
│
├── learning-path/
│   └── SKILL.md
│
├── research-assistant/
│   └── SKILL.md
│
├── senior-engineer/
│   └── SKILL.md
│
└── teacher/
    └── SKILL.md
```

Each skill is self-contained and can be used independently.

---

## 🛠️ Using a Skill

Open the skill's `SKILL.md` and provide its contents to your LLM as the skill/instruction.

For example:

```text
skills/
└── senior-engineer/
    └── SKILL.md
```

Give `SKILL.md` to Claude or another compatible LLM, then provide your task.

### Example

```text
Use the Senior Engineer skill.

Review this backend architecture and identify
production risks, performance problems,
security vulnerabilities, and maintainability issues.
```

The skill defines **how the model should think about and execute the task**, while your prompt defines **what you want it to work on**.

---

# 🎓 Learning Path

The **Learning Path** skill turns a goal into a structured roadmap.

It can determine:

* Current knowledge level
* Prerequisites
* Learning dependencies
* Topics and subtopics
* Learning resources
* Exercises
* Projects
* Review cycles
* Mastery checkpoints
* Next steps

It is designed to optimize for **understanding and practical competence**, not simply finishing courses.

---

# 🔬 Research Assistant

The **Research Assistant** skill is designed for serious academic and professional research.

It helps with:

* Research questions
* Literature reviews
* Paper analysis
* Methodology
* Hypothesis development
* Research design
* Statistical/econometric reasoning
* Evidence evaluation
* Research gaps
* Robustness analysis
* Academic writing
* Reproducibility

The goal is to make the LLM behave more like a **research collaborator** than a search box.

---

# 🧑‍💻 Senior Engineer

The **Senior Engineer** skill reviews software as if it were entering production.

It examines:

* Architecture
* Correctness
* Bugs
* Security
* Performance
* Concurrency
* Reliability
* Maintainability
* Testing
* Observability
* Dependencies
* Edge cases

Most importantly, it explains:

> **What is wrong, why it matters, and what engineering trade-offs exist.**

It does not simply replace the user's code with another implementation.

---

# 🏗️ App Spec

The **App Spec** skill converts an idea into an implementation blueprint.

It covers:

```text
Product Requirements
        ↓
User Stories
        ↓
Domains
        ↓
Architecture
        ↓
Data Model
        ↓
Database
        ↓
API
        ↓
Frontend
        ↓
Backend
        ↓
Security
        ↓
Testing
        ↓
CI/CD
        ↓
Deployment
        ↓
Implementation Roadmap
```

The output is an `APP_SPEC.md` designed to serve as a **single source of truth for implementation**.

---

# 🔄 Handoff

The **Handoff** skill solves one of the biggest problems with long AI conversations: losing context.

It creates a complete:

```text
HANDOFF.md
```

containing:

* Current objective
* Project state
* Decisions
* Rejected approaches
* Important reasoning
* Constraints
* Technical context
* Research context
* Files and artifacts
* Open questions
* Known problems
* Immediate next action
* Continuation instructions

This allows another LLM to pick up the project without making the user explain everything again.

---

# 🧑‍🏫 Teacher

The **Teacher** skill teaches programming and technical concepts by explaining **intuition before implementation**, helping the user understand not only *what* works, but *why* it works.

It is useful when the user:

* Invokes `/teacher`
* Asks why something works
* Wants a concept explained
* Is debugging to understand a mistake
* Requests mentorship-style teaching
* Wants to learn rather than simply receive an answer

The goal is to build **mental models, intuition, and independent problem-solving ability**, rather than simply providing solutions.

---

## 🧩 Design Philosophy

These skills follow a few principles:

### 1. Context Before Action

Understand the problem before producing an answer.

### 2. Explain the Reasoning

Don't just provide an output. Explain the important decisions behind it.

### 3. Separate Facts From Assumptions

Unknown information should not quietly become "facts."

### 4. Prefer Structured Workflows

Complex tasks should have explicit stages and dependencies.

### 5. Optimize for Continuity

Important decisions and project state should survive across conversations and models.

### 6. Avoid Unnecessary Complexity

Good skills should make AI more capable without turning every task into an enterprise architecture diagram.

---

## 🌱 Adding a New Skill

A good skill should contain:

```text
Role
Purpose
Responsibilities
Workflow
Rules
Decision criteria
Output format
Quality checks
Failure modes
Examples
```

A skill should be:

* Reusable
* Self-contained
* Explicit
* Practical
* Model-agnostic where possible
* Easy to understand
* Difficult to misinterpret

---

## 🤝 Contributing

Contributions are welcome.

When adding a skill:

1. Create a dedicated directory.
2. Add a `SKILL.md`.
3. Clearly define the skill's role.
4. Provide a structured workflow.
5. Define expected outputs.
6. Include quality-control rules.
7. Update this README.

Example:

```text
new-skill/
└── SKILL.md
```

---

## 🗺️ Roadmap

Potential future skills include:

* 🧑‍🏫 **Teacher**
* 🧠 **Concept Explainer**
* 📊 **Data Scientist**
* 📈 **Quant Researcher**
* 🏛️ **System Architect**
* 🧪 **Testing Engineer**
* 🔐 **Security Engineer**
* 📝 **Technical Writer**
* 📋 **Project Manager**
* 🎯 **Decision Analyst**
* 🐛 **Debugging Specialist**
* 📚 **Literature Reviewer**
* 💡 **Product Strategist**
* ⚡ **Performance Engineer**

---

## ⭐ Philosophy

The idea is simple:

> **Don't just give an LLM a prompt. Give it a profession.**

These skills are designed to turn broad AI capabilities into **repeatable expert workflows** that can be carried from project to project.

---

## 📄 License

Add your preferred license here, for example:

```text
MIT License
```

---

## 🚧 Status

Actively evolving. New skills, improvements, examples, and specialized workflows will be added over time.
