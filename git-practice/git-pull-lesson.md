# Git Pull Lesson

## What is git pull?

`git pull` brings the latest changes from GitHub into my local project folder.

Simple meaning:

```text
git pull = download the latest changes from GitHub to my laptop
```

---

## Push vs Pull

```text
git push = send my local committed work to GitHub

git pull = bring GitHub changes down to my local project
```

---

## Why git pull is important

`git pull` is important because my local project and GitHub project can become different.

For example:

```text
I edit a file directly on GitHub
Someone else pushes changes to the same repository
I use another laptop and push changes from there
```

In those cases, my laptop may not have the latest version.

So I use:

```bash
git pull
```

to update my local project.

---

## Basic syntax

```bash
git pull
```

This pulls changes from the connected GitHub branch.

In my project, this usually means:

```text
Pull from origin/main into my local main branch
```

---

## Normal workflow before starting work

Before I start editing files, I can run:

```bash
git status
git pull
```

Meaning:

```text
git status = check my current local project
git pull = get the latest changes from GitHub
```

---

## Normal workflow after finishing work

After editing files, I use:

```bash
git status
git add .
git commit -m "message"
git push
```

Meaning:

```text
git status = check what changed
git add . = prepare changes
git commit -m "message" = save changes locally
git push = upload changes to GitHub
```

---

## Full daily Git workflow

```bash
git pull
git status
git add .
git commit -m "message"
git push
```

Simple meaning:

```text
1. Pull latest changes from GitHub
2. Check what changed locally
3. Stage my changes
4. Commit my changes locally
5. Push my commit to GitHub
```

---

## What happens if there is nothing new?

If GitHub has no new changes, `git pull` may say:

```text
Already up to date.
```

This means:

```text
My laptop already has the latest version from GitHub.
```

---

## Key lesson

`git pull` helps me keep my local project updated with GitHub.

I should use it before starting work, especially if I edited files on GitHub or worked from another computer.