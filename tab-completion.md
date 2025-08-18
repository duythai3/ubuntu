# Tab Completion on Ubuntu
### 1. What is Tab Completion?
When you type a command in a terminal, sometimes pressing **Tab** will fill in the rest of the word for you.<br>
This is called **tab completion**.<br>
It saves time, avoid typos, and help you discover commands or files without remembering the full names.
### 2. Trying Basic Completion
Open the terminal and type:
```
ech
```
Now press **Tab**<br>
You should see it complete to:
```
echo
```
because `echo` is a command on Ubuntu.
### 3. Completing File Names
Change to the `~/learn/tmp` directory:
```
cd ~/learn/tmp
```
Now type:
```
cat e
```
Press **Tab**. It should expand to:
```
cat etc_file.txt
```
If there are multiple macthes, Bash shows them all. Try:
```
cat file
```
Press **Tab** twice. You'll see:
```
file1_copy_2.txt  file1_copy.txt    file1.txt         file2.txt         file_copy.txt
```
### 4. Completing Commands
Bash can also suggest commands. Type:
```
ls --
```
Then press **Tab** twice.<br>
You will see a list of options (--all, --help, etc.). These are long-form `ls` options.<br>
>In the previous lesson, you have learned `-a`, `-h` options.
>- `--all` is the long-form of `-a`.
>- `--human-readable` is the long-form of `-h`.
This helps you discover what a command can do.
### 5. Practice Excercises
1. Type `ls --h`, press **Tab** twice. What do you see?
2. Type `ls --help`, press **Enter**. Tell me what the result is.
3. Tell me what is the long form for `-l` of the `ls` command.
4. Type `ls /e`, then press **Tab**. Tell me what happens after you press **Tab**.
5. Type `ls /etc`, then press **Tab**. Tell me what happened, and why.
6. Type `ls /etc`, then press **Tab** twice. What do you see on the command line? And why does Bash show that message?
7. Tell me the list of commands that begin with `cat` on Ubuntu.
8. Tell me the list of files that begin with `host` in `/etc` directory.
9. Tell me what the command `mv` does (\*).
