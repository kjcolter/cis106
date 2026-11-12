# Notes 7

# Question 3: Wildcards and Brace Expansion

## 1. How to Use Each of the Wildcards

Wildcards are special characters used in Linux to match filenames and directories. They allow users to work with multiple files without typing each filename individually.

### A. Asterisk (`*`)

The asterisk matches zero or more characters in a filename.

**Examples:**

```bash
ls *.txt
```
Displays all files ending in `.txt`.

```bash
ls photo*
```
Displays files that start with `photo`.

```bash
rm *.log
```
Deletes all files ending in `.log` in the current directory.

### B. Question Mark (`?`)

The question mark matches exactly one character.

**Examples:**

```bash
ls file?.txt
```
Matches `file1.txt`, `file2.txt`, or `fileA.txt`.

```bash
ls img?.jpg
```
Matches `img1.jpg` and `img2.jpg`, but not `img10.jpg`.

```bash
ls ???.txt
```
Matches filenames containing exactly three characters before `.txt`.

### C. Square Brackets (`[]`)

Square brackets match exactly one character from a specified set or range.

**Examples:**

```bash
ls file[123].txt
```
Matches `file1.txt`, `file2.txt`, and `file3.txt`.

```bash
ls file[a-z].txt
```
Matches files with one lowercase letter in that position.

```bash
ls photo[0-9].jpg
```
Matches photos with one digit from 0 through 9.

---

## 2. How to Use Brace Expansion to Create Entire Directory Structures

Brace expansion allows users to create multiple directories or files with one command. It uses curly braces `{}` to specify multiple names or options.

### Example 1: Create a Wallpapers Directory Structure

```bash
mkdir -p wallpapers/cars/{1080p,2k,4k}
```

This creates the following directory structure:

```text
wallpapers/
└── cars/
    ├── 1080p/
    ├── 2k/
    └── 4k/
```

### Example 2: Create an Assets Directory Structure

```bash
mkdir -p assets/{imgs,video}/{large,small}
```

This creates the following directory structure:

```text
assets/
├── imgs/
│   ├── large/
│   └── small/
└── video/
    ├── large/
    └── small/
```

### Example 3: Create Multiple Project Directories

```bash
mkdir -p projects/{school,work,personal}/{documents,images,backup}
```

This creates the following directory structure:

```text
projects/
├── school/
│   ├── documents/
│   ├── images/
│   └── backup/
├── work/
│   ├── documents/
│   ├── images/
│   └── backup/
└── personal/
    ├── documents/
    ├── images/
    └── backup/
```
