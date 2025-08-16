# Learning the ls command on Ubuntu
Hi Toan,\
Today, you will learn about the ls command on Ubuntu. This command helps you see what files and folders are inside the place (called a directory) where you are working.
## What is ls?
- ls means list.
- When you type ls in the terminal and press Enter, Ubuntu will show you the files and folders in the current directory.
### Example:
```
# change to you home directory, ~ is the alias for your home directory (/home/toan)
cd ~
# list files and folders in the current working directory
ls
```
You might see something like:
```
Desktop  Documents  Downloads  Music  Pictures  Videos
```
This means those folders exist in your home directory.

## Adding Options to ls
ls has options that change how it shows the files. You add an option with a dash (-).
- Show more details: ls -l
```
ls -l
```
This shows a long list with details (permissions, size, date, etc.).
- Show hidden files: ls -a
```
cd ~
ls -a
```
Now you will see files like .bashrc that are usually hidden.\
On Ubuntu, files starting with '.' are hidden files.
- Combine options: ls -la\
You can put options together:
```
ls -la
```
This shows everything with details.
- Sort by time: 
```
ls -lt
```
- Show files's size in human readable format: -h
```
ls -lah
```
This lists files by last modified time, newest first.
## Using ls with Paths
You don’t have to list the current directory only.\
You can also list another path:
```
# list files and folders in the system configuration directory
ls /etc
# list files and folders in /home/toan/Documents
ls ~/Documents
```
## 4. Exercises
Reminder: To save something to a file from command line, use '>' or '>>'
```
# save the result of ls command to /tmp/ls-result.txt
ls > /tmp/ls-result.txt
```

1. Send me through email the list of files and folders in your home directory\
Tip: use cat to show the content of a file, copy it by using mouse, and then pass it to email
2. Tell me how big the .bashrc file is in bytes
3. Tell me how big the .bashrc file is in human readable format
4. Tell me when the /etc/hostname file was last modified
5. Send me the content of /etc/hostname. Can you guest what it is?
6. Tell me what the command below does:
```
ls -lah /etc > /tmp/1.txt
```
7. Explain the command below:
```
ls -lah ~ >> /tmp/2.txt
```
