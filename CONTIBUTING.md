# Intro to Contributing with GitHub

Welcome to the world of version control with Git and GitHub. This guide will walk you through the fundamental commands you'll need to start contributing to projects. Remember, before making any changes, always pull the latest updates from the repository.

## Essential Git Commands

Here are the core Git commands you will use regularly:

- `git fork`: Make a copy of someone else's repository to your GitHub account
- `git clone`: Copy a repository from GitHub to your local machine
- `git pull`: Fetch and merge changes from the remote server to your working directory
- `git push`: Send your commits to the remote repository
- `git commit`: Save your changes with a descriptive message
- `git branch`: Manage branches in your repository
- `git checkout`: Switch between branches or restore files

## Step-by-Step Guide

### Step 1: Forking a Repository

Before you can start working on a project, if you don't have write access to the repository, you will need to create a fork.

1. Go to the main page of the repository on GitHub.
2. At the top-right of the page, click the "Fork" button.
3. This creates a copy of the repository under your GitHub account. Now, you can make changes to your fork without affecting the original repository.

### Step 2: Cloning a Repository

Once you have forked the repository, you need to clone it to your local machine to start working on it.

```bash
git clone [forked repository link]
```

#### How to get the **[forked repository link]**?

1. Navigate to your fork on GitHub (it should be at `https://github.com/your-username/repository-name`).
2. Click on the "Clone or download" button.
3. Copy the link provided.

### Step 3: Pulling Changes

Before you start coding, ensure your local copy is up to date by running:

```bash
git pull
```

This command helps avoid conflicts by updating your local repository with the latest changes from the remote server.

### Step 4: Making Changes

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

### Step 5: Committing Changes

After staging your changes, you should commit them with a clear, descriptive message:

```bash
git commit -m "Your detailed commit message"
```

Example:
```bash
git commit -m "Added documentation for motor commands in moteus_test.py"
```

### Step 6: Pushing Changes

To share your commits with others, push your changes to the remote repository:

```bash
git push
```

If it's the first time you're pushing, you might need to set the upstream branch:

```bash
git push --set-upstream origin [branch-name]
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

### Handling Common Conflicts

#### Common Conflicts with Git Pull
Conflicts can occur when pulling updates. Here are scenarios and solutions:

##### Merge Conflicts
- **Modified Same Lines**: Manual resolution is needed when the same lines are changed in your local and the remote.
- **Deleted vs. Modified Files**: Decide whether to keep the deletion or modification during the merge.

##### Local Changes Not Committed
- **Uncommitted Changes**: Commit, stash, or discard your changes before pulling to avoid conflicts.

##### Branch Issues
- **Tracking Different Branches**: Ensure your local branch tracks the correct upstream branch.

##### Other Potential Issues
- **File Permission and Disk Space Issues**: Ensure you have adequate permissions and disk space.

#### Handling Merge Conflicts
1. **Use `git status`** to check the state of your repository.
2. **Stash Uncommitted Changes**: Use `git stash` to save uncommitted changes temporarily.
3. **Resolve Merge Conflicts**: Edit the files to fix conflicts or use a merge tool.
4. **Commit Resolved Conflicts**: Commit the resolved changes.

#### Potential Conflicts During Git Push
Push conflicts usually stem from diverged branch histories.

##### Non-Fast-Forward Updates
- **Remote Changes**: Pull and merge changes before pushing to integrate remote updates smoothly.

##### Rejected Due to Conflicting Changes
- **Concurrent Modifications**: Fetch the latest changes, resolve any conflicts, and then push again.

##### Branch Protection Rules
- **Restricted Push Access**: Use pull requests to propose your changes for protected branches.

##### Other Possible Issues
- **Authentication and Large Push Size**: Ensure correct credentials and consider pushing smaller sets of changes.

#### Tips for Smooth Collaboration
- **Communicate with Collaborators**: Avoid overlapping modifications.
- **Pull Before Pushing**: Always update your branch before starting work.
- **Follow Branch Protection Rules**: Respect the workflows established in your project.

### Conclusion
Remember, the key to successful use of Git is consistent communication and adherence to project workflows. Always pull the latest changes before starting work and resolve conflicts as they arise to maintain a clean project history.

By following these guidelines and using the commands provided, you can effectively manage your contributions to any project on GitHub.

### Remember:

**Please `git pull` before you start coding to synchronize your local repository with the remote.**

This guide covers the basics of working with Git and GitHub. There are many other commands and options you may find useful as you become more comfortable with Git.
