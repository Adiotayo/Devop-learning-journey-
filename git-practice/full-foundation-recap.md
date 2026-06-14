# Full Foundation Recap: Terminal, Linux, Git, GitHub, Markdown, and Cleanup

## Purpose of this recap

This recap brings together everything I have learned so far before moving into Bash scripting.

The goal is not just to memorise commands. The goal is to understand:

```text
where I am
what I am typing
what each command does
which tool is being used
what Git is tracking
what is saved locally
what is uploaded to GitHub
how to avoid common mistakes
```

---

# 1. The main tools I am using

## Terminal

The terminal is where I type commands.

Examples:

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

## VS Code

VS Code is where I open files and write inside them.

Example:

```bash
code git-practice/full-foundation-recap.md
```

What the syntax means:

```text
code = open in VS Code
git-practice/full-foundation-recap.md = the file I want to open
```

Simple meaning:

```text
VS Code = where I edit files and write notes
```

Important difference:

```text
Terminal = where I type commands
VS Code editor = where I write inside files
```

---

## Git

Git is a tool that tracks changes in my project.

Simple meaning:

```text
Git = local version control
```

Git helps me know:

```text
what changed
what file was added
what file was deleted
what has been saved in history
what has not been committed yet
```

---

## GitHub

GitHub is the online place where my Git project is stored.

Simple meaning:

```text
GitHub = online home for my repository
```

Important difference:

```text
Git = tracks changes locally on my laptop
GitHub = stores the project online
```

---

# 2. My main project folder

My main project folder is:

```bash
~/Devop-learning-journey-
```

To enter it, I use:

```bash
cd ~/Devop-learning-journey-
```

What the syntax means:

```text
cd = change directory
~ = home folder
/ = go inside the next folder
Devop-learning-journey- = my project folder
```

Simple meaning:

```text
Go into my DevOps learning project folder.
```

Why this matters:

```text
Before I create files, edit notes, or use Git, I should make sure I am inside the correct project folder.
```

---

# 3. Checking where I am

## Command

```bash
pwd
```

What the syntax means:

```text
pwd = print working directory
```

Simple meaning:

```text
Show me the folder I am currently inside.
```

Example output:

```text
/Users/tayoadio/Devop-learning-journey-
```

This means I am inside my project folder.

If I see:

```text
/Users/tayoadio
```

I am in my home folder, not inside the project yet.

---

# 4. Listing files and folders

## Command

```bash
ls
```

What the syntax means:

```text
ls = list
```

Simple meaning:

```text
Show me what is inside the current folder.
```

Example output:

```text
README.md
git-practice
linux-notes
python-practice
linux-command-practice
excel-files
```

---

## Detailed list

```bash
ls -la
```

What the syntax means:

```text
ls = list
-l = long format with more details
-a = show all files, including hidden files
```

Simple meaning:

```text
Show all files and folders with details.
```

This is useful because files like `.gitignore` may be hidden-style files.

---

# 5. Moving between folders

## Enter a folder

```bash
cd git-practice
```

What the syntax means:

```text
cd = change directory
git-practice = folder I want to enter
```

Simple meaning:

```text
Go inside the git-practice folder.
```

---

## Go back one level

```bash
cd ..
```

What the syntax means:

```text
cd = change directory
.. = one folder level back
```

Simple meaning:

```text
Move back to the parent folder.
```

---

## Go home

```bash
cd ~
```

What the syntax means:

```text
cd = change directory
~ = home folder
```

Simple meaning:

```text
Go back to my home folder.
```

---

# 6. Creating folders and files

## Create a folder

```bash
mkdir practice-folder
```

What the syntax means:

```text
mkdir = make directory
practice-folder = name of the folder
```

Simple meaning:

```text
Create a new folder called practice-folder.
```

Important:

```text
mkdir creates folders, not files.
```

---

## Create a file

```bash
touch practice-file.md
```

What the syntax means:

