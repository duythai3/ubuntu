# Understanding Paths on Ubuntu
### What Is a Path?
A path tells the computer where a file or folder is located in the filesystem.<br>
Think of it like an address for files and folders.<br>
On Ubuntu (and other Linux systems), everything starts from the **root directory** `/`.<br>
Example structure:
```
/
├── home/
│   ├── toan/
│   │   ├── Documents/
│   │   ├── Pictures/
│   │   └── .bashrc
├── etc/
├── bin/
└── var/

```
### Absolute vs. Relative Paths
**Absolute Path**<br>
- Always starts with / (root).
- Shows the full address of the file or folder.
- Example:

```
/home/toan/work/note/nano.txt

```
**Relative Path**<br>
- Does not start with /.
- Describes a location relative to your current folder.
- Example:<br>
If you're currently in /home/toan, then:
```
work/note/todo.txt
```
is the **relative path** to the file.<br>

### Special Symbols in Paths
| Symbol | Meaning | Example |
|--------|---------|---------|
|.|Current directory|./script.sh runs a script in the current folder|
|..|Parent directory|../notes.txt goes up one folder|
|~|Your home directory|cd ~/Pictures|
### Exercises
1. If you are in `/etc` directory, what is the command that you use to open the `nano.txt` file by using the Nano editor.<br>
2. If you are in `~/work/note`, what is the command used to get the `size` and `last modified time` of `/etc/hostname`.<br>
3. If you are in `~/work/note`, what command do you use to write "Hello" to `/tmp/t1.txt`.<br>
4. If you are in `~`, how do you use `nano` to open the `nano.txt` file.<br>
5. If you are in `~`, how do you use `nano` to open the `.bashrc` file.<br>
6. If you are in `~/work/note`, how do you use `nano` to open the `.bashrc` file by using a **relative path**.<br>
7. If you are in `~/work/note`, how do you get the list of files in `~`.<br>
8. If you are in `~/work/note`, how do you change to `~/Documents` by using a **relative path**.<br>
9. Take notes for this lesson, and save them into `~/work/note/path.txt`. Only write important information that you need to remember to navigate in Ubuntu Filesystem.<br>
