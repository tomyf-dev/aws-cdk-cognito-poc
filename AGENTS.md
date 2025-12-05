# AGENTS.md – Commit Rules Only

This file defines the **commit message rules** for AI coding agents.
All AI agents must strictly follow these rules when writing commits.

Architecture, infrastructure, directory structure, and dependency policies are **NOT decided yet**.
AI agents MUST NOT introduce new architecture, dependencies, or project structure without explicit instructions.

---

# 1. Branch Strategy

## 1.1 Single Branch: `main`

This project uses **only the `main` branch**.

* All work is done directly on `main`.
* No feature branches, fix branches, or other work branches are used.
* AI agents commit directly to `main`.

---

# 2. Commit Message Rules (Conventional Commits)

This project uses **Conventional Commits**.
All commit messages MUST follow the format below.

---

## 2.1 Commit Format

```
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

### Required:

* `<type>`
* `<description>` (short, clear, lowercase, English)

### Optional:

* `scope`
* body text
* footer (breaking changes, issue references, etc.)

---

## 2.2 Allowed Types

* `feat` — New feature
* `fix` — Bug fix
* `docs` — Documentation only
* `style` — Formatting (no code behavior impact)
* `refactor` — Code restructuring
* `perf` — Performance improvements
* `test` — Tests only
* `build` — Build system or dependency changes
* `ci` — CI pipeline changes
* `chore` — Miscellaneous changes

---

## 2.3 Scopes

Use scopes for clarity when appropriate:

Examples:

* `feat(auth): add passwordless login`
* `fix(api): handle missing spaceId`

Do NOT overuse scope. Only add it when meaningful.

---

## 2.4 Good Commit Examples

```
feat(auth): add passwordless login endpoint

fix(api): handle missing membership id in request

docs(readme): update branch strategy explanation

refactor(ui): simplify space selector component

chore(deps): update nextjs to 15.0.1
```

---

## 2.5 Bad Commit Examples (Prohibited)

```
update
fix bug
change something
wip
temp
test commit
```

Ambiguous commit messages are strictly prohibited.

---

# 3. AI Agent Guidelines

AI agents MUST follow these enforced rules:

1. **Commit directly to `main`.**
   This project does not use feature branches or pull requests.

2. **Do not introduce new architecture, dependencies, or directory structures** unless explicitly instructed.

3. **Keep commits meaningful:**

   * Group related changes together.
   * Avoid excessive tiny commits.

4. **Follow Conventional Commits format** for all commit messages.

---

This AGENTS.md will expand as the project evolves,
but at this stage, **commit rules are the ONLY enforced requirements** for AI agents.
