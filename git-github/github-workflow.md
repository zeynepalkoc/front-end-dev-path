# GitHub Workflow

GitHub workflow describes how developers collaborate on projects using Git and GitHub.

A typical workflow includes:

- cloning a repository
- creating branches
- making commits
- pushing changes
- creating pull requests
- merging changes

---

# Cloning a Repository

To copy a remote repository to your computer, use:

```bash
git clone https://github.com/username/project.git

This downloads the project to your local machine.

Making Changes

After cloning the repository, developers can modify files.

Example workflow:

git add .
git commit -m "Update feature"
Pushing Changes

To upload your changes to GitHub:

git push origin main

This sends your commits to the remote repository.

Pull Requests

A pull request (PR) is used to propose changes to a repository.

Developers create pull requests to:

review code

discuss improvements

merge changes safely

Typical process:

Create a feature branch

Push the branch to GitHub

Open a pull request

Review and merge

Example Workflow

Typical team workflow:

git checkout -b feature-login

git add .
git commit -m "Add login page"

git push origin feature-login

Then open a pull request on GitHub.

Merging

After the pull request is reviewed, it can be merged into the main branch.

This adds the feature to the main project.

Common Beginner Mistakes

❌ Pushing directly to the main branch
❌ Not writing clear commit messages
❌ Skipping code reviews