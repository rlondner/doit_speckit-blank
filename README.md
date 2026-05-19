# GitHub Spec Kit-Ready Next.js Blank Template

A blank, Claude-configured Next.js app template pre-wired with **Spec Kit** (v0.3.2) — a structured AI-assisted development workflow that takes a feature idea from natural language description through specification, planning, and implementation using Claude Code slash commands.

This repository is the companion template for a Medium blog post:
**[Link coming soon — will be updated with final URL]**

---

## What this is

This is the **blank starting point** used in the blog post. It is not a finished application — it is a clean slate Next.js project with the Spec Kit scaffolding already in place, so you can follow along with the post or use it as a starting template for your own projects.

The key additions over a stock `create-next-app` output are:

- `.claude/commands/` — eight Claude Code slash commands that drive the Spec Kit v0.3.2 workflow 
- `.specify/` — templates, PowerShell helper scripts, and a ratified project constitution
- Public artifacts cleaned up from the `public` folder

---

## Tech stack

| Technology   | Version   |
|--------------|-----------|
| Next.js      | ^16.2.0   |
| React        | ^19.2.4   |
| Tailwind CSS | ^4        |
| TypeScript   | ^5        |
| ESLint       | ^9        |

App Router only. No Pages Router. No test framework.

---

## Spec Kit commands

Once you open this folder in Claude Code, the following slash commands are available:

| Command | Purpose |
|---------|---------|
| `/speckit.specify` | Turn a natural-language feature description into a structured spec |
| `/speckit.clarify` | Ask Claude to fill in gaps and edge cases in an existing spec |
| `/speckit.plan` | Generate a technical implementation plan from the spec |
| `/speckit.implement` | Execute the plan — Claude writes the code |
| `/speckit.tasks` | Break the plan into a prioritised task list |
| `/speckit.taskstoissues` | Convert tasks into GitHub Issues |
| `/speckit.checklist` | Generate a quality checklist for any spec or plan |
| `/speckit.analyze` | Analyse an existing feature or codebase section |
| `/speckit.constitution` | View or amend the project's governing principles |

---

## Getting started

```bash
# Install dependencies
npm install

# Start the dev server (runs on port 3002)
npm run dev
```

Open [http://localhost:3002](http://localhost:3002) in your browser.

Then open the folder in Claude Code and run your first command:

```
/speckit.specify I want to add [describe your feature here]
```

---

## Project constitution

The `.specify/memory/constitution.md` file is the governing document for this project. It defines five non-negotiable principles:

1. **Clean Code** — readable, self-documenting, single-responsibility
2. **Simple UX** — one primary action per screen, explicit empty/error/loading states
3. **Responsive Design** — mobile-first Tailwind, verified at 320 / 768 / 1280 px
4. **Minimal Dependencies** — no new packages without justification
5. **No Testing** — no test files, no test frameworks, no test tasks (ESLint + TypeScript + manual verification only)

Claude reads this constitution before every Spec Kit command and respects it throughout code generation.

---

## Spec Kit version

This template was initialised with **Spec Kit v0.3.2** targeting the `claude` AI provider with PowerShell scripts.
