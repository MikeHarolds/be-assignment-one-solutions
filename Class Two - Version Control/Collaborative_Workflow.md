# Collaborative Workflow


### 1. Explain the purpose and process of creating a pull request.

A **pull request** (PR) is used to tell others that you’ve made changes to code and you want them to review and possibly add it to the main project. It’s common when working with teams on platforms like GitHub.

**Process:**

1. Create a new branch and make changes.
2. Push the branch to GitHub.
3. Click “New pull request.”
4. Compare your branch with the main one.
5. Add a title and description.
6. Submit it for review.

**Reference:** [https://docs.github.com/en/pull-requests](https://docs.github.com/en/pull-requests)



### 2. What is the difference between forking and cloning a repository?

**Forking** creates your own copy of someone else’s repo on GitHub. It’s useful when you don’t have permission to push directly.

**Cloning** copies a repo from GitHub to your local computer using `git clone`. You do this when you want to work on the code locally.

In short:

* **Fork** = copy repo to your GitHub
* **Clone** = copy repo to your PC

**Reference:** [https://docs.github.com/en/get-started/quickstart/fork-a-repo](https://docs.github.com/en/get-started/quickstart/fork-a-repo)



### 3. How would you use Git to collaborate with other developers on the same project?

To work with others:

1. Everyone clones the repo.
2. Each person creates their own branch.
3. Make changes, commit, and push.
4. Create a pull request for review.
5. After approval, merge into the main branch.
6. Regularly pull the latest changes using `git pull`.

This keeps teamwork organized and avoids messing up the main code.

**Reference:** [https://www.atlassian.com/git/tutorials/comparing-workflows](https://www.atlassian.com/git/tutorials/comparing-workflows)


