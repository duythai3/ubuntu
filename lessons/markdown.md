# Introduction to Markdown Syntax

## 1. What is Markdown?

Markdown is a lightweight way to write text that looks nice when converted to HTML.
It’s commonly used in **README files**, **notes**, and **documentation**.

With Markdown, you can write plain text but add styles like **bold**, *italic*, lists, links, images, and more.

---

## 2. Headings

You create headings by adding `#` before a line.
The number of `#` symbols decides the size of the heading.

Example:

```markdown
# Heading 1
## Heading 2
### Heading 3
```

Result:

# Heading 1

## Heading 2

### Heading 3

---

## 3. Bold and Italic

* **Bold** text uses `**word**` or `__word__`
* *Italic* text uses `*word*` or `_word_`
* ***Bold + Italic*** uses `***word***`

Example:

```markdown
This is **bold**, this is *italic*, and this is ***bold + italic***.
```

---

## 4. Lists

### Unordered lists

Use `-`, `*`, or `+` followed by a space.

```markdown
- Item 1
- Item 2
  - Sub item
```

Result:

* Item 1
* Item 2

  * Sub item

### Ordered lists

Use numbers with a dot.

```markdown
1. First
2. Second
3. Third
```

Result:

1. First
2. Second
3. Third

---

## 5. Links and Images

* Links: `[text](URL)`
* Images: `![alt text](image_url)`

Example:

```markdown
[Google](https://google.com)

![Cute Cat](https://placekitten.com/200/300)
```

---

## 6. Code

For short code, wrap it in backticks `` ` ``.
For blocks of code, use triple backticks.

Example:

```
Inline code: `echo "Hello World"`
```

```
```
def hello():
    print("Hello World")
```
```


---

## 7. Blockquotes
Use `>` to quote text.

```markdown
> This is line 1 of a quote.
> This is line 2 of a quote.
> This is line 3 of a quote.
````

Result:

> This is line 1 of a quote.
> This is line 2 of a quote.
> This is line 3 of a quote.

---

## 8. Tables

You can make simple tables using `|` and `-`.

```markdown
| Name | Age |
|------|-----|
| Toan | 14  |
| Alex | 15  |
```

Result:

| Name | Age |
| ---- | --- |
| Toan | 14  |
| Alex | 15  |

---

## 9. Horizontal Line

Use three or more dashes `---` or asterisks `***`.

```markdown
---
```

---

# Practice

1. View a markdown file.

Almost lessons I created for you are in markdown syntax. Look inside the `lessons` directory to find for `*.md` files. Open some files by using `nano` to see how `markdown` syntax look like.
Github understand `*.md` files, and it translates a `markdown` file to an `html` file that is the final format you see when you read my lesson.
Try the following:

- Copy a `*.md` file from the `lessons` directory to the `tmp` directory.
- Edit the file in the `tmp` directory by using `nano`.
- Commit your branch (student) to github.
- View your editied file on github.com.

In the `ubuntu` repo, I created two branches `main` and `student`. When you commit your works, they will be saved into the branch `student`, so you need to find your branch on github to view the file you edited.

2. Create a `markdown` file in the `tmp` directory, and do the following:

- Write your name in **bold** and your favorite food in *italic*.
- Create a shopping list with 3 items using an unordered list.
- Write a quote from your favorite movie using blockquote style.
- Add a link to your favorite website.
- Make a small table with two columns: “Game” and “Rating”.

3. Translate the first lesson to `markdown` format.

The first lesson that I created for you is in `pdf` format, so help me translate it into `markdown` format.

- View the lesson by cicking on this link:[Linux Filesystem](https://github.com/duythai3/ubuntu/blob/main/lessons/Linux%20Filesystem.pdf)
- Create file `linux-filesystem.md` in the `lessons` directory by using `nano`. Try to make the lesson in `markdown` format look the same as in `pdf` format.
- You don't need to take notes for this lesson today, the file `linux-filesystem.md` is enough.

---

