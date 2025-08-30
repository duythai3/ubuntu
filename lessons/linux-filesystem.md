# __Learning the Linux Filesystem__

---

## __1. Welcome to the World of Linux Files__

Hello! Today, we’re going to explore one of the most important parts of Linux: the filesystem.

Think of your computer as a __giant library__:

- Each shelf is a __directory__ (or folder).
- Each book is a __file__.
- The __filesystem__ is the map that tells you where every book is stored.

In Linux, __everything__ is a file — not just documents and pictures, but even your keyboard, mouse, and programs!

---

## __2. The Big Map — / (Root Directory)__
In Linux, the entire filesystem starts from one main place:  
This slash is called root. It’s like the “city center” of your computer.

Here’s a simple map of the most important places:

```
 /
├── bin     → Basic programs (tools you always need)
├── etc     → System settings (configuration files)
├── home    → Personal space for each user
├── tmp     → Temporary files (disappear after restart)
├── var     → Changing data (logs, caches)
├── usr     → Extra programs and files
├── dev     → Devices (keyboard, hard drive, etc.)
└── proc    → Info about running programs
```

💡 Remember: In Linux, directory names are case-sensitive. `/Home` is not the same as `/home`.

---

## __3. Moving Around the Filesystem__
To explore Linux, you use the Terminal.  
The Terminal is like a magic door — you type commands and it shows you results.  

__Commands to move around__
- pwd — Show where you are (print working directory).
- ls — List files and folders in the current place.
- cd folder_name — Go into a folder.
- cd .. — Go up one level.
- cd /path/to/place — Go directly to a location.  

__Try it!__   
1. Open Terminal.
2. Type:

```
pwd
ls /
cd /home
pwd
cd ..
pwd
```

3. Look at the output — can you see where you are at each step?

## __4. Looking Inside Files__
Some files are text files that you can read in the Terminal.  
Useful commands

- `cat file.txt` — Show the whole file.
- `less file.txt` — Scroll through the file (press q to quit).
- `file something` — Tell what type of file it is.

Try it!
```
# Go to /etc:
cd /etc
ls
# Did you see your computer’s hostname?
cat hostname
```
## __5. Creating and Removing Files & Folders__ 
⚠ Warning: Only create and delete files in your home folder for now.
This keeps the system safe.  
Creating
- `mkdir folder_name` — Make a folder.
- `touch file.txt` — Make a blank file.
- `echo "text" > file.txt` — Make a file with text.
Removing
- `rm file.txt` — Delete a file.
- `rm -r folder_name` — Delete a folder and its contents.
Try it!
```
cd ~
mkdir playground
cd playground
touch hello.txt
echo "I am learning Linux!" > hello.txt
cat hello.txt
rm hello.txt
```
## __6. Understanding Paths__
A path tells Linux where something is.  
__Absolute path — The full address from /:__
```
	/home/toan/playground/hello.txt
```
__Relative path__ — From where you are now:  
If you’re in /home/toan, the same file can be:
```
	playground/hello.txt
```
__Try it!__  
- Draw a “map” of your home folder on paper.
- Mark where you are.
- Write one absolute and one relative path for the same file.
## __7. Fun Treasure Hunt__
Your mission: Create a “treasure map” on your computer.
1. Go to /tmp:  
```
cd /tmp
```
2. Make a folder called treasure_chest:  
```
mkdir treasure_chest
```

```
cd treasure_chest
```
3. Make a file called map.txt with the text:  
```
echo "X marks the spot!" > map.txt
```
4. Read the map:  
```
cat map.txt
```

## __8. Quick Recap__
- Filesystem = map of where files are stored.  
- `/` is the root (starting point).  
- You move with cd, see where you are with pwd, and list with ls.  
- You can make files/folders with touch/mkdir and remove them with rm.  
- Paths can be absolute or relative.  
## __9. Challenge Yourself__
1. Find the passwd file in /etc (it’s not a password list — it’s a list of users!).
2. Go to your home folder and create a directory named projects.
3. Inside projects, create a file named my_notes.txt with your favorite Linux command written inside.
4. Read your file to check if it worked.
