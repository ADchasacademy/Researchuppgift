# Introduction 
This document provides an introduction to Markdown Syntax, Github, Terminal and Git.

# Table Of Contents
- [Markdown Syntax](#markdown-syntax)
    - [Example](#example)
- [Terminal Commands](#terminal-commands)
    - [Terminal commands picked up during lecture](#terminal-commands-picked-up-during-lecture)
    - [Terminal commands picked up by working on this project](#terminal-commands-picked-up-by-working-on-this-project)
- [Github](#github)
- [Git](#git)

    - [Git commands picked up during lecture](#git-commands-picked-up-during-lecture)
    - [Additional Git commands picked up while making this README.md](#additional-git-commands-picked-up-while-making-this-readmemd)
    - [How to retrieve and push commits using Git](#how-to-retrieve-and-push-commits-using-git)

![#Markdown](/markdown.png)
# Markdown Syntax
This text file has been formatted using the Markdown markup language. Markdown is a markup language that adds formatting elements to plain text without using text editor programs such as Word, google docs or files as HTML or CSS. 


### Example:
*[Escaping characters](https://www.markdownguide.org/basic-syntax/#escaping-characters) can be used if you don't want Markdown Syntax to render the text*

| Markdown    |      HTML      |  Rendered Output |
|----------|:-------------:|------:|
| \#Heading | \<h1>Heading\</h1> |<h1>Heading</h1>|
| \*\*Bold\*\*  |    \<b>Bold\</b>   |   <b>Bold</b>|
| \*Italic\*  |    \<em>Italic\</em>   |   <em>Italic</em>|


For more information, check
[Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)


 
![#Terminal](/terminal.png )
# Terminal commands

### Terminal commands picked up during lecture:

| Command | Explanation |
|:---	|:---	|
| **cd [folder/file]** | Enters another directory. |
| **cd ..** |  Goes one directory backwards. |
| **rm *[file.name]*** | deletes directory |
| **ls** |  Shows all folders or files in the current directory.	|
| **echo "*[text]*" > *[file.format]*** | Creates a file and adds everything that has been added in the string. |
| **ls -la*** |  Shows hidden folders or files in the current directory.	|
| **mkdir *[folder.name]*** |  Creates a folder in the current directory.	|
| **cat *[file]*** |  Displays file content.	|
| **touch [folder.name]** |  Creates a folder in the current directory. 	|
| **pwd*** |  Prints current directory in terminal on command prompt. |

### Terminal commands picked up by working on this project:

| Command | Explanation |
|:---	|:---	|
| **exit** | Terminates terminal. |
| **clear** | Clears terminal window. |
| **code .** |  Launches code to the chosen editor program. *PS! enter this code through the correct directory so that the chosen editor program knows which branch to launch.* |


 
![#Github](/github.png )
# Github
Github is a developer platform that allowes users to create, store and share repositories. Github can also be used as a GUI (*Graphical User Interface*), as it allows the users to interact with their repositories through the web interface. Such as creating repositories through the platform instead of using Git Terminal. 


![#Git](/git.png)
# Git

### Git commands picked up during lecture:
| Command | Explanation |
|:---	|:---	|
| **git --version** | Checks which Git version is being used. |
| **git init** |  Initializes a Git repository.	|
| **git clone *[url]*** |  Retrieves a repository to local client.	|
| **git status** |  Shows modified files.	|
| **git add *[file]*** |  Stages a file in the current state in preparation to be committed.	|
| **git add .** |  Stages  **all files** in current state in preparation to be committed.	|
| **git commit -m *“[descriptive.message]”*** |  Commits all staged content to current branch.|
| **git push -u origin *[branch.name]*** |  Pushes selected local branch to remote Git branch.	|
| **git branch *[branch.name]*** |  Creates a new branch.	|
| **git branch** |  See branches.	|
| **git checkout *[branch.name]*** |  Switch between branches.	|
| **git merge *[branch.name]*** |  Merges selected branch into current branch.	| 

To check out more Git commands, visit [GIT CHEAT SHEET](https://education.github.com/git-cheat-sheet-education.pdf)



### Additional Git commands picked up while making this README.md:
| Command | Explanation |
|:---	|:---	|
| **git branch *[branch.name]*** | Creates a new branch. But does not navigate to the branch. |
| **git branch -b *[branch.name]*** |  Creates a new branch and navigates to the new branch.	|
| **git commit** |  Commits staged files, by default with Vim, to insert text use **i**  and to exit insert mode use **Esc**,to **save** commit in Vim use :x, to **exit** use :q, to **search** use /, in search mode you can **move forward** with n and **move backwards** with N |
| **git commit --amend** |  Edits recent commit.	|
| **git branch -d *[branch.name]*** |  Deletes selected branch.	|
| **git diff --staged** |  Compare the staged changes with the local repository. |
| **git push -f** |  Forces a push from a local client. (*Avoid using this* :cold_sweat:)	|

I have also learned how to properly commit using descriptive messages that follow the Git Commit Convention, check [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) for more information. 



### How to retrieve and push commits using Git:
*An example showing how to retrieve a repository from a hosted location, such as Github, via url and how to push staged changes from a local branch to a remote repository branch*

1. **Clone the repository:**
    ```bash
    git clone https://github.com/ADchasacademy/Researchuppgift.git
    ```
2. **After changes have been made, stage all files (*or a specific file using git add [file.name]*):**
    ```bash
    git add .
    ```
3. **Commit staged files:**
    ```bash
    git commit -m "initial commit" 
    ```
 4. **Push local branch to remote repository branch:**
    ```bash
    git push -u origin [branch.name]
    ```



