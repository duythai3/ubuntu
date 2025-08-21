# Using * with the ls Command in Ubuntu
### What is `*` in Linux
In Linux, the `*` character is called a wildcard.<br>
It tells the shell:

>“Match any number of characters in the file or folder names.”

When combined with the `ls` command, `*` helps you list files that match a certain pattern.<br>

### Basic Usage
Open a terminal and go to the `tmp` directory in you `work` directory.<br>
Then create the following files:<br>
```
apple.txt banana.txt berry.txt book.pdf cat.png car.txt
```
Check what's inside the folder:<br>
```
ls
```
You will see:<br>
```
apple.txt  banana.txt  berry.txt  book.pdf  cat.png  car.txt
```

### Match All Files
Use `*` by itself:
```
ls *
```
It matches everything in the folder.<br>

### Match Files Starting with Certain Letters
- If you want only files starting with b:<br>
```
ls b*
```
Result:<br>
```
banana.txt  berry.txt  book.pdf
```
### Match Files with Certain Extensions
- List only .txt files:<br>
```
ls *.txt
```
Result:<br>
```
apple.txt  banana.txt  berry.txt  car.txt
```
- List only .png files:<br>
```
ls *.png
```
Result:<br>
```
cat.png
```
### Match Files That Contain Certain Words
List files that have "an" in their names:<br>
```
ls *an*
```
Result:<br>
```
banana.txt
```
### Combine Characters
You can mix letters and `*` for more control.<br>
- List files starting with `b` and ending with `.txt`:<br>
```
ls b*.txt
```
Result:<br>
```
banana.txt  berry.txt
```
### No Match?
If no file matches, `ls` shows an error:<br>
```
ls z*
```
Result:<br>
```
ls: cannot access 'z*': No such file or directory
```
### Exercices
1. What is the command used to list files and directories starting with `net` in the `/etc` directory?
2. What is the command used to list files and directories ending with `.d` in the `/etc` directory?
3. What is the command used to list files with exstension `.txt` in the `/etc` directory?
4. If you are in `/etc`, what is the command you use to list files with `.conf` extension?
5. If you are in you home directory, what is the command you use to list files that starts with `su` and ending with `.confg`?
6. Send me a file that list all files ending with `*.conf` in the `/etc` directory.
7. What is the command that you used to copy all files ending with `*.txt` in the `~/work/note/ubuntu` to the `/tmp` directory?
8. If you are in `/etc`, what is the command used to list all hidden files in `/etc`?
9. If you are in `/etc`, what is the command used to list all hidden files in your home directory?
