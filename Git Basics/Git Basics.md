# Introduction
In this lesson, we’ll cover common Git commands used to manage your projects and to upload your work onto GitHub. We refer to these commands as the basic Git workflow. When you’re using Git, these are the commands that you’ll use 70-80% of the time. Mastering these commands will take you more than halfway to mastering Git!

## Lesson Overview
This section contains a general overview of topics that you will learn in this lesson:

- How to create a repository on GitHub.
- How to get files to and from GitHub.
- How to take “snapshots” of your code.

## Assignment

### Before You Start!
GitHub recently updated the way it names the default branch. This means you need to make sure you are using a recent version of Git (2.28 or later). You can check your version by running:

```sh
git --version
```

If you haven’t already, set your local default Git branch to `main` by running:

```sh
git config --global init.defaultBranch main
```

For more information on the change from `master` to `main`, see GitHub’s [Renaming Repository](https://github.com/github/renaming).

## Create the Repository

You should have already created a GitHub account in the Setting Up Git lesson.

1. From the GitHub homepage, create a new repository by clicking the "+" button in the top-right corner and selecting "New repository".
2. Name your repository `git_test`.
3. Check "Add a README file".
4. Click "Create repository".
5. Once redirected to your repository page, click the green "Code" button, select the SSH option, and copy the SSH URL.

## Clone the Repository

Create a directory for your Git projects:

```sh
mkdir ~/repos
cd ~/repos
```

Clone your repository using the copied SSH URL:

```sh
git clone git@github.com:USER-NAME/git_test.git
```

Verify the remote repository is connected:

```sh
cd git_test
git remote -v
```

Expected output:

```sh
origin  git@github.com:USER-NAME/git_test.git (fetch)
origin  git@github.com:USER-NAME/git_test.git (push)
```

## Use the Git Workflow

### Add and Commit a File

1. Create a new file:

```sh
touch hello_world.txt
```

2. Check status:

```sh
git status
```

3. Add the file to the staging area:

```sh
git add hello_world.txt
```

4. Commit the file:

```sh
git commit -m "Add hello_world.txt"
```

5. Verify commit history:

```sh
git log
```

### Modify and Stage Files

1. Open `README.md` in your editor, add "Hello Odin!", and save.
2. Check status:

```sh
git status
```

3. Add changes to staging:

```sh
git add README.md
```

4. Modify `hello_world.txt`, save, and stage all changes:

```sh
git add .
```

5. Commit changes:

```sh
git commit -m "Edit README.md and hello_world.txt"
```

6. Verify commit history:

```sh
git log
```

## Push Changes to GitHub

```sh
git push origin main
```

Verify status:

```sh
git status
```

Your GitHub repository should now reflect the changes.

## Avoid Editing Directly on GitHub

Making changes directly on GitHub can cause conflicts. Instead, modify local files, commit, and push changes using Git commands.

## Cheatsheet

### Remote Repository Commands

```sh
git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
git push origin main
```

### Workflow Commands

```sh
git add .
git commit -m "Commit message"
```

### Status and Log Commands

```sh
git status
git log
```

### Basic Git Syntax

- `git add .` → Add all changes in the current directory to the staging area.
- `git commit -m "message"` → Save changes with a descriptive message.
- `git push origin main` → Upload committed changes to GitHub.

By following these steps, you are well on your way to mastering Git!

