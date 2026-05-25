# 🐧 Linux Notes

## 📌 What is Linux?

- _Open-source operating system developed by Linus Torvalds. Known for its security, flexibility, and strong community support._

## ❓ Why Learn Linux?

- _It is widely used in servers, especially in cloud environments._

---

## 💡 Before You Start: Terminal & Commands

### 💻 What is a Terminal?

- _The terminal (or console) is a text-based interface used to interact with the system by typing commands._
 

### 📥 What is a Command?

- _A command is an instruction given to the computer to perform a specific task._
- _Can be entered directly in the terminal and is **case sensitive**._
- _Each command has a manual page ``man``, which is built-in documentation that explains how it works._

### 🧱 Basic Command Structure
A Linux command typically has 3 main parts (or attributes):
``` 
command options arguments
```
- _**Command** is the actual program that you want the system to run_
- _**Options** modify the behavior of the command. They usually start with `-` or `--`._
- _**Arguments** tell the command **what to act on**. They are usually **file names, directories, users, or other inputs**._


## 📚 What’s Covered

1. Basic Linux Commands
2. The Shell 
3. Linux File System
4. User and Group Management
5. Advanced Topics

---

## 1.  Basic Linux Commands

- _`ls ` → list the content of the current directory_.
- _`ls -a ` → list all files, including hidden ones (those that start with `.`)_.
- _`cd ` → change directory_.
- _`touch` → Create a new empty file_.
- _`echo ` → Print text to terminal (or write to a file using redirection, e.g., `>` or `>>`)_.
- _`cat` → Display the content of a file in the terminal_.
- _`grep` → Search for a specific string or pattern inside a file_.
---

## 2.  The Shell 

- _A shell is like a **translator** or **middleman** between you (the user) and the linux kernel (the core of the operating system)_.
- _A simple flow of a shell: you type a command → the shell interprets it → talks to the Kernel → the Kernel tells the computer what to do → you see the result on the screen_.
- _We don’t talk to the kernel directly because it’s too low-level, complex, and unsafe — the shell acts as a safer and easier way to interact with the system_.
- _Different shells offer **different features and styles**, but all do the same basic job_.
- _For example, `bash` is the most common shell, while `zsh` stands out for its advanced features like auto-completion and spelling correction. Below are the common shell commands_.
- _To find out your current shell_  → `echo $SHELL`
- _To change default shell_  → e.g., `chsh -s /bin/zsh`
- _To know what shell you have_  → `cat /etc/shells`. _Once you changed the default shell, you must restart the instance._ 
---

## 3.  Linux File System

- _Organised in a hierarichial structure. Starting from the **root directory** denoted as `/`_. _Key directories are listed below_.
- _`/` → root directory, top level of the file system_.
- _`/home` → This is where users "live" — it contains a personal directory for each user._
- _`var` → stores variables, log, databases, etc.._.
- _Linux treats everything as a file including **devices and processes**_.
- _To create file, recap on your `touch` and `echo` commands_.
- The `head` and `tail` commands let you view the first or last few lines of a file. For example, `head -5` shows the first 5 lines, while `tail -5` shows the last 5 lines.
#### Common file commands
- `cp`, `mv`, and `rm` are used to **copy**, **move/rename**, and **delete** files and directories.
- Use `cp -r` to **copy directories recursively** (including all files and subfolders).
- The `mv` command can also be used to **rename files or folders**.
#### Working with directories 
- `mkdir` → Create a new directory.
- `rmdir` → Remove an **empty** directory.
- `rm -r` → Remove a **non-empty** directory and its contents.
- Use `mkdir -p` to **create nested directories** in one step (e.g., `project/source/components`).

> 💡 **Tip:** Use `rmdir` for empty folders and `rm -r` for folders that contain files.

## 4.  User and Group Management

_Work in progress — will update soon!._

---

## 5. Advanced Topics

_Work in progress — will update soon!._

---

## 📝 Notes & References
