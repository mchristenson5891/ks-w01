# Command Line and git

## Lesson Objectives

-   Navigating folders with Terminal
-   Command Line commands
-   Git repository
-   Pull, Push, and Merge

## Learning Objective

-   Learners will be able to create a folder and files using the Terminal
-   Learner will be able to explain in their own words how developers use git

## Terminal

> Why do you think some developers use the terminal to navigate their computers vs using their mouse?

Open the terminal by first opening Spotlight `⌘ (Command) + Space` and then start typing out the word `terminal`. Then hit `enter`

## Command Line Interface

-   Terminal gives us access to Command Line Interface (CLI) to the operating system.
-   You can give your computer direct, text-based instructions.
-   It's the most powerful piece of software on your computer!
-   Think of it as the central hub of your development process.
-   For now, we will use it to navigate the files and folders/directories in our computer.

When terminal launches, it will start in your computer's home directory (whatever you named your computer). Your home directory is denoted by the tilde ~.

## Bash

Bash is a type of Shell. It understands commands written in the bash scripting language. The commands are abbreviations of English words, or acronyms.

`pwd` - will print the current working directory. It shows you a path. This path shows you where are curently located in the filesystem.

`ls` - Lists the contents of the current directory.

-   You can see the immediate child directories (the directories inside this directory)
-   the files and directories that are not hidden.

Flags

-   Commands can take flags denoted by a dash -
-   `ls -a` - list content including hidden files and directories. Hidden files and directories begin with a period, for example, `.git`.
-   `ls -l` - list with details

There are also double-dash flags/options on most commands, for example many commands have the `--help` option:

-   `nano --help`

---

-   Create a folder
    -   mkdir - makes a directory

```sh
mkdir mern
```

-   Move into dirctory/folder

```sh
cd mern
```

-   Create a file

    -   touch - creates an empty file. A file typically will have a file extension like .txt whereas a directory will not.

```sh
touch index.html
```

-   Add to the file

    -   echo is a built-in command in the bash and C shells that writes its arguments to standard output

```sh
echo "Hello you!" >> index.html
```

-   Delete file

    -   The rm utility attempts to remove the non-directory type files specified on the command line.

```sh
rm index.html
```

-   Move out of the folder

```sh
cd ..
```

-   Create new folder

```sh
mkdir new_mern
```

-   Copy the folder

    -   `cp` command to make a copy of a file. The `-R` flag causes cp to copy the folder and its contents

```sh
cp -R mern new_mern
```

-   Delete a folder
    -   The rm utility attempts to remove the non-directory type files specified on the command line.

```sh
rm -R mern
```

-   Open nano (GNU nano is a text editor for Unix-like computing systems or operating environments using a command line interface.)

```sh
nano
```

-   Exit nano

`control + x`

## git

-   Initialize a repository
    -   The git init command creates a new Git repository.

```sh
git init
```

-   Add
    -   The git add command adds a change in the working directory to the staging area.

```sh
git add .
```

-   Commit
    -   The git commit command is one of the core primary functions of Git. Prior use of the git add command is required to select the changes that will be staged for the next commit. Then git commit is used to create a snapshot of the staged changes along a timeline of a Git projects history. The `-m` flag is a short way to add ac commit message.

```sh
git commit -m "your message here"
```

-   Push
    -   The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo. It's the counterpart to git fetch , but whereas fetching imports commits to local branches, pushing exports commits to remote branches.

```sh
git push origin <name of branch>
```

-   Pull
    -   The git pull command is used to fetch and download content from a remote repository and immediately update the local repository to match that content.

```sh
git pusll origin <name of branch>
```

-   Merge
    -   Merging is Git's way of putting a forked history back together again. The git merge command lets you take the independent lines of development created by git branch and integrate them into a single branch.

```sh
git merge <name of branch>
```

## Guided Practice (Pair Programming)

-   Have students pair up (CF will chose pairs) and one person create a folder with a file inside then exit out of the terminal
-   Have their partner open the terminal and navigate to the folder that was created and go inside of the file that was created and add something
-   Show them shortcuts
-   Have them switch roles

## Independent Practice

-   Test each other on commands

## Wrap-up (10 min)

-   Have 2-4 students explain concept(s) in their own words
-   Review lesson objective (Internal)
-   Check for completion of Lesson Objective
