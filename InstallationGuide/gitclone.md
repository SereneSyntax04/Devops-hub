# Cloning a Git Repository in VS Code

This guide explains **step-by-step** how to clone a Git repository using **Visual Studio Code (VS Code)**. You can use either the **VS Code UI** or the **integrated terminal**.

---

## Prerequisites

Before you begin, make sure you have:

* **Visual Studio Code** installed
* **Git** installed on your system
* A valid **repository URL** (GitHub / GitLab / Bitbucket)

### Check Git Installation

Open a terminal and run:

```bash
git --version
```

If Git is not installed, download it from:

* [https://git-scm.com/downloads](https://git-scm.com/downloads)

Restart VS Code after installing Git.

---

## Method 1: Clone Using VS Code UI (Recommended)

### Step 1: Open VS Code

Launch **Visual Studio Code**.

### Step 2: Open Command Palette

Press:

* **Windows / Linux:** `Ctrl + Shift + P`
* **macOS:** `Cmd + Shift + P`

### Step 3: Run Git Clone Command

* Type `Git: Clone`
* Select **Git: Clone** from the list

### Step 4: Enter Repository URL

* Paste the repository URL (HTTPS or SSH)

**Example:**

```
https://github.com/username/repository-name.git
```

### Step 5: Choose Destination Folder

* Select a folder on your system where the repo should be cloned

### Step 6: Open the Repository

* Once cloning completes, click **Open** when VS Code prompts you

✅ The repository is now cloned and ready to use.

---

## Method 2: Clone Using VS Code Terminal

### Step 1: Open VS Code Terminal

* Go to **View → Terminal**
* Or press **Ctrl + `** (backtick)

### Step 2: Run Git Clone Command

```bash
git clone https://github.com/username/repository-name.git
```

### Step 3: Open the Project Folder

```bash
cd repository-name
code .
```

✅ The project opens in VS Code.

---

## Authentication Notes

### HTTPS

* GitHub now requires a **Personal Access Token (PAT)** instead of a password

### SSH (Optional)

* Ensure an SSH key is generated and added to your Git provider

---

## Common Errors & Fixes

### ❌ `git: command not found`

* Install Git and restart VS Code

### ❌ Authentication Failed

* Use a Personal Access Token (for HTTPS)
* Or verify SSH key setup

### ❌ Permission Denied (SSH)

* Confirm your SSH key is added to GitHub/GitLab

---

## Useful VS Code Git Features

* **Source Control Panel** (left sidebar) for commits & changes
* **GitHub Account Sign-in** (bottom-left corner)
* Built-in diff viewer and branch management

---
