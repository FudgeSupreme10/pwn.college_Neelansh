# Scripting with multiple conditions

You've learned how to use a single if statement to check a condition. But what if you need to check multiple conditions? You can use elif (short for else if)

## My Solve

Flag : `pwn.college{MAW_fk8UwX6WPhBkrEZ6QJ-NYDl.0FOzMDOxwCM0gjNzEzW}`

Like previously challenges we are given with a set of arguments that if meet print a certain word, the solution is given below

```bash
hacker@chaining~scripting-with-multiple-conditions:~$ nano /home/hacker/solve.sh 
hacker@chaining~scripting-with-multiple-conditions:~$ cat /home/hacker/solve.sh 
#!/bin/bash

if [ "$1" == "hack" ]
then
    echo "the planet"
elif [ "$1" == "pwn" ]
then
    echo "college"
elif [ "$1" == "learn" ]
then
    echo "linux"
else
    echo "unknown"
fi
hacker@chaining~scripting-with-multiple-conditions:~$ /challenge/run 
Correct! Your script properly handles all the conditions with elif.
Here's your flag:
pwn.college{MAW_fk8UwX6WPhBkrEZ6QJ-NYDl.0FOzMDOxwCM0gjNzEzW}
hacker@chaining~scripting-with-multiple-conditions:~$ 
```
