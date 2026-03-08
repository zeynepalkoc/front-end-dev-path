# Git Branching

Branching allows developers to work on different features without affecting the main codebase.

Each branch represents an independent line of development.

The default branch is usually called **main** or **master**.

---

# Why Branching is Important

Branching helps developers:

- develop new features safely
- fix bugs without affecting production code
- collaborate with teams

Example workflow:

main branch → stable project  
feature branch → new feature development  

---

# Creating a Branch

To create a new branch:

```bash
git branch feature-login

this creates a branch called feature-login

Switching Branches

To switch to another branch:

git checkout feature-login

Now you are working in the feature-login branch.

Creating and Switching in One Command

You can create and switch to a branch in one step:

git checkout -b feature-login
Viewing Branches

To see all branches:

git branch

The current branch will be marked with *.

Example output:

* main
feature-login
feature-ui
Merging Branches

After finishing work in a branch, it can be merged into the main branch.

Example:

Switch to main:

git checkout main

Merge the branch:

git merge feature-login

Now the feature is included in the main branch.

Example Workflow
git checkout -b feature-navbar
# work on feature

git add .
git commit -m "Add navbar"

git checkout main
git merge feature-navbar
Common Beginner Mistakes

❌ Working directly on the main branch
❌ Forgetting to switch branches before committing