1. .gitignore
2. git remote -v
3. git clone practice
4. Markdown formatting
5. terminal shortcuts
---

# 2. git remote -v

## What is `git remote -v`?

`git remote -v` shows the online repository that my local project is connected to.

In my case, it shows the GitHub link connected to my local project.

Simple meaning:

```text
git remote -v = show the GitHub repo connected to this project
```

---

## Terminal command

```bash
git remote -v
```

## What the syntax means

```text
git = use Git

remote = show or manage remote repository connections

-v = verbose, meaning show more detail
```

Simple meaning:

```text
Show me the remote GitHub link connected to my local project.
```

---

## Example output

```text
origin  https://github.com/Adiotayo/Devop-learning-journey-.git (fetch)
origin  https://github.com/Adiotayo/Devop-learning-journey-.git (push)
```

## What the output means

```text
origin = the nickname Git uses for my GitHub repository

https://github.com/Adiotayo/Devop-learning-journey-.git = the GitHub repository link

fetch = where Git downloads/pulls changes from

push = where Git uploads/pushes changes to
```

---

## What is `origin`?

`origin` is the default nickname Git gives to the remote repository when I clone a project from GitHub.

Simple meaning:

```text
origin = nickname for my GitHub repo
```

So instead of typing the full GitHub link every time, Git can use the name `origin`.

---

## Why `git remote -v` is useful

`git remote -v` is useful because it helps me check whether my local project is connected to the correct GitHub repository.

This is important when:

```text
I clone a project
I work on a different laptop
I connect to the wrong GitHub account
I want to check where git push will upload my work
I want to check where git pull will download updates from
```

---

## Fetch vs push

When I see:

```text
(fetch)
```

It means:

```text
This is where Git pulls/downloads changes from.
```

When I see:

```text
(push)
```

It means:

```text
This is where Git pushes/uploads my commits to.
```

---

## My understanding

`git remote -v` helps me confirm the GitHub connection for my local project.

If the remote link is correct, then `git push` will upload to the right GitHub repository and `git pull` will download from the right GitHub repository.
---

# 3. Git clone practice

## What is `git clone`?

`git clone` copies a full GitHub repository onto my computer for the first time.

Simple meaning:

```text
git clone = download/copy a GitHub project onto this computer
```

---

## When do I use `git clone`?

I use `git clone` when the project is not already on the computer.

Examples:

```text
new laptop
different PC
fresh setup
I want to copy someone else's GitHub project
```

If the project is already on my computer, I do not need to clone again. I use:

```bash
git pull
```

---

## Terminal command

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
```

## What the syntax means

```text
git = use Git

clone = copy a repository for the first time

https://github.com/Adiotayo/Devop-learning-journey-.git = the GitHub repository link
```

Simple meaning:

```text
Use Git to copy this GitHub repository onto my computer.
```

---

## Why the command still starts with `git`

The command starts with `git` because Git is the tool doing the cloning.

It does not matter whether I am using:

```text
Mac terminal
Linux terminal
Windows terminal
VS Code terminal
```

The command is still:

```bash
git clone repository-link
```

Simple meaning:

```text
The operating system gives me the terminal.
Git does the clone, pull, push, and commit work.
```

---

## Clone vs pull

```text
git clone = first-time copy from GitHub to my computer

git pull = update a project that already exists on my computer
```

Example:

```text
New computer with no project yet = git clone

Same computer with project already there = git pull
```

---

## Safe clone practice

I should not clone a repository inside the same repository folder.

Wrong idea:

```text
Devop-learning-journey- inside Devop-learning-journey-
```

This can create confusion.

A safer place to practise clone is my home folder:

```bash
cd ~
```

Then clone from there:

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
```

---

## Enter the cloned folder

After cloning, I can enter the new project folder:

```bash
cd Devop-learning-journey-
```

What the syntax means:

```text
cd = change directory

Devop-learning-journey- = the cloned project folder
```

Simple meaning:

```text
Go inside the project I just cloned.
```

---

## Open the cloned project in VS Code

```bash
code .
```

What the syntax means:

```text
code = open in VS Code

. = current folder
```

Simple meaning:

```text
Open the current project folder in VS Code.
```

---

## Clone workflow on a new computer

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
cd Devop-learning-journey-
code .
git status
git pull
```

What each command does:

```text
git clone repository-link
Copies the project from GitHub to the computer.

cd Devop-learning-journey-
Enters the cloned project folder.

code .
Opens the whole project folder in VS Code.

git status
Checks the current Git state.

git pull
Checks for and downloads the latest GitHub updates.
```

---

## My understanding

`git clone` is used when I want to copy a GitHub repository onto a computer for the first time.

After cloning, I enter the folder with `cd`, open it with `code .`, and continue working normally with Git commands.

I should remember:

```text
Clone once.
Pull regularly.
Push after committing work.
```
---

# 3. Git clone practice

## What is `git clone`?

`git clone` copies a full GitHub repository onto my computer for the first time.

Simple meaning:

```text
git clone = download/copy a GitHub project onto this computer
```

---

## When do I use `git clone`?

I use `git clone` when the project is not already on the computer.

Examples:

```text
new laptop
different PC
fresh setup
I want to copy someone else's GitHub project
```

If the project is already on my computer, I do not need to clone again. I use:

```bash
git pull
```

---

## Terminal command

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
```

## What the syntax means

```text
git = use Git

clone = copy a repository for the first time

https://github.com/Adiotayo/Devop-learning-journey-.git = the GitHub repository link
```

Simple meaning:

```text
Use Git to copy this GitHub repository onto my computer.
```

---

## Why the command still starts with `git`

The command starts with `git` because Git is the tool doing the cloning.

It does not matter whether I am using:

```text
Mac terminal
Linux terminal
Windows terminal
VS Code terminal
```

The command is still:

```bash
git clone repository-link
```

Simple meaning:

```text
The operating system gives me the terminal.
Git does the clone, pull, push, and commit work.
```

---

## Clone vs pull

```text
git clone = first-time copy from GitHub to my computer

git pull = update a project that already exists on my computer
```

Example:

```text
New computer with no project yet = git clone

Same computer with project already there = git pull
```

---

## Safe clone practice

I should not clone a repository inside the same repository folder.

Wrong idea:

```text
Devop-learning-journey- inside Devop-learning-journey-
```

This can create confusion.

A safer place to practise clone is my home folder:

```bash
cd ~
```

Then clone from there:

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
```

---

## Enter the cloned folder

After cloning, I can enter the new project folder:

```bash
cd Devop-learning-journey-
```

What the syntax means:

```text
cd = change directory

Devop-learning-journey- = the cloned project folder
```

Simple meaning:

```text
Go inside the project I just cloned.
```

---

## Open the cloned project in VS Code

```bash
code .
```

What the syntax means:

```text
code = open in VS Code

. = current folder
```

Simple meaning:

```text
Open the current project folder in VS Code.
```

---

## Clone workflow on a new computer

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
cd Devop-learning-journey-
code .
git status
git pull
```

What each command does:

```text
git clone repository-link
Copies the project from GitHub to the computer.

cd Devop-learning-journey-
Enters the cloned project folder.

code .
Opens the whole project folder in VS Code.

git status
Checks the current Git state.

git pull
Checks for and downloads the latest GitHub updates.
```

---

## My understanding

`git clone` is used when I want to copy a GitHub repository onto a computer for the first time.

After cloning, I enter the folder with `cd`, open it with `code .`, and continue working normally with Git commands.

I should remember:

```text
Clone once.
Pull regularly.
Push after committing work.
```
