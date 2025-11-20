Here is a **clean, professional, repo-ready README.md** for your tools folder that includes **BMAD framework**, **OpenSpec**, and space for future tools.

You can drop this directly into `/_tools/README.md` or at the root of your tools repo.

---

# 🧰 Tools Workspace

*A centralized toolkit for development workflows, architecture, documentation, and automation.*

This repository contains all generic, reusable tools that support multiple projects.
Nothing here is project-specific — it is intended to be a **shared toolbox** for any app you build.

---

## 📂 Folder Structure

```
/_tools/
 ├── bmad/          # BMAD-framework replica / helpers / workflows / templates
 ├── openspec/      # OpenSpec tooling and spec definitions
 ├── scripts/       # CLI utilities, helper scripts, generators
 ├── templates/     # Project templates, file blueprints, boilerplates
 ├── cli/           # (Optional) Custom CLI for developer workflows
 └── README.md
```

You will keep your main product in:

```
/projectA/
```

All generic tooling stays in:

```
/_tools/
```

---

## 🚀 Purpose of This Repo

This repo exists to:

### ✔ Centralize all shared tools

Avoid duplicating logic across your different apps.

### ✔ Provide structured methodology

Via BMAD framework, reusable workflows, prompt files, and agents.

### ✔ Standardize architecture

OpenSpec is used to produce unified specifications that drive backend, frontend, and API decisions.

### ✔ Speed up development

Scripts and templates allow you to spin up features, modules, or entire services quickly.

---

## 📦 Included Tooling

### ### 1️⃣ BMAD Framework (Replica / Adapted)

Located in:
`/_tools/bmad/`

Includes:

* BMAD agents rewritten for local/CLI/Cursor use
* Workflows adapted from the official BMAD METHOD
* Templates for:

  * Architecture plans
  * Feature decomposition
  * Planning flows
  * Scope docs
  * PRD (Product Requirements Doc)
  * Task breakdowns

This version contains **no project-specific details** — it is pure framework logic.

### ### 2️⃣ OpenSpec

Located in:
`/_tools/openspec/`

Includes:

* OpenSpec schema definitions
* Spec templates for APIs, database models, entities, and flows
* Generators to output:

  * FastAPI models
  * React TypeScript types
  * JSON Schema
  * High-level docs

This acts as your **single source of truth** for all future apps.

### ### 3️⃣ Scripts & CLI Utilities

Located in:
`/_tools/scripts/` and `/_tools/cli/`

Examples:

* `generate-module.sh` — create a new business module skeleton
* `create-agent.py` — quickly spin up a BMAD-style agent
* `sync-specs.sh` — propagate OpenSpec into project repos
* `update-env.sh` — helper for environment variable management

---

## 🧭 How to Use This Repository

### Step 1 — Clone independently

This tools repo can be cloned once and reused:

```
git clone https://github.com/<you>/tools
```

### Step 2 — Link it into projects

Inside any project (e.g., `/resumai-app/`):

```
_tools/        -> symbolic link to your tools repo
```

Or keep `/tools` as a sibling folder.

### Step 3 — Use BMAD for planning

From Cursor or terminal:

* Follow BMAD workflows
* Use agents to analyze, plan, design, and generate
* Use templates to structure your architecture or specs

### Step 4 — Use OpenSpec as the source of truth

Define your specifications here, then:

```
spec generate backend
spec generate frontend
```

### Step 5 — Use scripts to standardize operations

Example:

```
./_tools/scripts/generate-module.sh tickets
./_tools/scripts/sync-specs.sh
```

---

## 🧩 Why this separation?

Your rule:

> **Everything generic must live in /_tools/bmad/**
> **Every project lives in /projectA/**

This allows:

* ✨ Clean separation of reusable vs. project-specific
* 🧼 No cross-contamination of business logic
* ♻️ One shared toolbox for future apps
* 🚀 Faster bootstrapping and consistent methodology

---

## 📌 Future Additions

You can expand this repository with:

* AI assistants (customized agents)
* Test data generators
* Reusable GitHub Action workflows
* CI/CD templates
* Architecture guidelines
* Persona templates
* UI design system documents
* Database design heuristics

✅ A quickstart “How to use OpenSpec on day 1”
Just tell me.
