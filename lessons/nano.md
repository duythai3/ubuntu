# The Nano Text Editor
### 1. What is Nano?
- Nano is a program that lets you write and edit text files inside the terminal.
- You can use it to write notes, code, or even edit system settings.
- At the bottom of the screen, nano shows you helpful shortcuts.<br>
Example: ^O means **Ctrl + O** (hold **Ctrl**, then press **O**).
### 2. Opening Nano
Type this in the terminal:
```
# Change to the temporary directory you created in previous lesson
cd ~/learn/tmp
# Start nano
nano
```
This opens nano with a blank page.<br>
To open (or create) a file directly:
```
nano t1.txt
```
Try it: Open `nano` and type a sentence, like:
```
I will use nano to take note while I am learning Ubuntu.
```
### 3. Saving Your Work
To save in nano:
- Press **Ctrl + O** (that’s “Write Out”).
- Nano asks for a file name. Type `t1.txt` and press **Enter**.
- To quit nano, press **Ctrl + X**.
Now you have saved your first text file!
### 4. Opening a File Again
To open the file you saved:
```
nano t1.txt
```
Now you can see your text again and add more lines.
### 5. Important Shortcuts
- Save file: `Ctrl + O` or `Ctrl + S`
- Exit nano: `Ctrl + X`
- Cut a line or selected text into nano's clipboard: `Ctrl + K`
- Copy current line or selected text into clipboard: `Alt + 6`
- Paste text from the clipboard to current position: `Ctrl + U`
- Search for text: `Ctrl + W`
- Undo: `Alt + U`
- Redo: `Alt + E`
### 6. Practice Exercises
#### 1. Create a directory to keep your notes.
```
# create directories
mkdir ~/work
mkdir ~/work/note
mkdir ~/work/note/ubuntu
# change to the directory used to keep notes about ubuntu
cd ~/work/note/ubuntu
```
#### 2. Take notes about `nano` editor.<br>
Use `nano` to create file `nano.txt` in your ubuntu note directory
```
nano nano.txt
```
Type text below:
```
- Save file: Ctrl + O
- Exit nano: Ctrl + X
- Cut (delete) a line: Ctrl + K
- Paste a line: Ctrl + U
- Search for text: Ctrl + W
- Go to start of line: Ctrl + A
- Go to end of line: Ctrl + E
```
Then save the file and exit `nano`.<br>
Open the `nano.txt` file and append text below:
```
- ^S means Ctrl + S
- M-6 means Alt + 6
```
Then save and exit `nano`.<br>
#### 3. Practice `nano`'s shutcuts.
- Create a temp file for practicing `nano`:
```
cd ~/learn/tmp
nano t1.txt
```
- Type and duplicate text below:
```
This line will be duplicated
```
- Copy the word `duplicated` to a new line

>Select the word `duplicated` by `Shift + Left Arrow/Right Arrow`,<br>
>press `M-6` to copy selected text to nano clipboard,<br>
>and press `^U` to paste the text from clipboard to the caret position.

- Duplicate the word "line"
- Create a new line with text "This line will be remove because it is a duplicated line" by using `M-6`, `^U` to copy the first line and edit it.
- Try `M-U` and `M-E`
- Use `M-U` to revert the file to empty and exit `nano`
