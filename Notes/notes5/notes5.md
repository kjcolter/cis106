# Linux Commands and File System

## Part 1: Linux Commands

### 1. `ls`

**Definition:**

The `ls` command is used to list files and directories inside a directory. It allows users to see the contents of their current location or another specified directory.

**Usage/Formula:**

```bash
ls [options] [directory]
```

**Examples:**

- List files and directories in the current directory:

  ```bash
  ls
  ```

- Display detailed information about files and directories:

  ```bash
  ls -l
  ```

- Show hidden files and directories:

  ```bash
  ls -a
  ```

- List the contents of a specific directory:

  ```bash
  ls /home
  ```

### 2. `pwd`

**Definition:**

The `pwd` command stands for **Print Working Directory**. It displays the full path of the directory that the user is currently working in.

**Usage/Formula:**

```bash
pwd
```

**Examples:**

- Display the current working directory:

  ```bash
  pwd
  ```

- Example output:

  ```text
  /home/student/Documents
  ```

  This means the user is currently inside the `Documents` directory, which is located inside `student` and `home`.

### 3. `cd`

**Definition:**

The `cd` command stands for **Change Directory**. It is used to move from one directory to another in the Linux file system.

**Usage/Formula:**

```bash
cd [directory]
```

**Examples:**

- Move into the Documents directory:

  ```bash
  cd Documents
  ```

- Move up one directory to the parent directory:

  ```bash
  cd ..
  ```

- Go directly to your home directory:

  ```bash
  cd ~
  ```

- Go to the root directory:

  ```bash
  cd /
  ```

---

## Part 2: Linux File System Questions

### 1. What is a variable?

A variable is a named storage location used to hold information or data that can be accessed and used later. In Linux, variables can store information such as text, numbers, and directory paths.

**Example:**

```bash
name="John"
```

This creates a variable named `name` and stores the value `John` inside it.

### 2. How do I use a variable?

You use a variable by placing a dollar sign (`$`) before its name. This allows the shell to access the value stored in that variable.

**Example:**

```bash
name="John"
echo $name
```

**Output:**

```text
John
```

The `echo` command displays the value stored in the variable.

### 3. What is an environment variable?

An environment variable is a variable that stores information about the environment in which programs and processes run. These variables can be accessed by programs started from the shell.

**Examples:**

- `$HOME` – Stores the path to the current user's home directory.
- `$PATH` – Contains the directories Linux searches when looking for executable commands.
- `$USER` – Stores the current username.

To display an environment variable, use:

```bash
echo $HOME
```

### 4. What is a user-defined variable?

A user-defined variable is a variable that a user creates and gives a name to. It can store information that the user wants to use in commands or scripts.

**Example:**

```bash
city="New York"
echo $city
```

**Output:**

```text
New York
```

The variable `city` was created by the user to store the text `New York`.

### 5. What is the root directory?

The root directory is the top-level directory in the Linux file system. It is represented by a forward slash (`/`). All other files and directories are located somewhere underneath the root directory.

**Example:**

```text
/
├── home
├── etc
├── bin
├── usr
└── var
```

To access the root directory, use:

```bash
cd /
```

### 6. What does "Parent Directory" mean?

A parent directory is a directory that contains another directory or file. It is one level above the current directory in the file system.

The double dots (`..`) represent the parent directory in Linux.

**Example:**

If the current directory is:

```text
/home/student/Documents
```

The parent directory is:

```text
/home/student
```

To move to the parent directory, use:

```bash
cd ..
```

### 7. What does "Current Working Directory" mean?

The current working directory is the directory that a user is currently located in while using the Linux terminal. Commands such as `ls` will normally operate on this directory unless another location is specified.

**Example:**

```bash
pwd
```

**Output:**

```text
/home/student/Documents
```

This tells the user that their current working directory is `Documents`.

### 8. What is an absolute path? Include an example.

An absolute path is the complete path to a file or directory starting from the root directory (`/`). It gives the exact location of something in the Linux file system, regardless of the current working directory.

**Example:**

```text
/home/student/Documents/assignment.txt
```

This path starts at the root directory and shows the complete location of the file named `assignment.txt`.

### 9. What is a relative path? Include an example.

A relative path is a path that describes the location of a file or directory in relation to the current working directory. It does not start with the root directory (`/`).

**Example:**

If the current working directory is:

```text
/home/student
```

The relative path to the Documents directory is:

```text
Documents
```

You can access it using:

```bash
cd Documents
```

Unlike an absolute path, a relative path depends on where the user is currently located.

### 10. What is the difference between "Your home directory" and "The home directory"?

**Your home directory:**

Your home directory is the personal directory assigned to your individual user account. It is where your personal files, folders, and user settings are normally stored.

For example:

```text
/home/student
```

The shortcut `~` represents your own home directory.

You can access it using:

```bash
cd ~
```

**The home directory:**

The home directory (`/home`) is the directory that normally contains the home directories of regular user accounts on a Linux system.

For example:

```text
/home
├── student
├── john
└── mary
```

**Main Difference:**

The home directory (`/home`) is the location that contains users' personal directories, while your home directory (`/home/student`) is the specific directory assigned to your own account.
