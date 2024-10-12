# Git and GitHub Guide for Windows/Linux

## Table of Contents
1. [Introduction to Git and GitHub](#introduction-to-git-and-github)
2. [Installing Git](#installing-git)
3. [Setting Up Git](#setting-up-git)
4. [Basic Git Commands](#basic-git-commands)
5. [Branching and Merging](#branching-and-merging)
6. [Collaborating with GitHub](#collaborating-with-github)
7. [Git Best Practices](#git-best-practices)
8. [Advanced Git Commands](#advanced-git-commands)
9. [Git Cheat Sheet](#git-cheat-sheet)

### Introduction to Git and GitHub
Git is a distributed version control system that allows you to track changes in your code. GitHub is a web-based platform for hosting and collaborating on Git repositories. Together, Git and GitHub make it easy to work with other developers, keep track of changes, and manage software projects.

### Installing Git

#### Windows
1. Download Git from [git-scm.com](https://git-scm.com/download/win).
2. Run the installer.
3. During installation, ensure you select "Use Git from the Windows Command Prompt" to make Git easily accessible.
4. Once installed, open "Git Bash" to use Git commands.

#### Linux
1. Open a terminal.
2. Install Git using your package manager:
   - **Debian/Ubuntu**: `sudo apt install git`
   - **Fedora**: `sudo dnf install git`
   - **Arch Linux**: `sudo pacman -S git`

### Setting Up Git
After installing Git, configure your user details so that your commits are properly identified.

```bash
# Set your username
git config --global user.name "Your Name"

# Set your email
git config --global user.email "youremail@example.com"

# Confirm your settings
git config --list
```

### Basic Git Commands

#### 1. Initialize a Repository
To start a new Git repository in a directory:
```bash
git init
```

#### 2. Clone a Repository
To copy an existing repository from GitHub:
```bash
git clone <repository-url>
```

#### 3. Check the Status
To see the current state of the repository and track changes:
```bash
git status
```

#### 4. Add Files to Staging
Add a file or all changes to staging:
```bash
# Add a specific file
git add filename.txt

# Add all files
git add .
```

#### 5. Commit Changes
To save changes to the repository:
```bash
git commit -m "Describe your changes here"
```

#### 6. Push to GitHub
Send your commits to a remote GitHub repository:
```bash
git push origin main
```

### Branching and Merging
Branches in Git are a great way to work on different features independently.

#### 1. Create a Branch
To create and switch to a new branch:
```bash
git checkout -b new-feature
```

#### 2. List Branches
To see all branches:
```bash
git branch
```

#### 3. Merge a Branch
Switch to the main branch and merge changes from another branch:
```bash
git checkout main
git merge new-feature
```

#### 4. Delete a Branch
Delete a branch after merging:
```bash
git branch -d new-feature
```

### Collaborating with GitHub

#### 1. Forking a Repository
To contribute to an open-source project, first "fork" it using the "Fork" button on GitHub. This creates a copy in your GitHub account.

#### 2. Cloning Your Fork
Clone your forked repository to your local machine:
```bash
git clone <your-fork-url>
```

#### 3. Adding a Remote
Add the original repository as a remote to keep up with changes:
```bash
git remote add upstream <original-repo-url>
```

#### 4. Fetch and Merge Updates
Get updates from the original repository:
```bash
git fetch upstream
git merge upstream/main
```

#### 5. Creating a Pull Request
Once you've made changes and pushed them to GitHub, you can create a pull request:
1. Go to your fork on GitHub.
2. Click the "Pull Request" button.
3. Fill out the pull request form and submit it.

### Git Best Practices
1. **Commit Often**: Make small, frequent commits with meaningful messages.
2. **Use Branches**: Always create a branch for new features or bug fixes.
3. **Pull Before Pushing**: Before pushing, pull the latest changes from the remote to avoid conflicts.
4. **Write Good Commit Messages**: Include clear descriptions about what changes you made and why.

### Advanced Git Commands

#### 1. Stashing Changes
If you want to save changes without committing them:
```bash
git stash
```
To apply stashed changes:
```bash
git stash apply
```

#### 2. Undoing Changes
To undo changes in your working directory:
```bash
git checkout -- filename.txt
```

#### 3. Revert a Commit
To create a new commit that undoes the changes from a previous commit:
```bash
git revert <commit-id>
```

#### 4. Resetting a Branch
To undo commits and changes permanently:
```bash
git reset --hard <commit-id>
```

### Git Cheat Sheet

#### Repository Management
- **Initialize Repository**: `git init`
- **Clone Repository**: `git clone <repository-url>`

#### Configuration
- **Set Username**: `git config --global user.name "Your Name"`
- **Set Email**: `git config --global user.email "youremail@example.com"`
- **View Configuration**: `git config --list`

#### Basic Workflow
- **Check Status**: `git status`
- **Add File to Staging**: `git add <filename>` or `git add .`
- **Commit Changes**: `git commit -m "Commit message"`
- **Push to Remote**: `git push origin <branch-name>`
- **Pull from Remote**: `git pull origin <branch-name>`

#### Branching
- **Create Branch**: `git branch <branch-name>`
- **Switch Branch**: `git checkout <branch-name>`
- **Create and Switch Branch**: `git checkout -b <branch-name>`
- **List Branches**: `git branch`
- **Delete Branch**: `git branch -d <branch-name>`

#### Merging
- **Merge Branch**: `git merge <branch-name>`

#### Remote Management
- **Add Remote**: `git remote add <name> <url>`
- **View Remotes**: `git remote -v`
- **Fetch from Remote**: `git fetch <remote>`

#### Stashing
- **Stash Changes**: `git stash`
- **Apply Stashed Changes**: `git stash apply`

#### Undoing Changes
- **Discard Changes in File**: `git checkout -- <filename>`
- **Revert Commit**: `git revert <commit-id>`
- **Reset Branch**: `git reset --hard <commit-id>`

#### Logs and History
- **View Commit History**: `git log`
- **View Specific File History**: `git log <filename>`

#### Tagging
- **Create Tag**: `git tag <tagname>`
- **Push Tag to Remote**: `git push origin <tagname>`

### Conclusion
Now you should have a solid understanding of how to use Git on Windows/Linux and collaborate using GitHub. The more you practice, the more comfortable you'll get with Git commands. Happy coding!