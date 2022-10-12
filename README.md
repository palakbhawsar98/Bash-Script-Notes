# Bash

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

## Variables
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
### Run bash
```
 bash hello.sh
 ./hello.sh
 
```
- $? ---- Exit status of last run command, 0 means success and anything else indicates failure.
- $0 ---- File name of our script
- $1..$n ---- Script arguements
- $# ----- number of args that our script was run with

