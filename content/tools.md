---
layout: layouts/base.njk
eleventyExcludeFromCollections: true
---

# Piazza
This term we will be using Piazza for class discussion. The system is highly catered to getting you help fast and efficiently from classmates, and myself. I encourage you to post your questions on Piazza.

Find our class signup link [here](https://piazza.com/stuyvesant_high_school/fall2023/mks21x)

# Git
It is an open-source version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers collaboratively developing source code during software development.

## GitHub
It is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere. This tutorial teaches you GitHub essentials like repositories, branches, commits, and pull requests. 

## Installing Git
**Mac and Linux:** Git should be installed already.

Windows: Install git and the shell gitbash from [here](https://gitforwindows.org/). This includes git, gitbash, and has shell integration so that you can right-click on a folder in Windows Explorer to access gitbash at that location.

## Git commands
**The git config command**

```
git config --global user.name "YOUR_NAME_HERE"
git config --global user.email YOUR_EMAIL_HERE
```

The basic commands we are going to use in this class are:

- **git clone:** Retrieve an entire repository from a hosted location via URL.
- **git pull:** Fetch and merge any commits from the tracking remote branch.
- **git add:** Add a file as it looks now to your next commit (stage).
- **git commit:** Commit your staged content as a new commit snapshot.
- **git push:** Transmit local branch commits to the remote repository branch.

You may take a look at the git reference [sheet](https:**//education.github.com/git-cheat-sheet-education.pdf).

## Connect to GitHub with SSH
Follow these steps to create an ssh key, connect to GitHub using SSH, and clone your repository.

1. Create your ssh key: Open your terminal and type

    `ssh-keygen -t ed25519`

    Check if your key was generated:
    ```
            cd .ssh/
            ls
    ```     
    You should see your private key (`id_ed25519`) and public key (`id_ed25519.pub`) inside that directory.

2. Log in to your GitHub account.

    Click on your profile picture (right-top). You will see a menu; click on [Settings](https://github.com/settings/keys).

    You will see a menu on the left. Click on SSH and GPG keys and click on Add New SSH key.

    You will give a title to that key. The key type should be "Authentication Key" and copy your public key (the content inside the file id_ed25519.pub) in the field "Key".

3. Go to the following [link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection) and test your SSH connection.

4. Let's clone your repository on your local computer:

    Go to your assignments repository that you created for this class in GitHub. You will see a green button, "Code". You must click on that button and select SSH to have the appropriate link that will allow you to clone your repository and copy the link you see there.

5. On your terminal, go inside the folder you want to clone your repository and type:
    ```
    git clone PASTE_THE_LINK_YOU_COPIED_FROM_GITHUB_(git@...)
    ```

6. Go inside the folder that appears after you execute the clone command, and you will see the files you have on your GitHub repository.
