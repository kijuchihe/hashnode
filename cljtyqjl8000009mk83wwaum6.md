---
title: "Getting Started with Git and GitHub"
datePublished: Sat Jul 08 2023 12:09:34 GMT+0000 (Coordinated Universal Time)
cuid: cljtyqjl8000009mk83wwaum6
slug: getting-started-with-git-and-github
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1688818118380/e85461f3-bff4-44f1-b3bd-5df9dc5194f6.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1688818157826/2e49b374-0709-4053-ace7-afcd098d382b.png
tags: github, git

---

## Introduction to Git and GitHub

Git is a distributed version control system that allows developers to track changes in their codebase and collaborate with others effectively. GitHub, on the other hand, is a web-based platform that provides hosting for Git repositories and offers additional features for collaboration.

## Installing Git

To start using Git, you'll need to install it on your computer. Follow these steps:

1\. **Windows**: Download the Git installer from the official Git website (https://git-scm.com/downloads) and run it. Follow the installation instructions and choose the default settings.

2\. **Mac**: You can install Git using Homebrew, a popular package manager. Open Terminal and run the command: `brew install git`

3\. **Linux**: Use your distribution's package manager to install Git. For example, on Ubuntu, run the command: `sudo apt-get install git`

## Configuring Git

Once Git is installed, you need to configure it with your name and email address. Open your terminal and run the following commands, replacing `Your Name` with your actual name and `your-email@example.com` with your email address:

```bash
git config --global user.name "Your Name"
```

## Creating a Repository

To create a new Git repository, follow these steps:

1\. **Local Repository**: Open your terminal, navigate to the desired directory, and run the command: git init. This will initialize a new Git repository in that directory.

2\. **GitHub Repository**: Go to GitHub (https://github.com) and sign in to your account. Click on the "+" button in the top-right corner and select "New repository". Follow the instructions to create a new repository on GitHub.

## Cloning a Repository

To clone an existing repository from GitHub, use the following command:

```bash
git clone <repository-url>
```

Replace `<repository-url>` with the URL of the repository you want to clone. This will create a local copy of the repository on your computer.

## Basic Git Commands

Here are some essential Git commands to help you get started:

\- `git status`: Shows the current status of your repository, including modified files and untracked files.

\- `git add <file>`: Adds a specific file or directory to the staging area. To add all files in the directory, simply type `git add .`

\- `git commit -m "Commit message"`: Commits the changes in the staging area with a descriptive commit message.

\- `git push`: Pushes your local commits to the remote repository on GitHub. Recall that the remote repository is the one on github. Pushing code is like syncing the code on your local repository - the one on your system - to the one one github.

\- `git pull`: Fetches and merges the latest changes from the remote repository to your local repository.

\- `git branch`: Lists all branches in your repository.

\- `git checkout <branch>`: Switches to a specific branch.

\- `git merge <branch>`: Merges a branch into the current branch.

## Collaborating on GitHub

GitHub provides powerful collaboration features. Here are a few key commands:

\- `git fork`: Creates a copy of a repository under your GitHub account.

\- `git pull-request`: Submits a pull request to propose changes to the original repository.

\- `git clone <forked-repository-url>`: Clones a forked repository to your local machine.

\- `git remote add upstream <original-repository-url>`: Adds a connection to the original repository.

\- `git fetch upstream`: Fetches the latest changes from the original repository.

\- `git merge upstream/main`: Merges the changes from the original repository into your local repository.

## Conclusion

Congratulations! You've learned the basics of using Git and GitHub. This article covered installing Git, configuring it, creating and cloning repositories, essential Git commands, and collaborating on GitHub. Remember to explore additional features and commands as you continue your journey with Git and GitHub.

I will release another article for a better understanding of some of the terms and commands used in this article. Also, for a better understanding of the differences between the terms `git` and `github`