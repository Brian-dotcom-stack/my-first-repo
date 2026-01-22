# My First Repo

## This is my first project.

This project is about learning Git.

## What is Git?
 
 
Git = Version Control System
 
 
Tracks changes in your code
 
 
Lets you go back in time, collaborate, and store code remotely
 
 
###  Step 1: Install Git

#### Windows
 
 
Go to  [Git Windows Download](https://git-scm.com)
 
During installation:
 
Select **“Git Bash Here”**
 
 
Choose **Default editor: VS Code (recommended)**
 
 
Leave all other options default
 
 
 
Finish installation
 
 
Verify Installation
Open Git Bash and run:

```bash
git --version
```

✔️ You should see something like:

***git version 2.x.x***
 
 
#### macOS

```bash
brew install git
```

OR install Xcode Command Line Tools:

```bash
git --version
```
 
Linux (Ubuntu)

```bash
sudo apt update
sudo apt install git
```
 
### Step 2: Configure Git (ONE TIME)

Set your name & email (must match GitHub email):

```bash
git config --global user.name "Your Name"
git config --global user.email "yourmail@gmail.com"
```

Check:

```bash
git config --list
```
 
### Step 3: Create GitHub Account

Go to  [Github.com](https://github.com)
 

**Click Sign Up**
 
 
Enter:
 
*** 
Email
 
 
Username
 
 
Password
 
 
Verify email
 
 
Login to GitHub
*** 
 
✔️ Account created
 
### Step 4: Create a Local Project (Your Computer)

```bash
mkdir my-first-git-project
cd my-first-git-project
```

Create a file:
```bash
touch README.md
```

Add content:
```bash
echo "# My First Git Project" > README.md
```

### Step 5: Initialize Git Repository

```bash
git init
```

✔️ Git starts tracking this folder
You’ll see:
Initialized empty Git repository
 
 
### 🔍 Step 6: Check Git Status

```bash
git status
```

Output:
*Untracked files:
  README.md*
 
 Git sees the file but is not tracking it yet
 
### ➕ Step 7: Add Files to Staging Area

```bash
git add README.md
```


OR add all files:

```bash
git add .
```

Check again:

```bash
git status
```

### ✔️ File is now staged
 
Step 8: Commit Changes (Save Snapshot)

```bash
git commit -m "Initial commit"
```

✔️ This creates a version of your project
 
### Step 9: Create Remote Repository (GitHub)
 
Login to GitHub
 
Click + → New Repository
 
Repository name: 

```
my-first-git-project
```
 
 
Public or Private → choose
 
 
Do NOT select README (already exists)
 
 
Click Create Repository
 
 
You’ll see remote commands
 
### 🔗 Step 10: Connect Local Repo to GitHub

Copy the HTTPS URL:

[](https://github.com/username/my-first-git-project.git)

Run:

```bash
git remote add origin https://github.com/username/my-first-git-project.git
```

Verify:

```bash
git remote -v
```
 
###  Step 11: Push Code to GitHub (FIRST TIME)

```bash
git branch -M main
git push -u origin main
```
 
Enter GitHub username & password
Password won’t work anymore
 
### Step 12: Use GitHub Token (IMPORTANT)
Create Token
 
 
GitHub → Settings
 
 
Developer Settings → Personal Access Tokens
 
 
Generate New Token (Classic)
 
 
Select:
 
 
repo
 
 
 
Generate & COPY TOKEN
 
 
Use token instead of password
 
✅ Push Success!
Refresh GitHub repository
Your code is online!
 
Daily Git Workflow (MOST IMPORTANT)

```bash
git status        # check changes
git add .         # stage files
git commit -m "message"
git push          # upload to GitHub
```
 
### Common Beginner Commands


```bash
git clone (URL) #  Download repo
git pull # Get latest changes
git log # Commit history
git diff # See changes
git reset --hard # Undo everything
```
 
### Visual Git Flow
Working Directory → Staging → Commit → GitHub
 
 
###  What You’ve Learned
✅ Git installation
✅ GitHub account creation
✅ Local repository
✅ Staging & committing
✅ Pushing to remote