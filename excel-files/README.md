code excel-files/README.md
# Excel Files

This folder will contain my Excel practice files and spreadsheet-related learning for DevOps, data, and automation practice.
git add .                         = terminal
git status                        = terminal
git commit -m "Add excel files folder" = terminal
git push                          = terminal
code excel-files/README.md        = terminal
# Excel Files...                  = inside the note/file
excel-files/README.md             = do not type alone
git add .      = select the pages you want to save
git commit     = save those pages on your laptop
git push       = upload those saved pages to GitHub
# Basic Linux / Terminal Commands

## pwd

`pwd` means **print working directory**.

It shows the folder I am currently inside.

Example:

```bash
pwd
```

Example output:

```bash
/Users/tayoadio/devops-learning-journey
```

Simple meaning:

```text
pwd = Where am I?
```

---

## ls

`ls` means **list**.

It shows the files and folders inside my current location.

Example:

```bash
ls
```

Example output:

```text
README.md
linux-notes
python-practice
```

Simple meaning:

```text
ls = What is inside this folder?
```

---

## cd

`cd` means **change directory**.

It is used to enter or move into a folder.

Example:

```bash
cd linux-notes
```

Simple meaning:

```text
cd folder-name = go inside that folder
```

---

## cd ..

`cd ..` moves me back one folder level.

Example:

```bash
cd ..
```

If I am inside:

```text
devops-learning-journey/linux-notes
```

and I run:

```bash
cd ..
```

I move back to:

```text
devops-learning-journey
```

Simple meaning:

```text
cd .. = go back one folder
```

---

## mkdir

`mkdir` means **make directory**.

It creates a new folder.

Example:

```bash
mkdir ADIO
```

This creates a folder called `ADIO`.

Simple meaning:

```text
mkdir folder-name = create a folder
```

---

## touch

`touch` creates a new empty file.

Example:

```bash
touch Tayo
```

This creates a file called `Tayo`.

Simple meaning:

```text
touch file-name = create a file
```

---

## rm

`rm` means **remove**.

It deletes a file.

Example:

```bash
rm Tayo
```

This deletes the file called `Tayo`.

Simple meaning:

```text
rm file-name = delete a file
```

---

## rmdir

`rmdir` means **remove directory**.

It deletes an empty folder.

Example:

```bash
rmdir ADIO
```

This deletes the folder called `ADIO`, but only if the folder is empty.

Simple meaning:

```text
rmdir folder-name = delete an empty folder
```

---

## rm -r

`rm -r` deletes a folder and everything inside it.

Example:

```bash
rm -r ADIO
```

This deletes the `ADIO` folder, including any files or folders inside it.

Simple meaning:

```text
rm -r folder-name = delete a folder and everything inside it
```

Important note:

```text
Be careful with rm -r because it deletes directly from the terminal.
```

---

## cp

`cp` means **copy**.

It copies a file.

Example:

```bash
cp app.log app-copy.log
```

This copies `app.log` and creates a new copy called `app-copy.log`.

Simple meaning:

```text
cp original-file new-copy-file = copy a file
```

---

## mv

`mv` means **move**.

It can be used to rename a file or move a file into another folder.

Example 1, rename a file:

```bash
mv app-copy.log backup.log
```

This renames `app-copy.log` to `backup.log`.

Example 2, move a file into a folder:

```bash
mv backup.log backups/
```

This moves `backup.log` into the `backups` folder.

Simple meaning:

```text
mv old-name new-name = rename
mv file-name folder-name/ = move file into folder
```

---

## grep

`grep` searches for text inside a file.

Example:

```bash
grep "ERROR" app.log
```

This searches for the word `ERROR` inside `app.log`.

Example output:

```text
ERROR: Database connection failed
ERROR: Payment service timeout
```

Case-insensitive search:

```bash
grep -i "error" app.log
```

This finds `error`, `Error`, or `ERROR`.

Simple meaning:

```text
grep "word" file-name = search inside a file
```

---

## head

`head` shows the first lines of a file.

Example:

```bash
head app.log
```

To show only the first 3 lines:

```bash
head -n 3 app.log
```

Simple meaning:

```text
head = show the beginning of a file
```

---

## tail

`tail` shows the last lines of a file.

Example:

```bash
tail app.log
```

To show only the last 3 lines:

```bash
tail -n 3 app.log
```

Simple meaning:

```text
tail = show the end of a file
```

This is useful in DevOps because logs are usually checked from the bottom to see the latest activity.

---

## less

`less` opens a file in reading mode.

Example:

```bash
less app.log
```

Inside `less`, I can use:

```text
Down arrow = move down
Up arrow = move up
Space = move forward
q = quit
```

Simple meaning:

```text
less = read a file page by page without editing it
```

---

## chmod

`chmod` means **change mode**.

It changes file permissions.

The beginner example is:

```bash
chmod +x hello.sh
```

This makes `hello.sh` executable, which means I can run it like a script.

Example:

```bash
chmod +x hello.sh
./hello.sh
```

Simple meaning:

```text
chmod +x file-name = allow the file to run like a program
```
