# scripting with conditionals

In bash, you can use if statements to make decisions, such as : 
```bash
if [ "$1" == "ping" ]
then
    echo "pong"
fi
```

## My Solve

Flag : `pwn.college{A7yqB7jhTwzF5i9pLbjCUUYh9PA.0lNzMDOxwCM0gjNzEzW}`

For this challenge, write a script at /home/hacker/solve.sh that:
- Takes one argument
- If the argument is "pwn", output "college"
- For any other input, output nothing

```bash
hacker@chaining~scripting-with-conditionals:~$ nano /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{A7yqB7jhTwzF5i9pLbjCUUYh9PA.0lNzMDOxwCM0gjNzEzW}
hacker@chaining~scripting-with-conditionals:~$ cat /home/hacker/solve.sh 
#!/bin/bash

if [ "$1" == "pwn" ]
then
    echo "college"
fi
hacker@chaining~scripting-with-conditionals:~$ 
```
