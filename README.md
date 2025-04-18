# Git & GitHub Tutorial

---
### Day-01 : https://youtu.be/ERTz8EkHBBA
### Day-02 : https://youtu.be/MVq5TORaIC0
### Day-03 : https://youtu.be/nNkV1Q3NDt0
---

## Git vs GitHub

- **Git** is a version control software.
- **GitHub** is a platform used to store all developers' project source code in one place.
- On GitHub, we can create repositories to store project code.
- All developers can connect to the GitHub repository for code integration (making code integration very easy).
- GitHub allows tracking of all code changes:
  - Who modified
  - When modified
  - What was modified
  - Why modified

---

## Environment Setup

1. Create an account at [github.com](https://www.github.com) (free of cost).
2. Download & install Git client software: [https://git-scm.com/downloads](https://git-scm.com/downloads)
3. Open Git Bash and configure your name and email:
   ```bash
   git config --global user.name "your-name"
   git config --global user.email "your-email"
   ```

> Configuring name and email is a one-time process.

---

## What is a GitHub Repository?

- A repository is a place to store project source code/files.
- For each project, one GitHub repository is created.
- Two types of repositories:
  1. **Public Repo**: Anybody can see & you choose who can commit.
  2. **Private Repo**: You choose who can see & who can commit.

### Example:
Project Git Repo URL: `https://github.com/ashokitschool/sbi_loans_app.git`

Project team members use the repo URL to connect.

---

## Git Architecture

1. Working Tree
2. Staging Area
3. Local Repository
4. Central Repository (Remote)

---
![Project Screenshot](git-architecture.gif)
---

## Git Bash Commands

```bash
git init              # Initialize working tree
git status            # Show working tree status
git add <file-name>   # Add file to staging area
git add .             # Add all files to staging area
git commit -m "msg"   # Commit staged files to local repo
git push              # Push local commits to remote repo
git restore <file>    # Unstage or discard changes
git log               # Show commit history
git rm <file-name>    # Remove a file
git clone <repo-url>  # Download remote repo to local
git pull              # Get latest changes from remote repo
```

> Note: After `git rm`, commit and push to delete file from remote repo.

---

## Git GUI

- A desktop tool to perform Git operations.
- Run in working tree:

```bash
git gui
```

---

## .gitignore File

- Specifies files/folders to skip in Git operations.

### Example:
```
.settings
.classpath
.project
target/
```

---

## Git Branches

When multiple teams work on the same repo, use branches to avoid delivery issues.

### Recommended Branches:

- `main` (default)
- `develop` (development team)
- `sit` (bug fixing team)
- `research` (R&D team)
- `release` (production team)

> Multiple teams can work in parallel using branches.

---

## Lab Task

1. Go to GitHub and create `develop` branch from `main`.
2. Clone the repo (main branch will be cloned by default):
   ```bash
   git clone <url>
   ```
3. Switch to develop branch:
   ```bash
   git checkout develop
   ```
4. Create a file and push it to `develop` branch.
5. Create a Pull Request and merge `develop` into `main`.
