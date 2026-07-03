# Question 3 – File System and Link Analysis

## Command 1

**Command**

```bash
echo "Linux Link Experiment" > original.txt
```

**Output**

(No output)

**Explanation**

Creates a file named `original.txt` with sample content.

---

## Command 2

**Command**

```bash
ln original.txt hardlink.txt
```

**Output**

(No output)

**Explanation**

Creates a hard link to the original file.

---

## Command 3

**Command**

```bash
ln -s original.txt softlink.txt
```

**Output**

(No output)

**Explanation**

Creates a symbolic link pointing to the original file.

---

## Command 4

**Command**

```bash
ls -i
```

**Output**

(Paste your output.)

**Explanation**

Displays inode numbers for the files.

---

## Command 5

**Command**

```bash
stat original.txt
stat hardlink.txt
stat softlink.txt
```

**Output**

(Paste your output.)

**Explanation**

Displays detailed metadata such as inode number, permissions, owner, and timestamps.

---

## Command 6

**Command**

```bash
rm original.txt
```

**Output**

(No output)

**Explanation**

Deletes the original file.

---

## Command 7

**Command**

```bash
cat hardlink.txt
```

**Output**

```
Linux Link Experiment
```

**Explanation**

Shows that the hard link still works after deleting the original file.

---

## Command 8

**Command**

```bash
cat softlink.txt
```

**Output**

```
No such file or directory
```

**Explanation**

Demonstrates that the symbolic link is broken after deleting the original file.