```text
touch = create a new empty file
practice-file.md = file name
.md = Markdown file extension
```

Simple meaning:

```text
Create a new empty Markdown file.
```

Important:

```text
touch creates files, not folders.
```

---

# 7. Opening files in VS Code

## Open one file

```bash
code practice-file.md
```

What the syntax means:

```text
code = open in VS Code
practice-file.md = file I want to open
```

Simple meaning:

```text
Open the file in VS Code so I can write inside it.
```

---

## Open the current folder in VS Code

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
Open the whole current folder in VS Code.
```

This is useful after cloning a project.

---

# 8. Deleting files and folders

## Delete a file

```bash
rm file-name
```

What the syntax means:

```text
rm = remove
file-name = file I want to delete
```

Simple meaning:

```text
Delete this file.
```

---

## Delete an empty folder

```bash
rmdir folder-name
```

What the syntax means:

```text
rmdir = remove directory
folder-name = empty folder I want to delete
```

Simple meaning:

```text
Delete an empty folder.
```

---

## Delete a folder and everything inside it

```bash
rm -r folder-name
```

What the syntax means:

```text
rm = remove
-r = recursive, meaning include everything inside the folder
folder-name = folder to delete
```

Simple meaning:

```text
Delete the folder and its contents.
```

---

## Force-delete folders

```bash
rm -rf clone-practice-repo clone-practice-repo-2
```

What the syntax means:

```text
rm = remove
-r = recursively delete folders and contents
-f = force, do not ask for confirmation
clone-practice-repo clone-practice-repo-2 = folders to delete
```

Simple meaning:

```text
Delete both practice clone folders completely.
```

Warning:

```text
rm -rf is powerful. Use it carefully.
```

---

# 9. Copying and moving files

## Copy a file

```bash
cp original-file copied-file
```

What the syntax means:

```text
cp = copy
original-file = file I want to copy
copied-file = new copied file name
```

Simple meaning:

```text
Make a copy of a file.
```

---

## Rename a file

```bash
mv old-name new-name
```

What the syntax means:

```text
mv = move or rename
old-name = current file name
new-name = new file name
```

Simple meaning:

```text
Rename the file.
```

---

## Move a file into a folder

```bash
mv file-name folder-name/
```

What the syntax means:

```text
mv = move
file-name = file I want to move
folder-name/ = destination folder
```

Simple meaning:

```text
Move this file into that folder.
```

---

# 10. Reading files in the terminal

## head

```bash
head learning-recap.md
```

What the syntax means:

```text
head = show the first lines of a file
learning-recap.md = file I want to read
```

Simple meaning:

```text
Show the beginning of the file.
```

---

## tail

```bash
tail learning-recap.md
```

What the syntax means:

```text
tail = show the last lines of a file
learning-recap.md = file I want to read
```

Simple meaning:

```text
Show the end of the file.
```

---

## less

```bash
less learning-recap.md
```

What the syntax means:

```text
less = open file for reading page by page
learning-recap.md = file I want to read
```

Simple meaning:

```text
Read the file inside the terminal.
```

To quit:

```text
q
```

---

## grep

```bash
grep "Git" learning-recap.md
```

What the syntax means:

```text
grep = search inside a file
"Git" = word I am searching for
learning-recap.md = file I am searching inside
```

Simple meaning:

```text
Find lines containing the word Git.
```

`grep` is similar to `Command + F`, but inside the terminal.

---

## Count lines containing a word

```bash
grep -c "Git" learning-recap.md
```

What the syntax means:

```text
grep = search
-c = count matching lines
"Git" = word I am searching for
learning-recap.md = file I am searching inside
```

Simple meaning:

```text
Count how many lines contain the word Git.
```

---

# 11. Understanding file paths

A file path tells the terminal where a file is.

Example:

```bash
git-practice/learning-recap.md
```

What it means:

```text
git-practice = folder
/ = inside
learning-recap.md = file
```

Simple meaning:

```text
The file learning-recap.md is inside the git-practice folder.
```

Important rule:

```text
If I am inside the main project folder, I can use:
git-practice/learning-recap.md

