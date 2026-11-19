# Experiment 26: Cloning a GitHub Repository and Editing Files Locally

## Aim

To clone an existing GitHub repository to a local computer, edit files using a code editor, and push the changes back to GitHub.

## Software Requirements

- Git installed on the computer
- A GitHub account
- Visual Studio Code or another text editor
- Internet connection
- Terminal (macOS/Linux) or Git Bash/Command Prompt (Windows)

## Introduction

Git is a distributed version control system that tracks changes made to files. GitHub is an online platform for hosting Git repositories.

**Cloning** means creating a local copy of a remote GitHub repository. After cloning, files can be edited locally. The changes can then be staged, committed, and pushed to the remote repository.

## Procedure

### Step 1: Open the GitHub repository

Open the repository:

[https://github.com/Rohith-192007/exp-26](https://github.com/Rohith-192007/exp-26)

Select **Code** and copy the HTTPS clone URL:

```text
https://github.com/Rohith-192007/exp-26.git
```

### Step 2: Open the terminal

Open Terminal on macOS/Linux or Git Bash/Command Prompt on Windows. Move to the folder where you want to save the project.

Example:

```bash
cd Desktop
```

### Step 3: Clone the repository

Run:

```bash
git clone https://github.com/Rohith-192007/exp-26.git
```

Git downloads the repository and creates a local folder named `exp-26`.

### Step 4: Enter the cloned folder

```bash
cd exp-26
```

### Step 5: Open the project in Visual Studio Code

If the `code` command is installed, run:

```bash
code .
```

Alternatively, open Visual Studio Code and select **File → Open Folder**, then choose the cloned `exp-26` folder.

### Step 6: Edit a file locally

Open `README.md` in the editor. Add or modify a line, for example:

```markdown
## Local Editing

This line was added after cloning the repository to my computer.
```

Save the file.

### Step 7: Check the changes

Run:

```bash
git status
git diff
```

- `git status` shows which files have been modified.
- `git diff` displays the changes made to tracked files.

### Step 8: Stage the changes

```bash
git add README.md
```

To stage all modified and new files in the project, use `git add .` instead.

### Step 9: Commit the changes

```bash
git commit -m "Update README after local editing"
```

A commit records the staged changes in the local Git repository.

### Step 10: Push the changes to GitHub

```bash
git push origin main
```

If GitHub requests authentication, complete the sign-in flow using a GitHub-supported method. Do not share passwords or access tokens.

### Step 11: Verify the changes

Refresh the GitHub repository page and check that the updated README is visible.

## Important Git Commands

| Command | Description |
|---|---|
| `git clone URL` | Downloads a remote repository |
| `cd folder-name` | Enters the project folder |
| `git status` | Shows the current working-tree status |
| `git diff` | Displays local file changes |
| `git add README.md` | Stages the selected file |
| `git commit -m "message"` | Records staged changes |
| `git push origin main` | Pushes commits to the remote main branch |
| `git pull` | Fetches and integrates remote changes |

## Workflow

```text
GitHub Repository
       |
       | git clone
       v
Local Repository
       |
       | Edit files
       v
Modified Files
       |
       | git add
       v
Staging Area
       |
       | git commit
       v
Local Commit
       |
       | git push
       v
Updated GitHub Repository
```

## Result

The GitHub repository was cloned to the local computer. A file was edited and saved locally. The changes were checked, staged, committed, and pushed to GitHub. The updated file was then verified on the GitHub repository page.

## Repository

[https://github.com/Rohith-192007/exp-26](https://github.com/Rohith-192007/exp-26)
