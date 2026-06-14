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
---

# 4. Markdown formatting

## What is Markdown?

Markdown is a simple way to write formatted notes using plain text.

Markdown files usually end with:

```text
.md
```

Simple meaning:

```text
Markdown = a clean way to write notes, headings, lists, and code examples
```

Markdown is useful because it makes my notes easier to read on GitHub.

---

## Headings

Headings help me organise my notes.

### Main heading

```markdown
# Main Heading
```

What the syntax means:

```text
# = biggest heading
Main Heading = the title text
```

Simple meaning:

```text
Use one # for the main title of the page.
```

Example:

```markdown
# Git and Terminal Cleanup Lesson
```

---

### Section heading

```markdown
## Section Heading
```

What the syntax means:

```text
## = second-level heading
Section Heading = the section title
```

Simple meaning:

```text
Use ## for a major section inside the note.
```

Example:

```markdown
## What is Git?
```

---

### Smaller heading

```markdown
### Smaller Heading
```

What the syntax means:

```text
### = third-level heading
Smaller Heading = smaller section title
```

Simple meaning:

```text
Use ### for smaller points under a section.
```

Example:

```markdown
### What the syntax means
```

---

## Bullet points

Bullet points help me list things clearly.

```markdown
- First point
- Second point
- Third point
```

What the syntax means:

```text
- = bullet point symbol
First point = item in the list
```

Simple meaning:

```text
Use bullet points when listing items.
```

Example:

```markdown
- Git tracks changes
- GitHub stores the project online
- VS Code is where I edit files
```

---

## Numbered lists

Numbered lists help me show steps in order.

```markdown
1. First step
2. Second step
3. Third step
```

What the syntax means:

```text
1. = first item
2. = second item
3. = third item
```

Simple meaning:

```text
Use numbered lists when order matters.
```

Example:

```markdown
1. Write the note
2. Save the file
3. Add the file to Git
4. Commit the work
5. Push to GitHub
```

---

## Inline code

Inline code is used when I mention a command or file name inside a sentence.

```markdown
Use `git status` to check the project.
```

What the syntax means:

```text
` ` = backticks around a command or file name
git status = the command I am highlighting
```

Simple meaning:

```text
Use one backtick on each side when writing a command inside a sentence.
```

Example:

```markdown
The command `git push` uploads my commits to GitHub.
```

---

## Code blocks

Code blocks are used when I want to show commands clearly on separate lines.

````markdown
```bash
git status
git add .
git commit -m "message"
git push
````

````

What the syntax means:

```text
``` = start or end of a code block
bash = the type of code or command being shown
git status = command inside the code block
````

Simple meaning:

```text
Use code blocks when writing terminal commands in my notes.
```

Example:

```bash
git status
git add .
git commit -m "Update notes"
git push
```

---

## Text blocks

Text blocks are useful when I want to explain output or simple meaning.

````markdown
```text
This is a simple explanation.
````

````

What the syntax means:

```text
``` = start or end of a code block
text = plain explanation, not a command
````

Simple meaning:

```text
Use text blocks for explanations or expected terminal output.
```

Example:

```text
nothing to commit, working tree clean
```

---

## Bold text

Bold text is used to make important words stand out.

```markdown
**important word**
```

What the syntax means:

```text
** ** = make the text bold
important word = the text I want to highlight
```

Simple meaning:

```text
Use bold text for important points.
```

Example:

```markdown
**Do not clone inside your main project folder.**
```

---

## Horizontal line

A horizontal line separates sections.

```markdown
---
```

What the syntax means:

```text
--- = horizontal divider line
```

Simple meaning:

```text
Use this to separate big sections in my notes.
```

---

## Good Markdown note structure

A clean Markdown lesson can follow this structure:

````markdown
# Lesson Title

## What is it?

Short explanation.

## Terminal command

```bash
command here
````

## What the syntax means

```text
command = meaning
option = meaning
file-name = meaning
```

## Simple meaning

```text
Simple explanation here.
```

## My understanding

My own explanation in simple words.

````

Simple meaning:

```text
A good note has a title, explanation, command, syntax breakdown, simple meaning, and my understanding.
````

---

## Markdown mistakes to avoid

### Mistake 1: Forgetting to close a code block

Wrong:

````markdown
```bash
git status
````

Correct:

````markdown
```bash
git status
````

````

Simple meaning:

