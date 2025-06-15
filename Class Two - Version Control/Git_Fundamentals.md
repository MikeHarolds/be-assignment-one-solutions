# Git Fundamentals


### 1. Explain the difference between Git and other version control systems.

Git is a **distributed version control system (DVCS)**, which means every developer has the full copy of the project’s history on their own machine. Unlike older systems like SVN or CVS (which are centralized), Git doesn’t depend on one server. You can work offline and still access the full history.

Git is also super fast, supports branching and merging really well, and makes collaboration easier through platforms like GitHub.

**Reference:** [https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)



### 2. What is the purpose of a repository in version control?

A **repository** (or repo) is like a folder where Git stores your project and all its version history. It keeps track of every change you make, whether it's a new file, edit, or deletion. There are two types:

* **Local repo** (on your PC)
* **Remote repo** (like GitHub)

The main purpose is to help manage and organize code, allow collaboration with others, and roll back to earlier versions when needed.

**Reference:** [https://www.atlassian.com/git/tutorials/what-is-version-control](https://www.atlassian.com/git/tutorials/what-is-version-control)


### 3. How does Git track changes in your codebase?

Git tracks changes by taking **snapshots** of your files. Every time you commit, Git saves what changed from the last commit, not the whole files again. It uses something called a **SHA hash** to identify each version uniquely.

This makes Git efficient and reliable. You can go back to old versions, compare changes, and see who did what using commands like `git log` or `git diff`.

**Reference:** [https://git-scm.com/docs/gittutorial](https://git-scm.com/docs/gittutorial)

