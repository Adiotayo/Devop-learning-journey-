# DevOps Learning Recap

## My current learning stage

I am currently building my foundation in Linux, terminal usage, Git, GitHub, Markdown, and basic scripting.

The goal is not to rush into advanced tools yet. The goal is to understand the basics properly so I can use them confidently later in DevOps, cloud, automation, and infrastructure work.

---

## 1. Terminal basics

The terminal is where I type commands for the computer to run.

Examples of terminal commands:

```bash
pwd
ls
cd
mkdir
touch
git status
git add .
git commit -m "message"
git push
```

Simple meaning:

```text
Terminal = where I type commands
```

---

## 2. VS Code editor

VS Code is where I open files and write inside them.

The command:

```bash
code file-name.md
```

means:

```text
Open this file in VS Code so I can edit it.
```

Example:

```bash
code linux-notes/day-1-linux-basics.md
```

This opens the file `day-1-linux-basics.md` inside VS Code.

Simple meaning:

```text
code = open file in VS Code
```

---

## 3. Markdown files

A Markdown file usually ends with:

```text
.md
```

Markdown is used for writing clean notes with headings, bullet points, and code examples.

Examples:

```markdown
# Main Heading

## Section Heading

### Smaller Heading
```

Simple meaning:

```text
.md = Markdown notes file
```

---

## 4. Linux commands I have learned

### pwd

```bash
pwd
```

Shows the folder I am currently inside.

Simple meaning:

```text
pwd = where am I?
```

### ls

```bash
ls
```

Lists the files and folders in my current location.

Simple meaning:

```text
ls = what is inside this folder?
```

### cd

```bash
cd folder-name
```

Moves into a folder.

Simple meaning:

```text
cd = enter a folder
```

### cd ..

```bash
cd ..
```

Moves back one folder level.

Simple meaning:

```text
cd .. = go back one folder
```

### mkdir

```bash
mkdir folder-name
```

Creates a new folder.

Simple meaning:

```text
mkdir = make folder
```

### touch

```bash
touch file-name
```

Creates a new empty file.

Simple meaning:

```text
touch = create file
```

### rm

```bash
rm file-name
```

Deletes a file.

Simple meaning:

```text
rm = remove file
```

### rmdir

```bash
rmdir folder-name
```

Deletes an empty folder.

Simple meaning:

```text
rmdir = remove empty folder
```

### rm -r

```bash
rm -r folder-name
```

Deletes a folder and everything inside it.

Simple meaning:

```text
rm -r = remove folder recursively
```

### cp

```bash
cp original-file copied-file
```

Copies a file.

Simple meaning:

```text
cp = copy
```

### mv

```bash
mv old-name new-name
```

Renames a file.

```bash
mv file-name folder-name/
```

Moves a file into a folder.

Simple meaning:

```text
mv = move or rename
```

### grep

```bash
grep "word" file-name
```

Searches for text inside a file.

Simple meaning:

```text
grep = search inside file
```

### head

```bash
head file-name
```

Shows the first lines of a file.

Simple meaning:

```text
head = show beginning of file
```

### tail

```bash
tail file-name
```

Shows the last lines of a file.

Simple meaning:

```text
tail = show end of file
```

### less

```bash
less file-name
```

Opens a file in reading mode.

Press:

```text
q
```

to quit.

Simple meaning:

```text
less = read file page by page
```

### chmod

```bash
chmod +x file-name
```

Gives a file permission to run like a program.

Simple meaning:

```text
chmod +x = make file executable
```

---

## 5. Script basics

A script is a file that contains commands for the computer to run.

Example:

```bash
#!/bin/bash
echo "Hello Tayo, this script is working"
```

The file:

```text
hello.sh
```

is a shell script.

To run it, I first give permission:

```bash
chmod +x hello.sh
```

Then run it:

```bash
./hello.sh
```

Simple meaning:

```text
Script = a file containing commands
```

---

## 6. Git basics

Git helps me track changes in my project.

The normal Git workflow is:

```bash
git status
git add .
git commit -m "message"
git push
```

Simple meaning:

```text
git status = check what changed
git add . = prepare changes
git commit -m "message" = save changes locally
git push = upload changes to GitHub
```

---

## 7. Working area, staging area, commit, and push

### Working area

