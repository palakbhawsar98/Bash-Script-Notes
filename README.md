# Bash(Bourne Again Shell) 🐧

### What is Bash sripting
Bash stands for Bourne Again Shell. A Bash Shell Script is a plain text file containing a set of various commands that we usually type in the command line. It is used to automate repetitive tasks on Linux. To automate day to day automation task, system admins write bash script in Linux system.
Bash script has .sh extension but the extension is not mandatory.

### Advantages of Bash scripting
- Easy to use
- Time saving
- Automated
- Can be installed on all Linux system
- Portable
- Can run multiple commands

### First Bash script
Bash script starts with **#!** referred as the shebang followed by **/bin/bash** it actually tells the path of the interpreter to execute the commands in the script.

**echo**: echo is a built-in command in Bash, which is used to display the standard output by passing the arguments. It is the most widely used command for printing the lines of text/String to the screen.

### To Run bash use 
```
 bash script_name.sh
 OR
./script_name.sh
 
```

### Script to print Hello Wrld!
```
#!/bin/bash
echo "******************"
echo "Hello World!"
echo "******************"
```
### After execution

![image](https://user-images.githubusercontent.com/69889600/218807819-e1b42e78-0ec8-4d7c-8406-2fbc2a5dd229.png)

### Single line comment in bash use [**#**]

![image](https://user-images.githubusercontent.com/69889600/218809940-a93d1325-e79e-4bdc-a6d8-3191ea3d4224.png)

### After execution

![image](https://user-images.githubusercontent.com/69889600/218807819-e1b42e78-0ec8-4d7c-8406-2fbc2a5dd229.png)

### Multiple line comment in bash use [: ' commented text  ']

![image](https://user-images.githubusercontent.com/69889600/218812434-edc051c9-7492-4b3d-94de-4c330a00990c.png)

### After execution

![image](https://user-images.githubusercontent.com/69889600/218812563-d1abbd60-109a-450a-812e-1070737f7437.png)

### Variables
Variables are used to store information.

## To store information use below syntax

```

```
```
echo $variable-name
```
Set variable user="john"
```
echo $user ---> john
```
Print environment variables
```
echo "This is user ${user} in the team"
```
Use back tick ` ` to print output of the command
```
 echo "There are `wc -l > hello.txt` files in media directory"
```

### Bash commands

Find shell in the terminal
```
echo $shell
```
Ping in the terminal
```
ping ip-address/domain-name/
```
Print "Hello world" in terminal
```
echo "Hello World"
```
Redirecting output > will override >> will append
```
echo "Hello World" > hello.txt ----> Hello World
echo "Welcome," > hello.txt ------> Welcome,
echo "How are you?" >> hello.txt ------> Welcome, How are you?
```
Count number of lines in file
```
wc -l > hello.txt
cat hello.txt | wc -l
```
Conditiona AND && ---- both condition should be true
```
cat hello.txt && echo "Successful"
```
Conditiona OR || ---- Any one condition should be true
```
cat hel.txt || echo "Successful"
```


- $? ---- Exit status of last run command, 0 means success and anything else indicates failure.
- $0 ---- File name of our script
- $1..$n ---- Script arguements
- $# ----- number of args that our script was run with

