---
title: Git and GitHub Roadmap
---

# Git and GitHub

Track changes with confidence, collaborate through pull requests, and deliver from a reproducible repository.

[← Skill based roadmaps](README.md) | [All roadmaps](../README.md)

## Start here

- [ ] Create a repository and commit a small change
- [ ] Push to a remote you control
- [ ] Create a branch and open a pull request
- [ ] Resolve a merge conflict

## Learning stages

### 1. Commits and history

- The working tree, index, and repository
- Staging selective changes
- Reading diffs and commit history
- Writing clear commit messages
- Ignoring generated files
- Reverting a commit safely

**Build:** initialize a small project and produce a readable series of small commits.

### 2. Branching and integration

- Branches as movable pointers
- Fast-forward and merge commits
- Rebasing a local branch
- Merge conflicts and how to resolve them
- Pull requests as a review and discussion workflow
- Keeping a branch current without losing work

**Build:** implement a small change on a branch, open a pull request, and respond to review feedback.

### 3. Collaboration

- Forks versus shared repositories
- Remotes, tracking branches, and fetching
- Issues, labels, and project tracking
- Reviewing code rather than rewriting it
- Protected branches and required checks
- Recovering from common mistakes without destructive commands

**Build:** review someone else’s change and leave specific, actionable comments.

### 4. Automation and delivery

- Repository templates and project setup documentation
- GitHub Actions for tests and checks
- Dependabot or equivalent dependency updates
- Releases, tags, and changelogs
- GitHub Pages for static sites
- Secrets and permission scopes in workflows

**Build:** add a workflow that runs tests on every pull request and deploy a static site.

### 5. Working safely at scale

- Large files and artifact storage
- Trunk-based development and short-lived branches
- Protecting history on shared branches
- Submodules or monorepo considerations
- Incident recovery and force-with-lease

**Build:** document a recovery playbook for a bad merge and a leaked credential, then test the safe path locally.

## Definition of done

You can collaborate through small branches and pull requests, diagnose history problems, automate basic checks, and explain what each command changes.

## Related roadmaps

- [Git and GitHub beginner](../beginners/git-and-github-beginner.md)
- [Frontend developer](../role-based/frontend-developer.md)
- [Portfolio project](../projects/portfolio-project.md)

## FAQ

### Do I need every Git command?

No. A small set of commands covers most work. Learn the state model behind them so you can choose the right operation instead of guessing or copying risky commands.

[↑ Catalog](README.md) | [← Category index](README.md)
