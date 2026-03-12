# Copilot Instructions for CI_TesrRepo2

## Repository Overview

**CI_TesrRepo2** is a minimal test/placeholder repository owned by `Fabletest4` on GitHub. It was created as a bare-bones project to serve as a test case for Copilot coding agent onboarding workflows. The repository currently contains only a `README.md` with a single heading line.

Because this repository has no application source code, there are currently **no build, test, lint, or run commands**. When new code is added, this file should be updated to reflect the actual stack and commands.

---

## Repository Structure

```
CI_TesrRepo2/
├── .github/
│   └── copilot-instructions.md   ← this file
└── README.md                     ← single-line heading only
```

- There is no `src/`, `lib/`, `test/`, `docs/`, or any other application directory.
- There is no `.gitignore`, `.env`, or any configuration file.
- There are no CI/CD workflow files (no `.github/workflows/`).

---

## Languages & Frameworks

| Category      | Details                          |
|---------------|----------------------------------|
| Languages     | None (bare repository)           |
| Frameworks    | None                             |
| Package mgr   | None                             |
| Build tools   | None                             |
| Test runner   | None                             |
| Linter        | None                             |

---

## Build, Test, Lint, and Run Commands

> **None currently exist.** This repository has no source code to build, test, lint, or run.

When adding code to this repository, update this section with:
- The language/runtime and version (e.g., `node --version`, `python --version`)
- Install dependencies command (e.g., `npm install`)
- Build command (e.g., `npm run build`)
- Test command (e.g., `npm test`)
- Lint command (e.g., `npm run lint`)
- Start/run command (e.g., `npm start`)

---

## CI/CD & Validation Pipelines

There are **no GitHub Actions workflows** in this repository. No `.github/workflows/` directory exists.

When CI pipelines are added, document them here with:
- Workflow file names and their triggers
- What each job does (lint, build, test, deploy)
- Required secrets or environment variables

---

## External Dependencies & Configuration

- **No external services** (no database, no API, no cloud provider)
- **No environment variables** required
- **No secrets** configured
- **No Docker or container setup**

---

## Development Workflow

Since there is no existing infrastructure, a new contributor or coding agent should follow these general steps when adding features:

1. **Clone the repository** — already done if you are reading this.
2. **Check the open PRs and issues** on GitHub before starting work to avoid duplication.
3. **Create a branch** from `main` for your changes.
4. **Add or modify files** as needed.
5. **Update this `copilot-instructions.md`** to reflect any new build/test/lint commands, directory structure, or dependencies introduced.
6. **Open a pull request** against `main`.

---

## Notes & Known Issues

- The repository name contains a typo (`TesrRepo2` instead of `TestRepo2`) — this is intentional and should not be changed.
- This repository was onboarded to Copilot coding agent on **2026-03-12**. The first PR added this `copilot-instructions.md` file.
- No CI failures have been encountered because no CI pipelines exist yet.
