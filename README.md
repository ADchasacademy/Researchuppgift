# Introduction 
This document provides an introduction to Markdown Syntax, Github, Terminal and Git.

# Table Of Contents
- [Markdown Syntax](#markdown-syntax)
    - [Example](###example)
- [Terminal](#terminal)
- [Github](#github)
- [Git](#git)


# Markdown Syntax
This text file has been formatted using the Markdown markup language. Markdown is a markup language that adds formatting elements to plain text without using text editor programs such as Word, google docs or files as HTML or CSS. 


### Example:
*[Escaping characters](https://www.markdownguide.org/basic-syntax/#escaping-characters) can be used if you dont want Markdown Syntax to render the text*

| Markdown    |      HTML      |  Rendered Output |
|----------|:-------------:|------:|
| \#Heading | \<h1>Heading\</h1> |<h1>Heading</h1>|
| \*\*Bold\*\*  |    \<b>Bold\</b>   |   <b>Bold</b>|
| \*Italic\*  |    \<em>Italic\</em>   |   <em>Italic</em>|


For more information, check
[Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)



# Terminal



# Git

### Git commands picked up during lecture:
| Command | Explanation |
|:---	|:---	|
| **git --version** | Checks which Git version is being used. |
| **git init** |  Initializes a Git repository.	|
| **git clone *[url]*** |  Retrieves a repository to local client.	|
| **git status** |  Shows modified files.	|
| **git add *[file]*** |  Stageds a file in current state in preparation to be commited.	|
| **git add .** |  Stageds  **all files** in current state in preparation to be commited.	|
| **git commit -m *“[descriptive.message]”*** |  Commits all staged content.|
| **git push -u origin *[branch.name]*** |  Pushes local branch commits to remote Git branch	|
| **git branch *[branch.name]*** |  Creates a new branch.	|
| **git branch log** |  See branches	|
| **git checkout *[branch.name]*** |  Switch between branches.	|
| **git merge *[branch.name]*** |  Merges selected branch into current branch.	| 

To check out more Git commands, visit [GIT CHEAT SHEET](https://education.github.com/git-cheat-sheet-education.pdf)



### Additinal Git commands picked up while making this README.md:
| Command | Explanation |
|:---	|:---	|
| **git branch *[branch.name]*** | Creates a new branch. But does not navigate to branch. |
| **git branch -b *[branch.name]*** |  Creates a new branch and navigates to the new branch.	|
| **git commit** |  Commits staged files, by default with Vim, to insert text use **i**  and to exit intert mode use **Esc**,to **save** commit in Vim use :x, to **exit** use :q, to **search** use /, in search mode you can **move forward** with n and **move backwards** with N |
| **git commit --amend** |  Edits recent commit.	|
| **git branch -d *[branch.name]*** |  Deletes selected branch.	|
| **git diff --staged** |  Compares the staged changes with local repository. |
| **git push -f** |  Forces a push from local client. (*avoid using this* :cold_sweat:)	|

I have also learned how to properly commit using descriptive messages that follow the Git Commit Convention, check [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) for more information. 



## How to retrieve and push commits using Git:
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
    git push -u origin [*branch.name*]
    ```



