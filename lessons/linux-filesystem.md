#Learning the Linux Filesystem

1. Welcome to the World of Linux Files
Hello! Today, we’re going to explore one of the most important parts of Linux: the filesystem.
---
Think of your computer as a giant library:
- Each shelf is a directory (or folder).
- Each book is a file.
- The filesystem is the map that tells you where every book is stored.

In Linux, everything is a file — not just documents and pictures, but even your keyboard, mouse, and programs!

2. The Big Map — / (Root Directory)
In Linux, the entire filesystem starts from one main place: /
This slash is called root. It’s like the “city center” of your computer.
Here’s a simple map of the most important places:
 /
├── bin     → Basic programs (tools you always need)
├── etc     → System settings (configuration files)
├── home    → Personal space for each user
├── tmp     → Temporary files (disappear after restart)
├── var     → Changing data (logs, caches)
├── usr     → Extra programs and files
├── dev     → Devices (keyboard, hard drive, etc.)
└── proc    → Info about running programs

💡 Remember: In Linux, directory names are case-sensitive. /Home is not the same as /home.
3. Moving Around the Filesystem
To explore Linux, you use the Terminal.
The Terminal is like a magic door — you type commands and it shows you results.
Commands to move around
    • pwd — Show where you are (print working directory).
    • ls — List files and folders in the current place.
    • cd folder_name — Go into a folder.
    • cd .. — Go up one level.
    • cd /path/to/place — Go directly to a location.
Try it!
    1. Open Terminal.
    2. Type:
       	pwd
       	ls /
       	cd /home
       	pwd
       	cd ..
       	pwd
    3. Look at the output — can you see where you are at each step?

4. Looking Inside Files
Some files are text files that you can read in the Terminal.
Useful commands
    • cat file.txt — Show the whole file.
    • less file.txt — Scroll through the file (press q to quit).
    • file something — Tell what type of file it is.

Try it!
    • Go to /etc:
	cd /etc
	ls
	cat hostname
    • Did you see your computer’s hostname?

5. Creating and Removing Files & Folders
⚠ Warning: Only create and delete files in your home folder for now.
This keeps the system safe.
Creating
    • mkdir folder_name — Make a folder.
    • touch file.txt — Make a blank file.
    • echo "text" > file.txt — Make a file with text.
Removing
    • rm file.txt — Delete a file.
    • rm -r folder_name — Delete a folder and its contents.
Try it!
	cd ~
	mkdir playground
	cd playground
	touch hello.txt
	echo "I am learning Linux!" > hello.txt
	cat hello.txt
	rm hello.txt
6. Understanding Paths
A path tells Linux where something is.
Absolute path — The full address from /:
	/home/toan/playground/hello.txt
Relative path — From where you are now:
If you’re in /home/toan, the same file can be:
	playground/hello.txt
Try it!
    • Draw a “map” of your home folder on paper.
    • Mark where you are.
    • Write one absolute and one relative path for the same file.
7. Fun Treasure Hunt
Your mission: Create a “treasure map” on your computer.
    1. Go to /tmp:
	cd /tmp
    2. Make a folder called treasure_chest:
	mkdir treasure_chest
	cd treasure_chest
    3. Make a file called map.txt with the text:
       echo "X marks the spot!" > map.txt
    4. Read the map:
       cat map.txt

8. Quick Recap
    • Filesystem = map of where files are stored.
    • / is the root (starting point).
    • You move with cd, see where you are with pwd, and list with ls.
    • You can make files/folders with touch/mkdir and remove them with rm.
    • Paths can be absolute or relative.
9. Challenge Yourself
    1. Find the passwd file in /etc (it’s not a password list — it’s a list of users!).
    2. Go to your home folder and create a directory named projects.
    3. Inside projects, create a file named my_notes.txt with your favorite Linux command written inside.
    4. Read your file to check if it worked.
