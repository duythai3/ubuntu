# Lesson: Users on Ubuntu

## 1. What is a User?

A **user** is like an account on Ubuntu.
Ubuntu uses accounts to know **who you are** and **what you can do**.

Each user has:

* A **username** (like "toan" or "duy").
* A **home folder** (where your personal files are stored).
* A set of **permissions** (what you are allowed to do).

---

## 2. Why Do We Need Users?

Imagine a family computer:

* Toan has his own account.
* Dad has his account.
* Mom has hers.

Each person can:

* Keep private files (home folder).
* Set their own wallpaper and settings.
* Avoid breaking each other’s files.

Users also keep the system safe:

* Regular users can’t damage the system.
* Only the **administrator (root)** can install or remove software.

---

## 3. Types of Users

1. **Root User**

   * The most powerful account (like a “superuser”).
   * Can change any file, install software, and control the whole system.
   * Usually hidden for safety.

2. **Regular Users**

   * Normal accounts for everyday use.
   * Can create files, change their own settings, and use programs.
   * Need permission to do system changes.

3. **System Users**

   * Invisible accounts that Ubuntu creates for services (like web servers or databases).
   * You usually don’t log into them.

---

## 4. The Home Directory

Every user has a **home folder**:

* Located at `/home/username`
* Example:

  * Toan’s files → `/home/toan`
  * Dad’s files → `/home/duy`

This is where you keep documents, pictures, and downloads.
Ubuntu protects your folder so other users cannot read or change it without permission.

---

## 5. Switching Users

On Ubuntu Desktop:

* You can switch users from the login screen.
* Or click User Menu → “Switch User”.

On the command line:

```bash
su - username
```

(`su` means "switch user").

To return, type:

```bash
exit
```

---

## 6. Sudo: Superuser for a Moment

Instead of logging in as the root user, Ubuntu lets regular users temporarily act like root with `sudo`.

Example:

```bash
sudo apt update
```

* `sudo` = “superuser do”
* It will ask for your password.
* After that, the command runs as root.

This keeps the system safe because you only have root powers when necessary.

---

## 7. Creating and Managing Users

On the command line:

* **Create a new user:**

  ```bash
  sudo adduser newusername
  ```

* **Delete a user:**

  ```bash
  sudo deluser username
  ```

* **See all users:**

  ```bash
  cat /etc/passwd
  ```

---

## 8. Practice Tasks

1. Find your username with:

   ```bash
   whoami
   ```

2. Find your home folder with:

   ```bash
   echo $HOME
   ```

3. Use `sudo ls /root` → It should only work with `sudo`.

4. Try to create a new test user:

   ```bash
   sudo adduser testuser
   ```

5. Switch to that user:

   ```bash
   su - testuser
   ```

---

## 9. Summary

* Users are accounts on Ubuntu that control **access** and **permissions**.
* Each user has a home directory.
* The root user is the superuser.
* `sudo` lets you run commands as root safely.
* You can create, switch, and manage users from the terminal.