The working area is my actual project files and folders.

Example:

```text
devops-learning-journey
```

Simple meaning:

```text
Working area = where my files live and change
```

### Staging area

The staging area is where files go after I run:

```bash
git add .
```

Simple meaning:

```text
Staging area = files prepared for commit
```

### Commit

A commit saves staged changes locally on my Mac.

Example:

```bash
git commit -m "Update notes"
```

Simple meaning:

```text
Commit = save locally in Git history
```

### Push

Push uploads committed work to GitHub.

Example:

```bash
git push
```

Simple meaning:

```text
Push = upload local commits to GitHub
```

---

## 8. GitHub

GitHub is the online place where my Git project is stored.

Simple meaning:

```text
Git = local version control
GitHub = online repository hosting
```

If I commit but do not push, the work is saved locally but not uploaded to GitHub.

If I commit and push, the work is saved locally and uploaded online.

---

## 9. Git diff

```bash
git diff
```

Shows what changed before staging.

Simple meaning:

```text
git diff = what changed before git add?
```

```bash
git diff --staged
```

Shows what is ready to be committed.

Simple meaning:

```text
git diff --staged = what am I about to commit?
```

---

## 10. Git log

```bash
git log --oneline
```

Shows my saved commit history in a short format.

Simple meaning:

```text
git log --oneline = show my saved Git history
```

---

## 11. Git restore

```bash
git restore file-name
```

Undo uncommitted changes in a file.

```bash
git restore --staged file-name
```

Remove a file from the staging area after `git add`.

Simple meaning:

```text
git restore = undo file change
git restore --staged = undo git add
```

---

## 12. Git branch

A branch is a separate workspace inside the same project.

Simple meaning:

```text
Branch = separate version of the project
```

Useful commands:

```bash
git branch
git switch -c branch-name
git switch main
git merge branch-name
git branch -d branch-name
```

Simple meaning:

```text
git branch = show branches
git switch -c branch-name = create and enter a branch
git switch main = go back to main
git merge branch-name = bring branch changes into main
git branch -d branch-name = delete branch
```

---

## 13. Git pull

```bash
git pull
```

Brings latest changes from GitHub to my laptop.

Simple meaning:

```text
git pull = download latest changes from GitHub
```

Difference:

```text
git push = send my local commits to GitHub
git pull = bring GitHub updates to my laptop
```

---

## 14. Mistakes I made and what I learned

### Mistake 1: Typing file names as commands

Example:

```bash
README.md
```

This does not work because `README.md` is a file name, not a command.

Correct way to open it:

```bash
code README.md
```

### Mistake 2: Typing folder names as commands

Example:

```bash
excel-files
```

This does not work because `excel-files` is a folder name, not a command.

Correct way to enter it:

```bash
cd excel-files
```

### Mistake 3: Using `git up`

This is wrong:

```bash
git up
```

Correct command:

```bash
git push
```

### Mistake 4: Forgetting the difference between save and commit

Command + S saves the file in VS Code.

Git commit saves the change in Git history.

Git push uploads the commit to GitHub.

---

## 15. My current understanding

I now understand that I need to know where I am, what files exist, what changed, what is staged, what is committed, and what has been pushed to GitHub.

The main workflow I should remember is:

```bash
git status
git add .
git commit -m "message"
git push
```

Before starting work, I can use:

```bash
git pull
```

to update my laptop from GitHub.

---

## 16. What I need to practise more

I need to practise:

```text
moving between folders
creating and opening files
knowing terminal vs editor
reading git status carefully
using git add, commit, and push correctly
understanding staging vs commit
using branches slowly
```

---

## 17. Next step

Before moving to Docker, I should become more comfortable with:

```text
Git cleanup
.gitignore
git clone
git remote -v
Markdown basics
Bash scripting
```

My next major lesson after recap should be:

```text
Git and Terminal Cleanup Lesson
```
# DevOps Learning Recap: Full Beginner Foundation

## Purpose of this recap

This recap is to help me understand the foundation properly before moving to the next stage.

The goal is not just to memorise commands. The goal is to understand:

```text
where I am
what I am typing
what each command does
what Git is tracking
what is saved locally
what is pushed to GitHub
how to avoid common mistakes
```

---

# 1. Terminal, VS Code, Git, and GitHub

