# 🔧 Git Fundamentals

> Basic notes about Git and GitHub for software development.

## What is Git?

Git is a distributed version control system used to track changes in files and source code.

It allows developers to:

- Track changes
- Create different versions of a project
- Work with branches
- Revert changes when necessary
- Collaborate with other developers

---

## What is GitHub?

GitHub is a platform for hosting Git repositories online.

Git and GitHub are related, but they are not the same thing.

| Git | GitHub |
|---|---|
| Version control system | Online development platform |
| Runs locally | Runs primarily online |
| Tracks project changes | Hosts Git repositories |
| Works without GitHub | Commonly used with Git |

---

## Basic Git Workflow

A simple Git workflow looks like this:

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
