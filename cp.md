# Learning the cp Command in Ubuntu
### 1. What is `cp`?
The cp command in Linux/Ubuntu is used to copy files and directories.
Think of it like "copy & paste" on Windows or macOS, but in the terminal.
### 2. Basic Syntax
```
cp [options] source destination
```
- **source** = the file or folder you want to copy

- **destination** = where you want to put the copy

- **options** = extra instructions (like "copy folders" or "ask before overwriting")
### 3. Simple Examples
#### a) Copy a file in the same folder
```
cp file1.txt file1_copy.txt
```
This creates a copy named `file1_copy.txt`.
#### b) Copy a file into another folder
```
cp file1.txt /home/toan/Documents/
```
This copies `file1.txt` into the`Documents` folder.
#### c) Copy multiple files at once
```
cp file1.txt file2.txt /home/toan/Desktop/
```
Copies both files to the Desktop.
### 4. Copying Folders
By default, `cp` only works on files.
To copy a folder (with everything inside), add the `-r` (recursive) option:
```
cp -r my_folder/ /home/toan/Documents/
```
### 5. Useful Options
- `-i` → Interactive (asks before overwriting a file)
```
cp -i file1.txt file2.txt
```
- `-v` → Verbose (shows what’s happening)
```
cp -v file1.txt /home/toan/Desktop/
```
- `-u` → Update (only copies if the source is newer)
```
cp -u notes.txt backup/
```
### Practice Exercises
- [ ] Run commands below to create files and directories for practicing:
```
# change to your home directory
cd ~
# create a directory to store files and directories for learning Linux/Ubuntu
mkdir learn
# create a directory to contain temporary files & folders
mkdir learn/tmp
# change to ~/learn/tmp directory
cd learn/tmp
# create files for practice `cp` command
echo "file1" > file1.txt
echo "file2" > file2.txt
```
- [ ] Copy `file1.txt` to `file_copy.txt`
- [ ] Copy `file1.txt` to `/tmp`
- [ ] Copy `file1.txt` and `file2.txt` to `/tmp` by using one `cp` command
- [ ] List all files and folders in `/etc` and save the result to `/tmp/etc_file.txt`
- [ ] Copy `/tmp/etc_file.txt` to `~/learn/tmp` folder
- [ ] Copy the `~/learn/tmp` directory to the `/tmp` directory
- [ ] Run the command below and tell me what you see, and why you see the message:
```
cp -i file1.txt file1_copy.txt
```
- [ ] Run the command below and tell me what you see, and why you see the message:
```
cp -v file1.txt file1_copy_2.txt
```
- [ ] Run the command below and tell me what you see, and why you see the message:
```
cp -vu file1.txt file1_copy_2.txt
```
- [ ] Attach the `~/learn/tmp/etc_file.txt` to an email and send it to me
> I have also installed `thunderbird` on the math computer