## What is the terminal?

The terminal is where I type commands for the computer to run.

Examples of terminal commands:

```bash
pwd
ls
cd
mkdir
touch
git status
git add .
git commit -m "message"
git push
```

Simple meaning:

```text
Terminal = where I give instructions to the computer
```

---

## What is VS Code?

VS Code is the editor where I open files and write inside them.

Example:

```bash
code git-practice/learning-recap.md
```

What this command does:

```text
code = open something in VS Code
git-practice/learning-recap.md = the file I want to open
```

Simple meaning:

```text
VS Code = where I write and edit files
```

---

## What is Git?

Git is a tool that tracks changes in my project.

It helps me save versions of my work.

Simple meaning:

```text
Git = local version control on my computer
```

Git answers questions like:

```text
What changed?
What file was added?
What file was deleted?
What did I save before?
What version am I currently working on?
```

---

## What is GitHub?

GitHub is the online place where my Git project is stored.

Simple meaning:

```text
GitHub = online storage for my Git repository
```

Important difference:

```text
Git = tracks work locally on my laptop
GitHub = stores my repository online
```

---

# 2. Opening my project folder

## Terminal command

```bash
cd ~/Devop-learning-journey-
```

## What the syntax means

```text
cd = change directory
~ = my home folder
/ = go inside the next folder
Devop-learning-journey- = the project folder name
```

## Simple meaning

```text
Go into my DevOps learning project folder.
```

## Why this matters

Before I run Git commands or create files, I must make sure I am inside the correct project folder.

If I am in the wrong folder, commands like `touch`, `git status`, or `git add .` may affect the wrong place.

---

# 3. Checking where I am

## Terminal command

```bash
pwd
```

## What the syntax means

```text
pwd = print working directory
```

## Simple meaning

```text
Show me where I currently am in the terminal.
```

## Example output

```text
/Users/tayoadio/Devop-learning-journey-
```

## What this tells me

This tells me I am inside my project folder.

If I see something ending with:

```text
Devop-learning-journey-
```

then I am in the correct place.

---

# 4. Listing files and folders

## Terminal command

```bash
ls
```

## What the syntax means

```text
ls = list
```

## Simple meaning

```text
Show me the files and folders inside my current location.
```

## Example output

```text
README.md
git-practice
linux-notes
python-practice
linux-command-practice
excel-files
```

## What this tells me

It shows me what exists inside my project folder.

---

# 5. Moving into folders

## Terminal command

```bash
cd git-practice
```

## What the syntax means

```text
cd = change directory
git-practice = the folder I want to enter
```

## Simple meaning

```text
Enter the git-practice folder.
```

---

## Go back one folder

```bash
cd ..
```

## What the syntax means

```text
cd = change directory
.. = one level back
```

## Simple meaning

```text
Go back to the previous folder.
```

---

# 6. Creating folders

## Terminal command

```bash
mkdir practice-folder
```

## What the syntax means

```text
mkdir = make directory
practice-folder = name of the new folder
```

## Simple meaning

```text
Create a new folder called practice-folder.
```

## Important note

`mkdir` creates folders, not files.

---

# 7. Creating files

## Terminal command

```bash
touch practice-file.md
```

## What the syntax means

```text
touch = create a new empty file
practice-file.md = name of the file
.md = Markdown file extension
```

## Simple meaning

```text
Create a new empty Markdown file called practice-file.md.
```

## Important note

`touch` creates files, not folders.

---

# 8. Opening files in VS Code

## Terminal command

```bash
code practice-file.md
```

## What the syntax means

```text
code = open in VS Code
practice-file.md = the file I want to open
```

## Simple meaning

```text
Open practice-file.md in VS Code so I can write inside it.
```

## Important note

This command opens the file for editing. It does not run the file.

---

# 9. Markdown basics

Markdown files usually end with:

```text
.md
```

Markdown is used to write clean notes.

## Main heading

```markdown
# Main Heading
```

This creates a big title.

## Section heading

```markdown
## Section Heading
```

This creates a smaller section title.

## Smaller heading

```markdown
### Smaller Heading
```

This creates an even smaller heading.

## Bullet points

```markdown
- First point
- Second point
- Third point
```

This creates a list.

## Code block

````markdown
```bash
git status
```
````

