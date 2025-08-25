>Toàn ơi,<br>
>Để giúp con ghi nhớ các thư mục dể dàng, ba sắp xếp nó lại như sau:
```
~/work/
   |──ubuntu/
      ├──lessons/
      ├──answers/
      ├──notes/
      ├──tmp/

```

- `~/work/ubuntu/lessons` chứa các bài học ba tạo ra.
- `~/work/ubuntu/answers` chứa các bài làm của con.
- `~/work/ubuntu/notes` chứa các ghi chú của con.
- `~/work/ubuntu/tmp` chứa các file tạm con tạo ra khi thực hành.

Thư mục `ubuntu` này là một repository trên server `github.com`.
Sau khi con làm bài xong thì con phải commit bài làm của con lên repository `ubuntu` trên `github.com` để ba có thể thấy được:

```
cd ~/work/ubuntu
./pull.sh
./commit.sh
```


---
Got it 👍 Let’s create a **lesson for Toan (14 years old)** about **permissions of users on Ubuntu**.
The style will be **clear, simple, and teenager-friendly**, so he can read and study by himself.

---

# 📘 Lesson: Understanding Permissions of Users on Ubuntu

## 1. Why Do We Need Permissions?

Imagine your computer is like a big house:

* Each **user** has their own room (home directory).
* Some areas are **shared** (like the kitchen).
* Some areas are **locked** so only certain people can enter.

Permissions are the **rules** that tell the computer who can:

* **Read** (look inside a file or folder)
* **Write** (change it)
* **Execute** (run it like a program)

Without permissions, anyone could mess up anyone else’s files — and that would be chaos!

---

## 2. The Three Types of Permissions

On Ubuntu (and Linux in general), every file and folder has three kinds of permissions:

1. **Read (r)** – You can open and read the file.
2. **Write (w)** – You can change the file or add/remove files inside a folder.
3. **Execute (x)** – You can run the file if it’s a program/script, or enter a folder.

---

## 3. The Three Groups of People

Permissions apply to three groups:

1. **User (u)** – The owner of the file.
2. **Group (g)** – A group of users (like teammates).
3. **Others (o)** – Everyone else.

So each file has permissions for **user, group, and others**.

---

## 4. Seeing Permissions

Open a terminal and type:

```bash
ls -l
```

You’ll see something like:

```
-rwxr-xr--  1 toan family  1234 Aug 25 09:00 script.sh
```

Let’s break it down:

* **-rwxr-xr--**

  * `-` → it’s a file (if it were a folder, it would be `d`)
  * `rwx` → user has read, write, execute
  * `r-x` → group has read, execute
  * `r--` → others have read only

So in plain English:

* The owner (toan) can do everything.
* The group (family) can read and run it, but not edit it.
* Others can only read.

---

## 5. Changing Permissions

We use the command **chmod** (change mode).

Examples:

* Add execute permission for user:

  ```bash
  chmod u+x script.sh
  ```
* Remove write permission for others:

  ```bash
  chmod o-w file.txt
  ```
* Give everyone read and write:

  ```bash
  chmod a+rw notes.txt
  ```

(`a` means **all users**)

---

## 6. Numeric (Shortcut) Permissions

Instead of `rwx`, we can use numbers:

* **4 = read**
* **2 = write**
* **1 = execute**

Add them together:

* `7 = rwx`
* `6 = rw-`
* `5 = r-x`
* `4 = r--`

So:

```bash
chmod 755 script.sh
```

Means:

* User = 7 (rwx)
* Group = 5 (r-x)
* Others = 5 (r-x)

---

## 7. Ownership

Each file has an **owner** and a **group**.

Check with:

```bash
ls -l
```

Change owner with:

```bash
sudo chown newuser file.txt
```

Change group with:

```bash
sudo chgrp newgroup file.txt
```

---

## 8. Why It Matters

Permissions protect:

* Your files from being deleted accidentally.
* The system from being broken by mistakes.
* Privacy (others can’t read your personal files).

---

✅ **Summary:**

* Permissions = rules (read, write, execute).
* Apply to user, group, others.
* Check with `ls -l`.
* Change with `chmod`.
* Ownership matters too.

---

👉 Do you want me to also create **exercises** for Toan (like practice tasks after reading this lesson) so he can test what he learned?

