# Lesson 1: Introduction to Git

## 1. What is Git?

* Git is a **version control system**.
* It helps programmers keep track of changes in their code, like saving different versions of a video game project or a school essay.
* With Git, you can:

  * Save your work in "snapshots" (called **commits**).
  * Go back to older versions if something breaks.
  * Work together with friends on the same project without messing up each other’s changes.

---

## 2. Key Ideas

* **Repository (repo):** A special folder that Git tracks.
* **Commit:** A saved snapshot of your files at a certain time.
* **Branch:** A separate line of development. You can test new ideas here without breaking the main project.
* **Merge:** Combining changes from one branch into another.
* **Remote:** An online copy of your repo (like on GitHub) so others can work with you.

---

## 3. Basic Workflow

Imagine you’re writing a story:

1. **Create a repo** (tell Git: “please track this folder”).

   ```bash
   git init
   ```
2. **Add files** (choose what you want to save).

   ```bash
   git add filename.txt
   ```
3. **Commit changes** (take a snapshot).

   ```bash
   git commit -m "Write first chapter"
   ```
4. **Check status** (see what’s going on).

   ```bash
   git status
   ```
5. **View history** (see old versions).

   ```bash
   git log
   ```

---

## 4. Example

Let’s say you are writing a story in a file called `story.txt`.

```bash
# Step 1: Create a folder and go inside
mkdir my-story
cd my-story

# Step 2: Tell Git to track this folder
git init

# Step 3: Create the file
echo "Once upon a time..." > story.txt

# Step 4: Add it to Git
git add story.txt

# Step 5: Save a snapshot
git commit -m "Start the story"
```

If you later add another sentence and commits again, Git will remember both versions.

---

## 5. Why Git is Useful

* If you **make a mistake**, you can go back.
* If you **try new ideas**, you can use branches.
* If you **work with friends**, everyone can share updates.

It’s like a **time machine + teamwork tool** for code and text.

---

## 6. Practice Exercises

1. Create a folder called `my-notes` in the `tmp` directory. Initialize it with Git.
2. Make a file `notes.txt` with one line of text, add it, and commit.
3. Add another line, then commit again.
4. Use `git log` to see your history.
5. Try changing something, but **don’t commit yet**. Run `git status` and see what Git says.
6. Do you have any questions? Write your questions in the file `~/work/ubuntu/note/git-questions.md`.
7. Take notes about this lesson. 

---

