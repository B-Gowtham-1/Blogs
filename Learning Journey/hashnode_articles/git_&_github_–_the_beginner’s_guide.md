# Git & GitHub – The Beginner’s Guide

---

## **What is Git? (And Why Do We Need It?)**

Git is like a **time machine for your code**. It **saves different versions** of your project, so if you mess up, you can **go back** to a working version instead of starting from scratch.

Imagine writing an essay. If you accidentally delete half of it, you’d want an *undo* button, right? **That’s what Git does for code.**

## **What is GitHub? (Not the Same as Git!)**

GitHub is like a **cloud storage** for your Git projects. It lets you **store your code online, share it, and collaborate with others**.

Think of Git as your **notes app**, and GitHub as **Google Drive** where you save and share those notes.

---

# **Getting Started With Git**

### **Step 1: Install Git**

If you haven’t installed Git yet, download it here: [git-scm.com](https://git-scm.com/)

### **Step 2: Set Up Git (Just Once)**

Tell Git who you are:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

---

# **Creating a New Git Project**

### **Step 1: Create a Folder and Open Terminal**

Pick a folder where you want to save your project. Open your terminal (Command Prompt or Git Bash) and go to that folder using:

```bash
cd path/to/your/folder
```

### **Step 2: Turn the Folder Into a Git Project**

```bash
git init
```

Boom! Your project is now **tracked by Git**.

### **Step 3: Check Git Status (To See What’s Happening)**

```bash
git status
```

If you see *“No commits yet”*, that’s fine. We haven’t added anything yet.

### **Step 4: Add Files to Git**

Git doesn’t track your files automatically, so we need to **add them**:

```bash
git add .
```

The dot (`.`) means “add everything.” You can also add specific files:

```bash
git add myfile.txt
```

### **Step 5: Save Your Changes (Commit)**

Now that we’ve added files, we need to **commit** (save) them:

```bash
git commit -m "First commit - added files"
```

Think of this like taking a **snapshot** of your project at this moment.

---

# **Connecting to GitHub**

### **Step 1: Create a Repository on GitHub**

1. Go to [GitHub](https://github.com/) and sign in.
    
2. Click **New Repository**.
    
3. Give it a name (e.g., `my-first-repo`).
    
4. Keep it **public** (so everyone can see) or **private** (just for you).
    
5. Click **Create Repository**.
    

### **Step 2: Connect Your Local Project to GitHub**

Back in your terminal, link your local project to GitHub:

```bash
git remote add origin https://github.com/your-username/my-first-repo.git
```

Then push your code to GitHub:

```bash
git push -u origin main
```

Now your code is **online**! 🎉

---

# **Working With GitHub (Branches, Pull Requests & Forking)**

## **Branches – So You Don’t Break the Main Project**

A **branch** is like creating a **copy of your project** where you can experiment without breaking the original.

### **Creating & Switching to a Branch**

```bash
git branch new-feature
git checkout new-feature
# Or do both in one step
git checkout -b new-feature
```

Now you can **make changes** without touching `main`.

Once your work is done, switch back to `main` and merge it:

### **Merging Your Branch Back Into Main**

```bash
git checkout main
git merge new-feature
```

This is a Flow of how branch works :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1740572778491/9e3f5a2a-6f25-4d02-8d2e-395080f39888.png align="center")

---

## **Pull Requests – Asking Permission to Merge**

When working with a team (or contributing to open-source), you **don’t** merge changes directly. Instead, you create a **Pull Request (PR)** to ask for approval.

### **How to Create a Pull Request**

1. Push your branch to GitHub:
    
    ```bash
    git push origin new-feature
    ```
    
2. Go to GitHub and click **Compare & Pull Request**.
    
3. Add a **title** and **description** (e.g., *"Added new feature"*) and submit.
    
4. Wait for approval (or approve it yourself if it’s your project).
    
5. Click **Merge** to add your changes.
    

---

## **Forking – Making Your Own Copy of Someone Else’s Project**

Forking lets you **copy someone else’s GitHub project** and work on it **without affecting the original**.

### **How to Fork a Repository**

1. Go to any public repo on GitHub.
    
2. Click **Fork** (top-right corner).
    
3. This creates **your own copy** under your GitHub account.
    
4. Clone it to your computer:
    
    ```bash
    git clone https://github.com/your-username/forked-repo.git
    ```
    
5. Make changes, push them, and **open a Pull Request** if you want the original creator to accept your changes.
    

---

# **Common Git Commands Cheat Sheet**

| **Command** | **What It Does** |
| --- | --- |
| `git init` | Start a new Git project |
| `git status` | Check the status of your files |
| `git add .` | Add all files to Git |
| `git commit -m "message"` | Save changes |
| `git log` | See commit history |
| `git branch` | List branches |
| `git checkout branch-name` | Switch to a branch |
| `git merge branch-name` | Merge a branch |
| `git push origin main` | Push changes to GitHub |
| `git pull origin main` | Get updates from GitHub |

---

# **Final Thoughts (Things I Messed Up Today)**

* Forgot to create a branch and edited `main` directly. Oops.
    
* Wrote a Pull Request description that just said *“fixed stuff”* (very helpful, I know).
    
* Tried forking my own repo just to see what happens (spoiler: nothing exciting).