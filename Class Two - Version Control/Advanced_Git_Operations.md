# Advanced Git Operations

### 1. When and how would you use Git stash?

You use `git stash` when you're working on something but need to switch branches or pull new updates without committing your current work. It saves your changes temporarily.

**How to use it:**

```bash
git stash         # saves uncommitted changes
git stash list    # shows all stashed items
git stash apply   # reapplies the latest stash
git stash pop     # reapplies and deletes the stash
```

It's super useful when you're in the middle of something and want a clean workspace.

**Reference:** [https://git-scm.com/docs/git-stash](https://git-scm.com/docs/git-stash)



### 2. Explain the purpose of Git tags and how to create them?

Git tags are used to **mark specific points in your commit history**, usually for releases (like `v1.0.0`). They help you track versions of your project easily.

**To create a tag:**

```bash
git tag v1.0.0
git tag -a v1.1.0 -m "Release version 1.1"
git push origin v1.1.0
```

Tags don’t move around like branches. Once created, they always point to that specific commit.

**Reference:** [https://git-scm.com/book/en/v2/Git-Basics-Tagging](https://git-scm.com/book/en/v2/Git-Basics-Tagging)



### 3. How do you manage remote repositories in Git?

Remote repositories are online versions of your project (e.g. on GitHub). You manage them using commands like:

* `git remote add origin <URL>` – connect your local repo to GitHub
* `git remote -v` – view remotes
* `git push origin main` – push to GitHub
* `git pull origin main` – pull updates from GitHub
* `git remote remove origin` – remove the remote

This lets you collaborate and back up your code online.

**Reference:** [https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)