This shows a command clearly in the note.

---

# 10. Saving a file vs saving with Git

## Save in VS Code

```text
Command + S
```

This saves the file content inside VS Code.

## Save in Git

```bash
git add .
git commit -m "message"
```

This saves the change into Git history.

## Upload to GitHub

```bash
git push
```

This uploads the saved Git commit to GitHub.

## Simple difference

```text
Command + S = save file on laptop
git commit = save version in Git history
git push = upload commit to GitHub
```

---

# 11. Checking Git status

## Terminal command

```bash
git status
```

## What the syntax means

```text
git = use Git
status = show current state of the project
```

## Simple meaning

```text
Tell me what Git can see right now.
```

## Git status can show me

```text
new files
modified files
deleted files
staged files
clean project
current branch
whether local branch is up to date with GitHub
```

## Example: clean project

```text
nothing to commit, working tree clean
```

This means:

```text
There are no unsaved Git changes.
```

## Example: modified file

```text
modified: git-practice/learning-recap.md
```

This means:

```text
The file has changed, but the change has not been committed yet.
```

## Example: untracked file

```text
Untracked files:
  new-file.md
```

This means:

```text
Git can see a new file, but Git is not tracking it yet.
```

---

# 12. Git working area, staging area, commit, and push

## Working area

The working area is my actual files and folders.

Example:

```text
Devop-learning-journey-
```

Simple meaning:

```text
Working area = where I edit files
```

When I change a file in VS Code, that change is in the working area.

---

## Staging area

The staging area is where files go after I run:

```bash
git add .
```

Simple meaning:

```text
Staging area = files prepared for commit
```

---

## Commit

A commit saves staged changes into Git history.

Example:

```bash
git commit -m "Add learning recap"
```

Simple meaning:

```text
Commit = save the staged changes locally in Git
```

---

## Push

Push uploads local commits to GitHub.

Example:

```bash
git push
```

Simple meaning:

```text
Push = send my local commits to GitHub
```

---

# 13. Staging files

## Terminal command

```bash
git add .
```

## What the syntax means

```text
git = use Git
add = prepare files for commit
. = everything changed in the current project folder
```

## Simple meaning

```text
Stage all changed files so they are ready to be committed.
```

## Important note

`git add .` does not save to GitHub.

It only prepares files for commit.

---

# 14. Committing changes

## Terminal command

```bash
git commit -m "Add learning recap"
```

## What the syntax means

```text
git = use Git
commit = save staged changes locally
-m = message
"Add learning recap" = the commit message
```

## Simple meaning

```text
Save my staged changes locally with a message explaining what I changed.
```

## Important note

A commit is saved locally on my computer first.

It is not on GitHub until I push.

---

# 15. Pushing changes to GitHub

## Terminal command

```bash
git push
```

## What the syntax means

```text
git = use Git
push = upload commits to GitHub
```

## Simple meaning

```text
Send my local committed work to GitHub.
```

## Important note

If I only commit but do not push, GitHub will not have the latest work.

---

# 16. Pulling changes from GitHub

## Terminal command

```bash
git pull
```

## What the syntax means

```text
git = use Git
pull = bring changes from GitHub to my local computer
```

## Simple meaning

```text
Download the latest changes from GitHub into my local project.
```

## When to use it

Use `git pull` when:

```text
I am starting work
I worked on another computer
someone else changed the repository
I edited something directly on GitHub
```

## Difference between push and pull

```text
git push = laptop to GitHub
git pull = GitHub to laptop
```

---

# 17. Cloning a project

