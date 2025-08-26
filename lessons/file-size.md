# Checking the Size of Files and Directories in Ubuntu

## 1. Why do we care about size?

Every file on your computer takes up **space on the disk**. Some files are small (like text files), others are big (like videos). If you know how to check file sizes, you can:

* Avoid running out of disk space.
* Find out which folders are using the most space.
* Clean up unnecessary files.

---

## 2. Checking the size of a file

The simplest way is with the `ls -lh` command.

* `ls` lists files.
* The `-l` option shows details.
* The `-h` option makes the size **human readable** (KB, MB, GB).

👉 Example:

```bash
ls -lh myfile.txt
```

Output might look like:

```
-rw-r--r-- 1 toan toan 1.2K Aug 26 07:00 myfile.txt
```

Here, `1.2K` means the file is about **1.2 kilobytes**.

---

## 3. Checking the size of a directory

Files are easy, but what about a whole folder (directory)?

We use the `du` command (**d**isk **u**sage).

👉 Example:

```bash
du -sh myfolder
```

* `-s` = summary (just show total).
* `-h` = human readable.

Output might be:

```
4.5M    myfolder
```

This means the folder and everything inside it takes up **4.5 megabytes**.

---

## 4. Checking sizes of all files in a directory

👉 Example:

```bash
ls -lh
```

Shows the size of each file in the current directory.

👉 Example:

```bash
du -sh *
```

Shows the total size of each item (file or subdirectory) inside the current folder.

---


## 6. Units you will see

* **B** = Bytes (very small, 1 character = \~1 byte)
* **K** = Kilobytes (1,000 bytes)
* **M** = Megabytes (1,000 KB, about 1 million bytes)
* **G** = Gigabytes (1,000 MB, about 1 billion bytes)
* **T** = Terabytes (1,000 GB)

---

# Exercises

1. Make nano wrap long lines.

To make nano wrap long lines, we need to turn on `softwrap` feature of `nano`.
Create the file `.nanorc` in your home directory with content:

```
set softwrap
```

`.nanorc` is the user's configuration of nano. When `nano` starts, it loads and applies settings from this file. You need to close and re-open it to make the new setting takes effects.

2. Copy your `.nanorc` file into my home directory to make my nano sessions wrap long lines also. After copying, you need to change its owner to `duy` to make it work with my account. Use the command below to change a file's owner:

```
chown new_owner filename
```

3. What is the total size in bytes of the directory `/var/log`?
4. What is the total size in megabytes of the directory `/etc`?
5. Create the file `file-in-duy-group.txt` in the `tmp` directory and make it belong to `duy` group.
6. Correct the name of the file `~/work/ubuntu/answers/user-in-ubuntu.txt`. You need to use the `mv` command to rename a file.
