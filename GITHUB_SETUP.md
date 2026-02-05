# Connect This Project to GitHub

Follow these steps to connect your project to your GitHub account.

---

## Step 1: Install Git (if needed)

Git wasn’t found on your system. Install it first:

1. Download Git for Windows: **https://git-scm.com/download/win**
2. Run the installer and use the default options (or adjust as you like).
3. **Restart Cursor/your terminal** after installation so `git` is recognized.

Check that it works by opening a new terminal and running:
```powershell
git --version
```

---

## Step 2: Configure Git (first time only)

Set your name and email so your commits are attributed correctly:

```powershell
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Use the same email as your GitHub account if you want commits to link to your profile.

---

## Step 3: Create a repository on GitHub

1. Go to **https://github.com** and sign in.
2. Click the **+** (top right) → **New repository**.
3. Choose a name (e.g. `vibecoding-tutorials`).
4. Choose **Public** or **Private**.
5. **Do not** check “Add a README” (your folder already has content).
6. Click **Create repository**.

---

## Step 4: Initialize Git and connect to GitHub

In a terminal, from this project folder, run:

```powershell
cd "c:\Users\chris\OneDrive\Desktop\Vibecoding Tutorials"

# Initialize a new Git repository
git init

# Add all files
git add .

# First commit
git commit -m "Initial commit"

# Add your GitHub repo as the remote (replace with YOUR username and repo name)
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username and `YOUR_REPO_NAME` with the repository name you created (e.g. `vibecoding-tutorials`).

---

## Step 5: Authentication

When you run `git push`, GitHub will ask you to sign in:

- **HTTPS**: You may be prompted for username and password. Use a **Personal Access Token** instead of your GitHub password:  
  GitHub → Settings → Developer settings → Personal access tokens → Generate new token.
- **SSH** (optional): You can set up SSH keys so you don’t need to enter credentials each time. See: https://docs.github.com/en/authentication/connecting-to-github-with-ssh

---

## Quick reference after setup

```powershell
git add .                    # Stage changes
git commit -m "Your message"  # Commit
git push                     # Push to GitHub
git pull                     # Pull latest from GitHub
```

---

Once Git is installed, you can run the commands in **Step 4** from this folder to connect the project to GitHub. If you tell me your GitHub username and desired repo name, I can give you the exact `git remote add origin` and `git push` commands.
