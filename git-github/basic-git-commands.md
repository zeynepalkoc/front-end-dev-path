# Basic Git Commands

Git provides several commands to track changes and manage projects.

These commands are used in almost every development workflow.

---

# git init

The `git init` command initializes a new Git repository.

Example:

```bash
git init

This creates a hidden .git folder in your project.

After this, Git will start tracking changes.

git add

The git add command stages files before committing.

Example:

git add index.html

To add all files:

git add .

This prepares the files for commit.



git commit

The git commit command saves a snapshot of your changes.

Example:

git commit -m "Initial project setup"

The message should describe what changed.

Good commit messages help track project history.

git status

The git status command shows the current state of the repository.

Example:

git status

It shows:

modified files

staged files

untracked files

git log

The git log command shows commit history.

Example:

git log

This displays:

commit IDs

author

date

commit messages

git push

The git push command uploads local changes to GitHub.

Example:

git push origin main

This sends your commits to the remote repository.

git pull

The git pull command downloads changes from the remote repository.

Example:

git pull origin main

This updates your local project.

Example Workflow

Typical Git workflow:

git init
git add .
git commit -m "Initial commit"
git push origin main
Common Beginner Mistakes

❌ Forgetting to add files before committing
❌ Writing unclear commit messages