If I am already inside git-practice, I should use:
learning-recap.md
```

Example:

```bash
cd ~/Devop-learning-journey-
less git-practice/learning-recap.md
```

But if I am already inside `git-practice`:

```bash
less learning-recap.md
```

---

# 12. Markdown basics

Markdown files usually end with:

```text
.md
```

Markdown is used for clean notes.

---

## Headings

```markdown
# Main Heading
## Section Heading
### Smaller Heading
```

Meaning:

```text
# = biggest heading
## = second-level heading
### = third-level heading
```

---

## Bullet points

```markdown
- First point
- Second point
- Third point
```

Simple meaning:

```text
Use bullet points when listing items.
```

---

## Numbered list

```markdown
1. First step
2. Second step
3. Third step
```

Simple meaning:

```text
Use numbered lists when order matters.
```

---

## Inline code

```markdown
Use `git status` to check the project.
```

Simple meaning:

```text
Use backticks when mentioning commands or file names inside a sentence.
```

---

## Code block

````markdown
```bash
git status
git add .
git commit -m "message"
git push
```
````

Simple meaning:

```text
Use code blocks for terminal commands.
```

---

## Text block

````markdown
```text
nothing to commit, working tree clean
```
````

Simple meaning:

```text
Use text blocks for explanations or expected output.
```

---

## Bold text

```markdown
**Important point**
```

Simple meaning:

```text
Use bold text to highlight important information.
```

---

## Horizontal line

```markdown
---
```

Simple meaning:

```text
Use this to separate sections.
```

---

# 13. Saving in VS Code vs saving in Git

## Save in VS Code

```text
Command + S
```

Simple meaning:

```text
Save the file content on my laptop.
```

---

## Save in Git history

```bash
git add .
git commit -m "message"
```

Simple meaning:

```text
Stage the changes, then save them in Git history.
```

---

## Upload to GitHub

```bash
git push
```

Simple meaning:

```text
Upload committed work to GitHub.
```

Important difference:

```text
Command + S = save file content locally
git commit = save a version in Git locally
git push = upload commits to GitHub
```

---

# 14. Git status

## Command

```bash
git status
```

What the syntax means:

```text
git = use Git
status = show current project state
```

Simple meaning:

```text
Tell me what Git sees right now.
```

Git status can show:

```text
current branch
modified files
new files
deleted files
staged files
untracked files
whether branch is up to date with origin/main
```

---

## Clean status

```text
nothing to commit, working tree clean
```

Meaning:

```text
There are no uncommitted changes.
```

---

## Modified file

```text
modified: git-practice/git-terminal-cleanup-lesson.md
```

Meaning:

```text
This file has changed since the last commit.
```

---

## Untracked file

```text
Untracked files:
  .gitignore
```

Meaning:

```text
Git sees a new file but is not tracking it yet.
```

---

## Staged file

```text
Changes to be committed:
  modified: git-practice/git-terminal-cleanup-lesson.md
```

Meaning:

```text
This file is ready to be committed.
```

---

# 15. Git working area, staging area, commit, and push

## Working area

The working area is the actual project folder where I edit files.

Simple meaning:

```text
Working area = where my files live and change
```

---

## Staging area

The staging area is where files go after:

```bash
git add .
```

Simple meaning:

```text
Staging area = prepared changes waiting to be committed
```

---

## Commit

A commit saves staged changes into Git history.

```bash
git commit -m "Update notes"
```

Simple meaning:

```text
Commit = save staged changes locally in Git history
```

---

## Push

Push uploads commits to GitHub.

```bash
git push
```

Simple meaning:

```text
Push = upload committed work to GitHub
```

---

# 16. Normal Git workflow

## Full workflow

```bash
git status
git add .
git status
git commit -m "Update notes"
git push
git status
```

What each command does:

```text
git status
Check what changed.