## Terminal command

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
```

## What the syntax means

```text
git = use Git
clone = copy a repository for the first time
https://github.com/Adiotayo/Devop-learning-journey-.git = GitHub repository link
```

## Simple meaning

```text
Copy the full project from GitHub onto this computer for the first time.
```

## When to use clone

Use `git clone` when the project is not already on the computer.

Example:

```text
new laptop
different PC
fresh setup
```

## Clone vs pull

```text
git clone = download the full project for the first time
git pull = update a project that is already on the computer
```

---

# 18. Checking commit history

## Terminal command

```bash
git log --oneline
```

## What the syntax means

```text
git = use Git
log = show commit history
--oneline = show each commit in one short line
```

## Simple meaning

```text
Show my saved Git history in a short format.
```

## Example output

```text
b5308e7 Add git branch lesson
fc62bf Add learning recap
```

## What this tells me

It shows previous commits and their messages.

---

# 19. Checking exact changes before staging

## Terminal command

```bash
git diff
```

## What the syntax means

```text
git = use Git
diff = show differences
```

## Simple meaning

```text
Show what changed before I run git add.
```

## Important note

`git diff` shows changes in the working area that are not staged yet.

---

# 20. Checking staged changes

## Terminal command

```bash
git diff --staged
```

## What the syntax means

```text
git = use Git
diff = show differences
--staged = show changes already staged with git add
```

## Simple meaning

```text
Show what I am about to commit.
```

## When to use it

Use it after:

```bash
git add .
```

but before:

```bash
git commit -m "message"
```

---

# 21. Undoing file changes

## Terminal command

```bash
git restore file-name
```

## Example

```bash
git restore git-practice/learning-recap.md
```

## What the syntax means

```text
git = use Git
restore = put file back to last committed version
git-practice/learning-recap.md = file I want to restore
```

## Simple meaning

```text
Undo uncommitted changes in this file.
```

## Warning

This can delete work that has not been committed.

Use it carefully.

---

# 22. Unstaging a file

## Terminal command

```bash
git restore --staged file-name
```

## Example

```bash
git restore --staged git-practice/learning-recap.md
```

## What the syntax means

```text
git = use Git
restore = restore something
--staged = remove from staging area
file-name = file to unstage
```

## Simple meaning

```text
Remove the file from staging, but keep the actual changes in the file.
```

## Difference between restore and restore staged

```text
git restore file-name = remove uncommitted file changes
git restore --staged file-name = undo git add only
```

---

# 23. Branches

## What is a branch?

A branch is a separate workspace inside the same project.

Simple meaning:

```text
Branch = separate version of the project
```

## Why branches are useful

Branches allow me to test changes safely without disturbing `main`.

Example:

```text
main = stable version
recap-learning = branch for working on recap
```

---

# 24. Checking branches

## Terminal command

```bash
git branch
```

## What the syntax means

```text
git = use Git
branch = show branches
```

## Simple meaning

```text
Show all local branches.
```

## Example output

```text
* main
  recap-learning
```

## What the star means

```text
* = the branch I am currently on
```

---

# 25. Creating and switching to a branch

## Terminal command

```bash
git switch -c recap-learning
```

## What the syntax means

```text
git = use Git
switch = move to another branch
-c = create a new branch
recap-learning = name of the new branch
```

## Simple meaning

```text
Create a branch called recap-learning and move into it.
```

---

# 26. Switching back to main

## Terminal command

```bash
git switch main
```

## What the syntax means

```text
git = use Git
switch = move to another branch
main = the branch I want to move into
```

## Simple meaning

```text
Go back to the main branch.
```

---

# 27. Merging a branch

## Terminal command

```bash
git merge recap-learning
```

## What the syntax means

```text
git = use Git
merge = bring changes from another branch into my current branch
recap-learning = the branch I want to merge
```

## Simple meaning

```text
Bring the work from recap-learning into the branch I am currently on.
```

## Important note

Usually, I switch to `main` first:

```bash
git switch main
```

Then merge:

```bash
git merge recap-learning
```

This means:

```text
Bring recap-learning into main.
```

---

# 28. Deleting a branch

## Terminal command

```bash
git branch -d recap-learning
```

## What the syntax means

```text
git = use Git
branch = work with branches
-d = delete safely
recap-learning = branch I want to delete
```

## Simple meaning

```text
Delete the recap-learning branch after it has been merged.
```

## Important note

This only deletes the local branch.

It does not delete the committed work if the branch was already merged into main.

---

# 29. A full branch workflow

## Terminal commands

```bash
cd ~/Devop-learning-journey-
git status
git switch -c recap-learning
code git-practice/learning-recap.md
git status
git add .
git status
git commit -m "Add learning recap"
git switch main
git merge recap-learning
git push
git branch -d recap-learning
```

## What each command does

```text
cd ~/Devop-learning-journey-
Go into my project folder.

git status
Check the state of my project before starting.

git switch -c recap-learning
Create and enter a new branch.