```text
Every code block needs an opening and closing set of three backticks.
````

---

### Mistake 2: Writing command explanations inside config files

For example, inside `.gitignore`, I should not write:

```text
*.log = ignore all log files
```

Inside `.gitignore`, I should only write:

```text
*.log
```

The explanation belongs in the Markdown note, not the config file.

---

### Mistake 3: Mixing terminal commands and notes

Terminal command:

```bash
git status
```

Markdown note:

```markdown
`git status` checks what Git can see.
```

Simple meaning:

```text
Commands go in the terminal.
Explanations go in the Markdown note.
```

---

## My understanding

Markdown helps me write clean technical notes.

I can use headings, bullet points, numbered lists, inline code, code blocks, text blocks, bold text, and horizontal lines to make my notes easier to read.

Good Markdown notes will help me explain my learning clearly on GitHub.
---

# 5. Terminal shortcuts

## What are terminal shortcuts?

Terminal shortcuts help me work faster and avoid typing everything from scratch.

Simple meaning:

```text
Terminal shortcuts = quick keyboard actions that make terminal work easier
```

---

## Clear the terminal screen

Terminal command:

```bash
clear
```

What the syntax means:

```text
clear = clear the terminal screen
```

Simple meaning:

```text
Remove old terminal output from the screen so I can focus.
```

Important note:

```text
clear does not delete files.
clear only cleans the terminal view.
```

---

## Use the up arrow

Shortcut:

```text
Up Arrow
```

What it does:

```text
Shows the previous command I typed.
```

Simple meaning:

```text
Use the up arrow to repeat or edit an old command instead of typing it again.
```

Example:

If I typed this earlier:

```bash
git status
```

I can press the up arrow to bring it back.

---

## Use the down arrow

Shortcut:

```text
Down Arrow
```

What it does:

```text
Moves forward through command history after using the up arrow.
```

Simple meaning:

```text
Use the down arrow to move back toward newer commands.
```

---

## Use Tab autocomplete

Shortcut:

```text
Tab
```

What it does:

```text
Completes file or folder names automatically.
```

Simple meaning:

```text
Type part of a file or folder name, then press Tab to complete it.
```

Example:

```bash
cd ~/Devo
```

If I press Tab, the terminal may complete it to:

```bash
cd ~/Devop-learning-journey-
```

Another example:

```bash
code git-practice/git-terminal
```

Pressing Tab may complete the full file name.

Why this is useful:

```text
Tab helps me avoid spelling mistakes in long file names.
```

---

## Use Control + C to cancel

Shortcut:

```text
Control + C
```

What it does:

```text
Stops or cancels a command that is currently running.
```

Simple meaning:

```text
Use Control + C if the terminal is stuck or a command is still running.
```

Example:

If a command keeps running and does not stop, I can press:

```text
Control + C
```

Important note:

```text
Control + C cancels a running command.
It does not copy text in the terminal.
```

On Mac, copying text is usually:

```text
Command + C
```

---

## Use Control + L

Shortcut:

```text
Control + L
```

What it does:

```text
Clears the terminal screen.
```

Simple meaning:

```text
Control + L is a shortcut version of the clear command.
```

This is similar to typing:

```bash
clear
```

---

## Use q to quit reading mode

Shortcut:

```text
q
```

When to use it:

```text
When I am inside less, git log, or another page-by-page view.
```

Simple meaning:

```text
Press q to quit and return to the normal terminal.
```

Example:

If I run:

```bash
less git-practice/git-terminal-cleanup-lesson.md
```

I can exit by pressing:

```text
q
```

---

## Use Command + S in VS Code

Shortcut:

```text
Command + S
```

What it does:

```text
Saves the file I am editing in VS Code.
```

Simple meaning:

```text
Command + S saves the file on my laptop.
```

Important note:

```text
Command + S is not the same as git commit.
```

Difference:

```text
Command + S = save file changes in VS Code

git commit = save staged changes in Git history

git push = upload commits to GitHub
```

---

## Use Command + ` to open or hide terminal in VS Code

Shortcut:

```text
Command + `
```

What it does:

```text
Shows or hides the terminal panel in VS Code.
```

Simple meaning:

```text
Use Command + backtick to open or close the VS Code terminal quickly.
```

The backtick key usually looks like this:

```text
`
```

It is often near the Esc key on the keyboard.

---

## Use Control + A and Control + E

Shortcut:

```text
Control + A
```

What it does:

```text
Moves the cursor to the beginning of the command line.
```

Shortcut:

```text
Control + E
```

What it does:

```text
Moves the cursor to the end of the command line.
```

Simple meaning:

```text
Control + A = jump to the start of the command

Control + E = jump to the end of the command
```

These are useful when editing long commands.

---

## Useful beginner shortcut summary

```text
clear = clear terminal screen

Up Arrow = previous command

Down Arrow = newer command after using Up Arrow

Tab = autocomplete file or folder name

Control + C = cancel running command

Control + L = clear terminal screen

q = quit less or git log view

Command + S = save file in VS Code

Command + ` = show or hide terminal in VS Code

Control + A = move to beginning of command line

Control + E = move to end of command line
```

---

## My understanding

Terminal shortcuts help me work faster and make fewer mistakes.

For now, the most important ones for me are:

```text
Up Arrow
Tab
Control + C
q
Command + S
clear
```

I should practise these slowly while using the terminal, instead of trying to memorise everything at once.