git add .
Stage all changed files.

git status
Confirm the correct files are staged.

git commit -m "Update notes"
Save staged changes locally in Git.

git push
Upload the commit to GitHub.

git status
Confirm everything is clean.
```

---

# 17. git add

## Stage everything

```bash
git add .
```

What the syntax means:

```text
git = use Git
add = stage files
. = everything changed in the current project
```

Simple meaning:

```text
Prepare all changed files for commit.
```

---

## Stage one file

```bash
git add git-practice/git-terminal-cleanup-lesson.md
```

What the syntax means:

```text
git add = stage a file
git-practice/git-terminal-cleanup-lesson.md = specific file to stage
```

Simple meaning:

```text
Prepare only this file for commit.
```

---

# 18. git commit

## Command

```bash
git commit -m "Add Markdown formatting lesson"
```

What the syntax means:

```text
git = use Git
commit = save staged changes locally
-m = message
"Add Markdown formatting lesson" = commit message
```

Simple meaning:

```text
Save the staged changes locally with a clear message.
```

Important:

```text
-m belongs to git commit, not git add.
```

Wrong:

```bash
git add . -m "Update notes"
```

Correct:

```bash
git add .
git commit -m "Update notes"
```

---

# 19. git push

## Command

```bash
git push
```

What the syntax means:

```text
git = use Git
push = upload commits to GitHub
```

Simple meaning:

```text
Send my local committed work to GitHub.
```

If Git says:

```text
Everything up-to-date
```

It means:

```text
GitHub already has the latest committed work.
```

---

# 20. git pull

## Command

```bash
git pull
```

What the syntax means:

```text
git = use Git
pull = bring changes from GitHub to my local computer
```

Simple meaning:

```text
Download the latest GitHub changes into my local project.
```

Use it when:

```text
starting work
using another computer
someone else updated the repo
I edited something directly on GitHub
```

Difference:

```text
git push = laptop to GitHub
git pull = GitHub to laptop
```

---

# 21. git log

## Command

```bash
git log --oneline
```

What the syntax means:

```text
git = use Git
log = show commit history
--oneline = show each commit in one short line
```

Simple meaning:

```text
Show my commit history in a short format.
```

If the terminal shows `(END)`, press:

```text
q
```

---

# 22. git diff

## Unstaged changes

```bash
git diff
```

What the syntax means:

```text
git = use Git
diff = show differences
```

Simple meaning:

```text
Show what changed before git add.
```

---

## Staged changes

```bash
git diff --staged
```

What the syntax means:

```text
git = use Git
diff = show differences
--staged = show staged changes
```

Simple meaning:

```text
Show what I am about to commit.
```

---

# 23. git restore

## Undo uncommitted file changes

```bash
git restore file-name
```

Example:

```bash
git restore git-practice/learning-recap.md
```

What the syntax means:

```text
git = use Git
restore = restore file to last committed version
file-name = file I want to restore
```

Simple meaning:

```text
Undo uncommitted changes in this file.
```

Warning:

```text
This can delete unsaved work that has not been committed.
```

---

## Unstage a file

```bash
git restore --staged file-name
```

Example:

```bash
git restore --staged git-practice/learning-recap.md
```

What the syntax means:

```text
git = use Git
restore = restore something
--staged = remove from staging area
file-name = file to unstage
```

Simple meaning:

```text
Undo git add, but keep the actual file changes.
```

Difference:

```text
git restore file-name = remove file changes
git restore --staged file-name = undo git add only
```

---

# 24. Git branches

## What is a branch?

A branch is a separate workspace inside the same project.

Simple meaning:

```text
Branch = separate version of the project
```

Why branches are useful:

```text
They let me test or work on changes without disturbing main.
```

---

## Show branches

```bash
git branch
```

Simple meaning:

```text
Show all local branches.
```

The star shows the current branch:

```text
* main
```

---

## Create and switch to a branch

```bash
git switch -c recap-learning
```

What the syntax means:

```text
git = use Git
switch = move to another branch
-c = create new branch
recap-learning = branch name
```

Simple meaning:

```text
Create a branch and move into it.
```

---

## Switch back to main

```bash
git switch main
```

Simple meaning:

```text
Go back to the main branch.
```

---

## Merge branch into main

```bash
git merge recap-learning
```

Simple meaning:

```text
Bring changes from recap-learning into the current branch.
```

Usually:

```bash
git switch main
git merge recap-learning
```

Meaning:

```text
Go to main, then bring the branch work into main.
```

---

## Delete branch

```bash
git branch -d recap-learning
```

What the syntax means:

```text
git branch = work with branches
-d = delete safely
recap-learning = branch to delete
```

Simple meaning:

```text
Delete the branch after merging.
```

---

# 25. git remote -v

## Command

```bash
git remote -v
```

What the syntax means:

```text
git = use Git
remote = show/manage remote repository connections
-v = verbose, show details
```

Simple meaning:

```text
Show the GitHub repository connected to this local project.
```

Example output:

```text
origin  https://github.com/Adiotayo/Devop-learning-journey-.git (fetch)
origin  https://github.com/Adiotayo/Devop-learning-journey-.git (push)
```

Meaning:

```text
origin = nickname for the GitHub repo
fetch = where git pull downloads from
push = where git push uploads to
```

---

# 26. git clone

## Command

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git
```

