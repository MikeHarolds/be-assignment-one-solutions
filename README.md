# BE Week One Assignment Solutions

This README explains the core concepts of Git and version control, especially how it’s used in real-world software development, including Node.js projects. 



# Git and Version Control – A Student's Guide


##  What is Version Control and Why Is It Important?

Version control helps developers track and manage changes in their codebase over time. It allows us to:

- Go back to previous versions of the project.
- Fix mistakes without losing progress.
- Track who made changes and when.
- Work safely without overwriting each other’s code.

---

##  How Version Control Helps Team Collaboration

- Developers can work on their own branches without interfering with others.
- Changes can be reviewed before merging.
- It keeps the main project stable while features are developed separately.
- Everyone stays in sync, and conflicts can be resolved properly.

---

##  Best Practices for Organizing a Git Repository

- Use meaningful folder names like `src/`, `assets/`, `docs/`.
- Add a `.gitignore` file to ignore `node_modules/` and other unnecessary files.
- Keep the `main` branch clean and stable.
- Create feature branches for new work.
- Use meaningful commit messages like `fix: login button error`.
- Keep a good `README.md` explaining the project.

---

##  Setting Up a New Node.js Project with Git

1. Run `git init` to start version control.
2. Run `npm init` to create `package.json` for managing dependencies.
3. Add `node_modules/` to `.gitignore`.
4. Commit with a message like `Initial commit`.
5. Create branches for features and bug fixes.

---

##  Relationship Between Node.js and Version Control

- Node.js helps build the app, Git manages the history of the app’s code.
- Together, they allow safe, organized development.
- Git tracks all files except `node_modules`, which are too large to store.

---

##  How Git Manages Node.js Dependencies

- Only `package.json` and `package-lock.json` are tracked.
- They store a list of all dependencies and their versions.
- When someone clones the repo, they just run `npm install` to set up the project.

---

##  Purpose of Branching in Git

- Branches let you work on features without touching the main code.
- You can experiment, test, and merge later.
- Helps avoid breaking the main project while still making progress.

---

##  Merging vs. Rebasing

- **Merging** keeps all history and shows how two branches joined.
- **Rebasing** makes the history cleaner by placing your changes on top of the latest branch.

Use **merge** when you want to preserve history.  
Use **rebase** when you want a straight, clean timeline before pushing.

---

##  Merge Conflicts and How to Fix Them

Conflicts happen when two branches change the same part of a file.

**Steps to resolve:**
1. Git marks the conflict in the file.
2. Manually fix the code.
3. Run `git add .`
4. Commit with `git commit`

---

##  Pull Requests

Pull Requests (PRs) are used when you want others to review your changes before merging them into the main branch.

**Steps:**
1. Push your branch to GitHub.
2. Click "New pull request."
3. Compare branches and submit.
4. After review, it can be merged.

---

##  Forking vs. Cloning

- **Forking**: Copies a repo to your GitHub account.
- **Cloning**: Copies a repo from GitHub to your PC.

Fork when you don’t have permission to push. Clone when you want to work locally.

---

##  Collaborating with Others Using Git

1. Clone the repo.
2. Create your own branch.
3. Make changes and commit.
4. Push and create a PR.
5. After review, changes are merged into the main project.

---

##  Using Git Stash

Use `git stash` when you’re not ready to commit, but need to switch branches or pull updates.

**Commands:**
- `git stash` – saves your current changes.
- `git stash pop` – restores the latest stash.
- `git stash list` – shows saved stashes.

---

##  Git Tags and How to Create Them

Tags are used to mark specific points in history (e.g. a release version).

**Examples:**
```bash
git tag v1.0.0
git tag -a v2.0 -m "New release"
git push origin v2.0