code git-practice/learning-recap.md
Open the recap file in VS Code.

git status
Check what changed after editing.

git add .
Stage all changed files.

git status
Confirm the correct file is staged.

git commit -m "Add learning recap"
Save the staged work locally in Git history.

git switch main
Go back to the main branch.

git merge recap-learning
Bring the recap work into main.

git push
Upload main to GitHub.

git branch -d recap-learning
Delete the branch after merging.
```

---

# 30. Reading files from the terminal

## grep

```bash
grep "Git" git-practice/learning-recap.md
```

What it means:

```text
grep = search inside a file
"Git" = the word I am searching for
git-practice/learning-recap.md = the file I am searching inside
```

Simple meaning:

```text
Find lines that contain the word Git.
```

---

## head

```bash
head git-practice/learning-recap.md
```

What it means:

```text
head = show the first lines of a file
git-practice/learning-recap.md = the file I want to read
```

Simple meaning:

```text
Show the beginning of the recap file.
```

---

## tail

```bash
tail git-practice/learning-recap.md
```

What it means:

```text
tail = show the last lines of a file
git-practice/learning-recap.md = the file I want to read
```

Simple meaning:

```text
Show the end of the recap file.
```

---

## less

```bash
less git-practice/learning-recap.md
```

What it means:

```text
less = open file for reading page by page
git-practice/learning-recap.md = the file I want to read
```

Simple meaning:

```text
Read the file in the terminal.
```

To quit `less`, press:

```text
q
```

---

# 31. File and folder mistakes to avoid

## Mistake: typing a file name as a command

Wrong:

```bash
README.md
```

Why it is wrong:

```text
README.md is a file, not a command.
```

Correct:

```bash
code README.md
```

Meaning:

```text
Open README.md in VS Code.
```

---

## Mistake: typing a folder name as a command

Wrong:

```bash
git-practice
```

Why it is wrong:

```text
git-practice is a folder, not a command.
```

Correct:

```bash
cd git-practice
```

Meaning:

```text
Enter the git-practice folder.
```

---

## Mistake: using git up

Wrong:

```bash
git up
```

Why it is wrong:

```text
git up is not the command for uploading work.
```

Correct:

```bash
git push
```

Meaning:

```text
Upload committed work to GitHub.
```

---

# 32. Daily beginner workflow

## Before starting work

```bash
cd ~/Devop-learning-journey-
git status
git pull
```

Meaning:

```text
cd ~/Devop-learning-journey-
Go into the project folder.

git status
Check the current state.

git pull
Bring latest updates from GitHub.
```

---

## While working

```bash
code git-practice/learning-recap.md
```

Meaning:

```text
Open the file and edit it in VS Code.
```

Then save with:

```text
Command + S
```

Meaning:

```text
Save the file locally in VS Code.
```

---

## After working

```bash
git status
git add .
git status
git commit -m "Update learning recap"
git push
```

Meaning:

```text
git status
Check what changed.

git add .
Stage the changed files.

git status
Confirm the correct files are staged.

git commit -m "Update learning recap"
Save the staged work locally.

git push
Upload the commit to GitHub.
```

---

# 33. My current understanding

I understand that the terminal, VS Code, Git, and GitHub do different jobs.

```text
Terminal = where I type commands
VS Code = where I edit files
Git = tracks versions locally
GitHub = stores the project online
```

I understand that:

```text
cd moves me into folders
touch creates files
mkdir creates folders
code opens files in VS Code
git status checks Git state
git add stages changes
git commit saves changes locally
git push uploads to GitHub
git pull downloads from GitHub
git clone copies a repo for the first time
git branch shows branches
git switch moves between branches
git merge brings branch work together
```

---

# 34. What I need to practise more

I need to keep practising:

```text
checking where I am with pwd
opening the correct project folder
knowing terminal vs VS Code
reading git status carefully
using git add and git commit correctly
understanding local commit vs GitHub push
using branches slowly
knowing when to clone and when to pull
```

---

# 35. Next lesson after recap

After this recap, the next lesson should be:

```text
Git and Terminal Cleanup Lesson
```

That lesson should cover:

```text
.gitignore
git remote -v
git clone practice
Markdown formatting
terminal shortcuts
```

After that, I can move into:

```text
Bash Scripting Basics
```