What the syntax means:

```text
git = use Git
clone = copy a repository for the first time
https://github.com/Adiotayo/Devop-learning-journey-.git = GitHub repository link
```

Simple meaning:

```text
Copy the GitHub project onto this computer.
```

Use clone when:

```text
new laptop
different PC
fresh setup
project is not already on the computer
```

---

## Clone into a specific folder

```bash
git clone https://github.com/Adiotayo/Devop-learning-journey-.git clone-practice-repo
```

What the syntax means:

```text
git = use Git
clone = copy repository
GitHub link = repository to copy
clone-practice-repo = new folder name
```

Simple meaning:

```text
Clone the GitHub project into a folder called clone-practice-repo.
```

---

## Clone vs pull

```text
git clone = first-time copy from GitHub
git pull = update a project that is already on the computer
```

Simple rule:

```text
Clone once.
Pull regularly.
Push after committing.
```

---

# 27. .gitignore

## What is `.gitignore`?

`.gitignore` tells Git what files or folders not to track.

Simple meaning:

```text
.gitignore = do not track these files
```

---

## Create `.gitignore`

```bash
touch .gitignore
```

What the syntax means:

```text
touch = create file
.gitignore = file name
```

Simple meaning:

```text
Create a .gitignore file.
```

---

## Open `.gitignore`

```bash
code .gitignore
```

Simple meaning:

```text
Open .gitignore in VS Code.
```

---

## Correct `.gitignore` content

```text
.DS_Store
.env
__pycache__/
node_modules/
*.log
```

Meaning:

```text
.DS_Store = ignore Mac system file
.env = ignore secret environment file
__pycache__/ = ignore Python cache folder
node_modules/ = ignore Node.js dependency folder
*.log = ignore all files ending in .log
```

Important:

```text
Explanations should not go inside .gitignore.
Only ignore rules should go inside .gitignore.
```

Explanations belong inside Markdown notes.

---

# 28. Terminal shortcuts

## Clear screen

```bash
clear
```

Simple meaning:

```text
Clear the terminal view.
```

This does not delete files.

---

## Up Arrow

```text
Up Arrow
```

Simple meaning:

```text
Bring back the previous command.
```

---

## Down Arrow

```text
Down Arrow
```

Simple meaning:

```text
Move forward through command history.
```

---

## Tab

```text
Tab
```

Simple meaning:

```text
Autocomplete file or folder names.
```

Useful for avoiding spelling mistakes.

---

## Control + C

```text
Control + C
```

Simple meaning:

```text
Cancel a running command.
```

