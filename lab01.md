# Lab 01; 20Sep Saturday

# 1. pwd - Present Working Directory

### Displays the full path of the current directory.

```bash
pwd
```

---

# 2. ls - List contents of the directory

### Lists the files and directories in the current directory.

```bash
ls
```

---

# 3. cd folder_name - Change Directory

### Moves into the specified folder (relative or absolute path).

```bash
cd folder_name
```

---

# 4. rmdir folder_name - Remove Directory

### Deletes an empty directory. It will fail if the directory has files or other directories in it.

```bash
rmdir folder_name
```

---

# 5. mkdir folder_name - Make Directory

### Creates a new directory with the specified name.

```bash
mkdir folder_name
```

---

# 6. cd .. - Go to the Parent Directory

### Moves one level up in the directory hierarchy.

```bash
cd ..
```

# 7. cd /home/administrator/Videos - Change to an Absolute Directory Path

### Changes the directory to the absolute path '/home/administrator/Videos'.

```bash
cd /home/administrator/Videos
```

---

# 8. cd ~/Music

### Changes the current directory to the `Music` directory located in the user's home directory.

```bash
cd ~/Music
```

---

# 9. rm -r parent_Folder_name / rm -rf parent_Folder_name

Removes a directory and its contents recursively.

- `rm -r parent_Folder_name` — deletes the folder and all its contents, prompting for confirmation if necessary.

- `rm -rf parent_Folder_name` — forcibly removes the folder and all its contents without prompting (use with caution).

```bash
rm -r parent_Folder_name
rm -rf parent_Folder_name
```

---

# 10 Creating and editing a text file

Commands to create, append, and view the contents of a text file named `first.txt`:

```bash
touch first.txt
echo "I am Ashraf" >> first.txt
cat >> first.txt
# Now you can type multiple lines:
I am ...
I wish ..
I like ..
# Press Ctrl+D to save and exit the input
cat first.txt
```

- `touch first.txt` — creates an empty file named `first.txt`.

- `echo "I am Ashraf" >> first.txt` — appends the text "I am Ashraf" to the file.

- `cat >> first.txt` — opens the file for appending text; type your lines and press `Ctrl+D` to finish.

- `cat first.txt` — displays the contents of the file.
