# Intro to Contributing with GitHub

Welcome to the world of version control with Git and GitHub. This guide will walk you through the fundamental commands you'll need to start contributing to projects. Remember, before making any changes, always pull the latest updates from the repository.

## Essential Git Commands

Here are the core Git commands you will use regularly:

- `git pull`: Fetch and merge changes from the remote server to your working directory
- `git push`: Send your commits to the remote repository
- `git commit`: Save your changes with a descriptive message
- `git branch`: Manage branches in your repository
- `git checkout`: Switch between branches or restore files
- `git clone`: Copy a repository from GitHub to your local machine

## Step-by-Step Guide

### Step 1: Cloning a Repository

To start working on a project, you first need to clone its repository from GitHub.

```bash
git clone [repository link]
```

#### How to get the **[repository link]**?

1. Go to the main page of the repository on GitHub.
2. Click on the "Clone or download" button.
3. Copy the link provided.

### Step 2: Pulling Changes

Before you start coding, ensure your local copy is up to date by running:

```bash
git pull
```

This command helps avoid conflicts by updating your local repository with the latest changes from the remote server.

### Step 3: Making Changes

Once your repository is up to date, you can start making changes. After you've modified existing files or added new files, you need to stage these changes for a commit.

#### Adding Changes

You can add all modified files using:

```bash
git add .
```

Or add a specific file:

```bash
git add [file name]
```

Using `git add .` adds all changes in the directory, whereas `git add [file name]` allows you to specify which changes to stage, which is useful for excluding temporary or experimental changes.

### Step 4: Committing Changes

After staging your changes, you should commit them with a clear, descriptive message:

```bash
git commit -m "Your detailed commit message"
```

Example:
```bash
git commit -m "Added documentation for motor commands in moteus_test.py"
```

Your commit message should succinctly describe what the changes do and why, if necessary.

### Step 5: Pushing Changes

To share your commits with others, push your changes to the remote repository:

```bash
git push
```

If it's the first time you're pushing, you might need to set the upstream branch:

```bash
git push --set-upstream origin [branch-name]
```

### Handling Merge Conflicts

If there is a conflict between your changes and the changes on the server, `git pull` will warn you. To resolve conflicts, manually edit the files to correct the discrepancies and then:

```bash
git add [resolved-file]
git commit -m "Resolved merge conflict by [your resolution]"
```

### Working with Branches

To create a new branch:

```bash
git branch [new-branch-name]
```

To switch to an existing branch:

```bash
git checkout [branch-name]
```

### Remember:

**Please `git pull` before you start coding to synchronize your local repository with the remote.**

This guide covers the basics of working with Git and GitHub. There are many other commands and options you may find useful as you become more comfortable with Git.
