===========================================================================================
# Git Workflow Command Reference

Quick reference for the Git commands commonly used in this project's development workflow.

===========================================================================================
## Start New Work

Update `main`:

```bash
git switch main
git pull
```

Create and switch to a new branch:

```bash
git switch -c <branch-name>
```

Example:

```bash
git switch -c feature/42-skill-confidence
```

===========================================================================================
## Check Your Work

View changed and staged files:

```bash
git status
```

View unstaged changes:

```bash
git diff
```

View staged changes:

```bash
git diff --staged
```

===========================================================================================
## Commit Changes

Stage specific files:

```bash
git add <file>
```

Commit staged changes:

```bash
git commit -m "<commit message>"
```

Example:

```bash
git commit -m "Add skill confidence selection"
```

===========================================================================================
## Push a New Branch

First push:

```bash
git push -u origin <branch-name>
```

After the upstream branch is configured:

```bash
git push
```

Then open a Pull Request into `main` on GitHub.

===========================================================================================
## Update an Existing Branch

If additional changes are requested during Pull Request review:

```bash
git add <file>
git commit -m "<commit message>"
git push
```

The existing Pull Request updates automatically.

===========================================================================================
## After a Pull Request Is Merged

Update local `main`:

```bash
git switch main
git pull
```

Delete the completed local branch:

```bash
git branch -d <branch-name>
```

The remote branch can be deleted using GitHub's **Delete branch** button after the Pull Request is merged.

===========================================================================================
## Useful Commands

View local branches:

```bash
git branch
```

View local and remote branches:

```bash
git branch -a
```

View recent commit history:

```bash
git log --oneline --graph --decorate
```

View configured remotes:

```bash
git remote -v
```

View the current branch:

```bash
git branch --show-current
```

===========================================================================================