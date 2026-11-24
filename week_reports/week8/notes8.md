# Notes 8

## 1. `cat`

**Definition:**

The `cat` command is used to show what is inside a text file. 

**Usage/Formula:**

```bash
cat [filename]
```

**Examples:**

1. Show the contents of a file:
   ```bash
   cat notes.txt
   ```

2. Show the contents of two files:
   ```bash
   cat file1.txt file2.txt
   ```


---

## 2. `tac`

**Definition:**

The `tac` displays the lines in reverse order. 

**Usage/Formula:**

```bash
tac [filename]
```

**Examples:**

1. Display a file in reverse order:
   ```bash
   tac notes.txt
   ```


2. Display two files in reverse line order:
   ```bash
   tac file1.txt file2.txt
   ```

---

## 3. `head`

**Definition:**

The `head` command shows the beginning of a file. By default, it displays the first 10 lines.

**Usage/Formula:**

```bash
head [options] [filename]
```

**Examples:**

1. Show the first 10 lines of a file:
   ```bash
   head notes.txt
   ```

2. Show only the first 5 lines:
   ```bash
   head -n 5 notes.txt
   ```

3. Show the first 20 lines:
   ```bash
   head -n 20 notes.txt
   ```

---

## 4. `tail`

**Definition:**

The `tail` command shows the end of a file. It displays the last 10 lines by default.

**Usage/Formula:**

```bash
tail [options] [filename]
```

**Examples:**

1. Show the last 10 lines of a file:
   ```bash
   tail notes.txt
   ```

2. Show only the last 5 lines:
   ```bash
   tail -n 5 notes.txt
   ```

---

## 5. `cut`

**Definition:**

The `cut` command is used to take out certain parts of a line from a file. You can choose specific characters or fields that you want to display.

**Usage/Formula:**

```bash
cut [options] [filename]
```

**Examples:**

1. Display the first 5 characters of each line:
   ```bash
   cut -c 1-5 names.txt
   ```

2. Display the first field from a CSV file:
   ```bash
   cut -d ',' -f 1 dracula.csv
   ```

3. Display the second field from a CSV file:
   ```bash
   cut -d ',' -f 2 dracula.csv
   ```

---

## 6. `sort`

**Definition:**

The `sort` command is used to organize the lines in a file. It can put words in alphabetical order or numbers in numerical order.

**Usage/Formula:**

```bash
sort [options] [filename]
```

**Examples:**

1. Sort names alphabetically:
   ```bash
   sort names.txt
   ```

2. Sort names in reverse order:
   ```bash
   sort -r names.txt
   ```

3. Sort numbers from smallest to largest:
   ```bash
   sort -n numbers.txt
   ```

---

## 7. `wc`

**Definition:**

The `wc` command stands for word count. It is used to count how many lines, words, and bytes are in a file.

**Usage/Formula:**

```bash
wc [options] [filename]
```

**Examples:**

1. Count the lines, words, and bytes in a file:
   ```bash
   wc notes.txt
   ```

2. Count only the lines:
   ```bash
   wc -l notes.txt
   ```

3. Count only the words:
   ```bash
   wc -w notes.txt
   ```

4. Count the characters:
   ```bash
   wc -m notes.txt
   ```

---

## Summary

| Command | What it does |
|---|---|
| `cat` | Shows the contents of a file or combines files. |
| `tac` | Shows the lines of a file in reverse order. |
| `head` | Shows the first lines of a file. |
| `tail` | Shows the last lines of a file. |
| `cut` | Takes out specific parts of a line. |
| `sort` | Puts lines in alphabetical or numerical order. |
| `wc` | Counts lines, words, and characters in a file. |