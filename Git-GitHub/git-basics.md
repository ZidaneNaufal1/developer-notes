# 🔧 Git Fundamentals

> Practical notes on Git and GitHub for everyday software development.

## What is Git?

Git is a **distributed version control system** used to track changes in files and source code.

It helps developers:

- Track project history
- Create safe checkpoints with commits
- Work on features in separate branches
- Revert unwanted changes
- Collaborate without overwriting each other's work

---

## What is GitHub?

GitHub is a platform for hosting Git repositories online.

Git and GitHub are related, but they are not the same thing.

| Git | GitHub |
|---|---|
| Version control system | Online development platform |
| Runs locally | Hosts repositories online |
| Tracks file history | Supports collaboration and code review |
| Works without GitHub | Commonly used together with Git |

---

## Basic Git Workflow

```text
Working Directory
       ↓
     git add
       ↓
   Staging Area
       ↓
   git commit
       ↓
  Local Repository
       ↓
    git push
       ↓
     GitHub
```

The basic idea is:

> **Edit → Stage → Commit → Push**

---

## Common Commands

### Check repository status

```bash
git status
```

Shows changed, staged, and untracked files.

### Stage changes

```bash
git add .
```

Stages all current changes.

### Create a commit

```bash
git commit -m "describe the change"
```

Creates a local checkpoint with a descriptive message.

### Push commits

```bash
git push
```

Sends local commits to the configured remote repository.

### Pull remote changes

```bash
git pull
```

Downloads and integrates changes from the remote branch.

### View commit history

```bash
git log --oneline
```

Displays a compact commit history.

---

## Example Workflow

```bash
git status
git add .
git commit -m "add calculator feature"
git push
```

This is a simple workflow I can use after making and testing a project change.

---

## What I Learned

- Git tracks versions of a project.
- GitHub hosts Git repositories and adds collaboration tools.
- A commit should represent a meaningful change.
- Clear commit messages make project history easier to understand.
- I should test changes before pushing them.

---

## 📌 Learning Status

- [x] Understand Git vs GitHub
- [x] Understand staging and commits
- [x] Understand push and pull
- [x] Practice a basic Git workflow
- [ ] Practice resolving merge conflicts
- [ ] Learn pull requests in more depth
- [ ] Learn branch protection and collaboration workflows
