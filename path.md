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
