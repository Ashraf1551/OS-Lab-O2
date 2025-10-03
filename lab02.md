# 🐧 Your First Linux Shell Script: A Quick Guide 🚀

Here's a quick revision guide for our first shell programming lab.  
It covers creating a script, making it runnable, and a few basic commands.

---

## 1. Creating Your Script File

First, we need an empty file. The `touch` command is perfect for this.  
It creates a blank file with the name you give it.

```bash
touch hello.sh
```

This creates the file **hello.sh** in your current directory.  
The `.sh` extension tells us it's a shell script.

---

## 2. Writing the Script's Code

Now, open `hello.sh` in a text editor (like **nano**, **gedit**, or **VS Code**) and type the following:

```bash
#!/usr/bin/bash

echo "Hello World"
```

### Let's break this down:

- `#!/usr/bin/bash`: This special first line is called a **shebang**.  
  It tells the operating system which interpreter to use to run the commands in the file.  
  In this case, we’re telling it to use the **Bash shell**.

💡 **Pro Tip:**  
If you run this command in your terminal:

```bash
which bash
```

it will show you the exact path to the Bash program — usually `/usr/bin/bash`.  
That’s how we know what to write in the shebang!

- `echo "Hello World"`: The **echo** command prints whatever text you give it to the terminal.

---

## 3. Running the Script (and the First Error!)

To run a script in your current directory, use:

```bash
./hello.sh
```

When you first try this, you’ll likely see an error message like this:

```
bash: ./hello.sh: Permission denied
```

This is a security feature in Linux — by default, new files don’t have permission to be executed (run as a program).

---

## 4. Making the File Executable with chmod

We need to give our script **execute** permission.  
We do this with the `chmod` (**change mode**) command.

```bash
chmod +x hello.sh
```

### Here’s what that means:

- `chmod`: The command to change permissions.
- `+x`: Add (`+`) execute (`x`) permission.
- `hello.sh`: The file you are changing.

---

## 5. Running it Successfully! 🎉

Now that the script has the correct permissions, try running it again:

```bash
./hello.sh
```

✅ **Output:**

```
Hello World
```

---

## 6. Taking Input from the User with read

Scripts can also be interactive.  
The `read` command pauses the script and waits for the user to type something and press **Enter**.

Let’s make a new script, `user_input.sh`, to see how it works:

```bash
#!/usr/bin/bash

echo "What is your name?"
read user_name
echo "Hello, $user_name! Nice to meet you."
```

### Here’s the new stuff:

- `read user_name`: Reads the user's input and stores it in a variable called `user_name`.
- `$user_name`: The `$` sign is used to get the **value** stored inside a variable.

So,

```bash
echo "Hello, $user_name"
```

prints “Hello,” followed by whatever the user typed.

---

## 7. Bonus Command: What is `ls -all`?

Your teacher probably used:

```bash
ls -al
```

or

```bash
ls -l -a
```

This is a very common command to **see details about files** —  
it lists all files (including hidden ones) with detailed information like permissions, owner, size, and modification date.

---

🎯 **Happy Scripting!**

```bash
echo "Keep practicing and exploring Linux Shell 🚀"
```
