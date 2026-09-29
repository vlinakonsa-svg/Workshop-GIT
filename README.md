# Git & GitHub Configuration and Workflow Notes

A comprehensive study guide for basic Git and GitHub repository configuration and workflow.

---

## 1. Repository Setup & Initialization

### Step 1: Create a GitHub Repository

Create a new empty repository on GitHub named:

```text
Hello-world
```

For example:

```text
https://github.com/your-username/Hello-world.git
```

---
### Step 2: Clone the Repository

Navigate to the directory where you want to store the project:

```bash
cd ..
```

Clone the GitHub repository:

```bash
git clone https://github.com/your-username/Hello-world.git
```

### What does `git clone` do?

`git clone` downloads a copy of the remote GitHub repository onto your computer.

After cloning, you will have a directory similar to:

```text
Hello-world/
└── .git/
```

The hidden `.git` directory contains the Git repository information and history.

---

### Step 3: Enter the Project Directory

Move into the cloned repository:

```bash
cd Hello-world
```

You should normally run your Git commands from inside this directory.

---

### Step 4: Configure the Remote URL

This step is optional if you used `git clone`, because cloning automatically creates a remote named `origin`.

You can update the remote URL with:

```bash
git remote set-url origin https://github.com/your-username/Hello-world.git
```

Check the configured remote:

```bash
git remote -v
```

---

## 2. Creating and Modifying Files

You can use the `echo` command to create files or write content into them.

Example:

```bash
echo Hello-world >> README.md
```

The `>>` operator **appends** text to a file.

If `README.md` does not exist, it will normally be created.

If it already exists, the new text will be added to the end.
