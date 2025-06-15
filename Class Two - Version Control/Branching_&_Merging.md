# Branching and Merging

### 1. What is the purpose of branching in Git?

Branching in Git lets you work on different features or fixes without affecting the main code. It’s like creating a separate copy of your project where you can make changes safely. Once you’re done, you can merge the branch back into the main code (usually the `main` or `master` branch).

This is useful for testing, working in teams, or adding features without breaking anything.

**Reference:** [https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell)



### 2. What is the difference between merging and rebasing? When would you use each?

**Merging** keeps the full history of both branches and adds a merge commit.
**Rebasing** moves your branch to the tip of the main branch, making the history look cleaner.

Use **merging** when you want to keep a full record of how branches came together.
Use **rebasing** when you want a straight, clean history (like before pushing to remote).

Both get the job done, but the choice depends on your team style.

**Reference:** [https://www.atlassian.com/git/tutorials/merging-vs-rebasing](https://www.atlassian.com/git/tutorials/merging-vs-rebasing)



### 3. How do merge conflicts occur, and what are the general steps to resolve them?

Merge conflicts happen when Git can’t decide which code to keep because two people edited the same part of a file differently.

To resolve:

1. Git marks the conflict in the file.
2. You open the file and choose what version to keep.
3. Save the changes.
4. Run `git add .`
5. Then run `git commit` to finish the merge.

**Reference:** [https://docs.github.com/en/get-started/using-git/resolving-merge-conflicts](https://docs.github.com/en/get-started/using-git/resolving-merge-conflicts)