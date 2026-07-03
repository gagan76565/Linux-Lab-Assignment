# Question 4 - File Access and I/O Investigation

## Command 1

### Command

```bash
echo "Linux File IO Investigation" > sample.log
```

### Output

```
(No output)
```

### Explanation

The `echo` command creates a file named `sample.log` and writes sample text into it.

---

## Command 2

### Command

```bash
cat sample.log
```

### Output

```
Linux File IO Investigation
```

### Explanation

The `cat` command displays the contents of the file to verify that it was created successfully.

---

## Command 3

### Command

```bash
lsof sample.log
```

### Output

```
(Paste your terminal output here)
```

### Explanation

The `lsof` command lists processes that currently have the file open.

---

## Command 4

### Command

```bash
ls -l /proc/$$/fd
```

### Output

```
(Paste your terminal output here)
```

### Explanation

This command displays the file descriptors currently used by the shell process.

---
