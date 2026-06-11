# Git Branch Lesson

## What is a Git branch?

A Git branch is like a separate version of my project.

It allows me to work on something new without affecting the main version of my project.

Simple meaning:

```text
A branch = a separate workspace inside the same project
```

---

## Why branches are useful

Branches are useful because I can test changes safely.

For example, if my main project is working well, I can create a new branch to try a new idea.

If the idea works, I can merge it back into the main branch.

If the idea does not work, I can delete the branch without damaging the main project.

---

## Check current branch

```bash
git branch
```

This shows the branches in my project.

The branch with `*` beside it is the branch I am currently using.

Example:

```text
* main
```

Simple meaning:

```text
git branch = show my branches
```

---

## Create a new branch

```bash
git branch branch-name
```

Example:

```bash
git branch lesson-practice
```

This creates a new branch called `lesson-practice`.

Simple meaning:

```text
git branch branch-name = create a new branch
```

---

## Switch to a branch

```bash
git switch branch-name
```

Example:

```bash
git switch lesson-practice
```

This moves me from my current branch to the `lesson-practice` branch.

Simple meaning:

```text
git switch branch-name = move to another branch
```

---

## Create and switch at the same time

```bash
git switch -c branch-name
```

Example:

```bash
git switch -c lesson-practice
```

This creates a new branch and switches into it immediately.

Simple meaning:

```text
git switch -c branch-name = create a branch and enter it
```

---

## Go back to main

```bash
git switch main
```

This moves me back to the main branch.

Simple meaning:

```text
git switch main = return to the main version of my project
```

---

## Merge a branch into main

First, go to main:

```bash
git switch main
```

Then merge the branch:

```bash
git merge lesson-practice
```

Simple meaning:

```text
git merge branch-name = bring changes from that branch into my current branch
```

---

## Delete a branch

```bash
git branch -d branch-name
```

Example:

```bash
git branch -d lesson-practice
```

This deletes the branch after it has been merged.

Simple meaning:

```text
git branch -d branch-name = delete a branch
```

---

## Key commands

```bash
git branch
git branch branch-name
git switch branch-name
git switch -c branch-name
git switch main
git merge branch-name
git branch -d branch-name
```

---

## Simple summary

```text
git branch = show branches
git branch branch-name = create branch
git switch branch-name = move to branch
git switch -c branch-name = create and move to branch
git switch main = go back to main
git merge branch-name = bring branch changes into current branch
git branch -d branch-name = delete branch
```
