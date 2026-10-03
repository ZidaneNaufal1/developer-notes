# 🌿 Git Branching

> Practical notes about branches and a basic feature-development workflow.

## What is a Branch?

A branch is an independent line of development inside a Git repository.

Branches let developers work on features, fixes, or experiments without immediately changing the stable version of a project.

```text
main
 │
 ├── feature-login
 │
 └── fix-navbar
```

---

## Why Use Branches?

Branches are useful for:

- Developing features separately
- Fixing bugs safely
- Testing experiments
- Collaborating with other developers
- Reviewing work before merging it into `main`

---

## Common Branch Commands

### View branches

```bash
git branch
```

### Create and switch to a new branch

```bash
git switch -c feature-login
```

### Switch to an existing branch

```bash
git switch main
```

### Merge a branch

First switch to the branch that should receive the changes:

```bash
git switch main
```

Then merge:

```bash
git merge feature-login
```

---

## Basic Feature Workflow

```text
main
 │
 └── feature-login
        │
        ├── edit files
        ├── test changes
        ├── git add .
        ├── git commit
        │
        ↓
     switch to main
        │
        ↓
     merge feature-login
```

> **Create → Develop → Test → Commit → Merge**

---

## Branch Naming Examples

```text
feature-login
feature-inventory
fix-player-movement
fix-ui-layout
docs-update-readme
```

Good branch names describe the purpose of the work.

---

## Basic Best Practices

- Keep `main` stable.
- Use one branch for one focused change.
- Test before merging.
- Write small, descriptive commits.
- Avoid mixing unrelated changes in the same branch.

---

## What I Learned

Branches provide a safer workflow for developing changes without directly modifying the stable branch.

They become especially useful when projects grow or when multiple developers collaborate.

---

## 📌 Learning Status

- [x] Understand what a branch is
- [x] Understand why branches are useful
- [x] Create and switch branches
- [x] Understand basic merging
- [ ] Practice merge conflicts
- [ ] Practice pull requests
- [ ] Learn GitHub branch protection