This is not the same as copy on Mac.

---

## Control + L

```text
Control + L
```

Simple meaning:

```text
Clear the terminal screen.
```

Similar to:

```bash
clear
```

---

## q

```text
q
```

Simple meaning:

```text
Quit less or git log reading mode.
```

---

## Command + S

```text
Command + S
```

Simple meaning:

```text
Save file in VS Code.
```

This is not the same as Git commit.

---

## Command + `

```text
Command + `
```

Simple meaning:

```text
Show or hide the terminal in VS Code.
```

---

# 29. Common mistakes and corrections

## Mistake 1: Typing a file name as a command

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

---

## Mistake 2: Typing a folder name as a command

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

---

## Mistake 3: Using git up

Wrong:

```bash
git up
```

Correct:

```bash
git push
```

---

## Mistake 4: Putting commit message on git add

Wrong:

```bash
git add . -m "Update notes"
```

Correct:

```bash
git add .
git commit -m "Update notes"
```

---

## Mistake 5: Running Git commands in the wrong folder

Example mistake:

```text
Running git status inside /Users/tayoadio
```

This may show:

```text
fatal: not a git repository
```

Correct:

```bash
cd ~/Devop-learning-journey-
git status
```

---

## Mistake 6: Using the wrong path

If I am inside `git-practice`, this may be wrong:

```bash
less git-practice/learning-recap.md
```

Because Git will look for:

```text
git-practice/git-practice/learning-recap.md
```

Correct if I am already inside `git-practice`:

```bash
less learning-recap.md
```

Correct if I am inside the main project folder:

```bash
less git-practice/learning-recap.md
```

---

# 30. Daily workflow

## Before starting work

```bash
cd ~/Devop-learning-journey-
git status
git pull
```

Meaning:

```text
Go into the project.
Check project state.
Download latest changes from GitHub.
```

---

## While working

```bash
code git-practice/file-name.md
```

Then save with:

```text
Command + S
```

Meaning:

```text
Open the file.
Write notes.
Save the file.
```

---

## After working

```bash
git status
git add .
git status
git commit -m "Update notes"
git push
git status
```

Meaning:

```text
Check changes.
Stage changes.
Confirm staged files.
Commit locally.
Push to GitHub.
Confirm clean status.
```

---

# 31. What I have learned so far

I have learned the foundation of:

```text
terminal usage
file and folder movement
creating files and folders
reading files in terminal
Markdown notes
Git workflow
GitHub upload/download
branches and merge
restore and unstage
.gitignore
remote connection
clone practice
terminal shortcuts
```

---

# 32. My current understanding

I understand that:

```text
Terminal = where I type commands
VS Code = where I edit files
Git = tracks versions locally
GitHub = stores my project online
```

I understand that:

```text
cd moves between folders
pwd shows where I am
ls shows what is inside a folder
mkdir creates folders
touch creates files
code opens files
rm deletes files
grep searches files
head shows the start of a file
tail shows the end of a file
less reads files page by page
```

I understand that:

```text
git status checks what Git sees
git add stages changes
git commit saves changes locally
git push uploads commits to GitHub
git pull downloads updates from GitHub
git clone copies a repo for the first time
git remote -v shows the GitHub connection
git branch shows branches
git switch changes branches
git merge brings branch work together
git restore can undo changes
```

---

# 33. What I should practise more

I should keep practising:

```text
checking where I am with pwd
using cd correctly
understanding file paths
reading git status carefully
knowing terminal vs VS Code
saving with Command + S before committing
staging the correct file
committing with a clear message
pushing after committing
knowing when to clone and when to pull
```

---

# 34. Readiness for Bash scripting

I should move to Bash scripting only after I am comfortable with:

```text
terminal commands
file paths
creating and opening files
running commands in the correct folder
chmod +x
./script-name.sh
Git add, commit, and push
```

My next topic should be:

```text
Bash Scripting Basics
```

But I should continue moving slowly and practising each part properly.
