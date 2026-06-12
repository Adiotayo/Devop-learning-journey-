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
