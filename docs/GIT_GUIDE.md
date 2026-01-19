# Git & GitHub Quick Reference

## First-Time Setup (One-Time Only)

### Configure Git Identity

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Generate SSH Key (Optional but Recommended)

```bash
ssh-keygen -t ed25519 -C "your.email@example.com"
# Press Enter to accept default location
# Add to GitHub: Settings → SSH and GPG keys → New SSH key
cat ~/.ssh/id_ed25519.pub  # Copy this output to GitHub
```

---

## Creating a New Repository

### On GitHub (Web)

1. Go to github.com → Click "+" → "New repository"
2. Name it (e.g., `my-project`)
3. Choose Public/Private
4. **Don't** initialize with README if you already have local files
5. Click "Create repository"
6. Copy the repository URL

### On Your Computer

```bash
# Navigate to your project folder
cd /path/to/your/project

# Initialize git (creates .git folder)
git init

# Add all files to staging
git add .

# Create first commit
git commit -m "Initial commit: description of what this is"

# Connect to GitHub (paste your repo URL)
git remote add origin https://github.com/username/repo-name.git

# Rename branch to main (GitHub standard)
git branch -M main

# Push to GitHub
git push -u origin main
```

---

## Daily Workflow

### Check Status

```bash
git status  # See what files changed
```

### Stage Changes

```bash
git add .                    # Stage all changes
git add filename.js          # Stage specific file
git add folder/              # Stage entire folder
```

### Commit Changes

```bash
git commit -m "Brief description of changes"
# Examples:
# "Add player dash mechanic"
# "Fix collision bug in obstacles"
# "Update README with install instructions"
```

### Push to GitHub

```bash
git push                     # Push to current branch
git push origin main         # Push to main branch specifically
```

### Pull Latest Changes (if working with others)

```bash
git pull                     # Download and merge remote changes
```

---

## Common Scenarios

### Start Fresh on New Project

```bash
cd ~/my-new-project
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/username/new-repo.git
git branch -M main
git push -u origin main
```

### Update Existing Project

```bash
cd ~/my-project
git add .
git commit -m "Describe what you changed"
git push
```

### Clone Someone Else's Repo

```bash
git clone https://github.com/username/repo-name.git
cd repo-name
# Now you can work on it
```

### Undo Last Commit (before push)

```bash
git reset --soft HEAD~1      # Keep changes, undo commit
git reset --hard HEAD~1      # Discard changes AND commit
```

### See Commit History

```bash
git log                      # Full history
git log --oneline            # Compact view
```

---

## .gitignore Basics

Create a `.gitignore` file to exclude files from git:

```
# OS files
.DS_Store
Thumbs.db

# Editor files
.vscode/
.idea/

# Dependencies
node_modules/
venv/
__pycache__/

# Secrets
.env
config.json

# Build outputs
dist/
build/
*.log
```

---

## Branch Workflow (Advanced)

### Create New Branch

```bash
git branch feature-name      # Create branch
git checkout feature-name    # Switch to it
# OR do both at once:
git checkout -b feature-name
```

### Switch Branches

```bash
git checkout main            # Go to main
git checkout feature-name    # Go to feature
```

### Merge Branch

```bash
git checkout main            # Switch to main
git merge feature-name       # Merge feature into main
git push
```

---

## GitHub Pages Setup

1. Push your code to GitHub
2. Go to repo → **Settings** → **Pages**
3. Source: **Deploy from a branch**
4. Branch: **main** / Folder: **/ (root)** or **/docs**
5. Click **Save**
6. Wait 1-2 minutes
7. Your site will be at: `https://username.github.io/repo-name/`

For `index.html` games: Use `/ (root)` folder.

---

## Troubleshooting

### "Permission denied (publickey)"

- Set up SSH key (see First-Time Setup)
- Or use HTTPS URLs instead of SSH URLs

### "fatal: not a git repository"

- You're not in a git folder. Run `git init` first.

### "Updates were rejected"

```bash
git pull --rebase           # Pull changes first
git push                    # Then push
```

### Accidentally Committed Large Files

```bash
# Remove from git but keep locally
git rm --cached large-file.mp4
echo "*.mp4" >> .gitignore
git commit -m "Remove large files"
git push
```

---

## Quick Command Reference

| Command                | What It Does            |
| ---------------------- | ----------------------- |
| `git init`             | Start tracking a folder |
| `git status`           | See what changed        |
| `git add .`            | Stage all changes       |
| `git commit -m "msg"`  | Save a snapshot         |
| `git push`             | Upload to GitHub        |
| `git pull`             | Download from GitHub    |
| `git clone URL`        | Copy a repo             |
| `git log`              | View history            |
| `git branch`           | List branches           |
| `git checkout -b name` | Create new branch       |
| `git merge name`       | Combine branches        |

---

## Best Practices

✅ **Commit often** — Small, focused commits are better than huge ones  
✅ **Write clear messages** — "Fix bug" is bad, "Fix player collision bug" is good  
✅ **Pull before push** — Avoid conflicts when working with others  
✅ **Use .gitignore** — Don't commit node_modules, .env, etc.  
✅ **Test before push** — Make sure your code runs  
✅ **Use branches** — Keep main clean, experiment in feature branches

❌ Don't commit passwords, API keys, or secrets  
❌ Don't commit 500MB files (use Git LFS or external storage)  
❌ Don't force push (`git push -f`) unless you know what you're doing

---

## Resources

- [GitHub Docs](https://docs.github.com)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [Visualize Git](https://git-school.github.io/visualizing-git/)
- [Learn Git Branching](https://learngitbranching.js.org/)

Practice with a test repository first! Create a throwaway repo and experiment.
