# scripting with default cases

Your if statements so far have handled specific cases, but what about everything else? That's where else comes in!

The else clause executes when the if condition is false:

```bash
if [ "$1" == "hello" ]
then
    echo "Hi there!"
else
    echo "I don't understand"
fi
```

## My solve

Flag : `pwn.college{MgxsWZ3G3-YeDMyjYz-q9wRSREZ.01NzMDOxwCM0gjNzEzW}`

For this challenge, write a script at /home/hacker/solve.sh that:

- Takes one argument
- If the argument is "pwn", output "college"
- For any other input, output "nope"

```bash
hacker@chaining~scripting-with-default-cases:~$ nano /home/hacker/solve.sh 
hacker@chaining~scripting-with-default-cases:~$ /challenge/run 
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{MgxsWZ3G3-YeDMyjYz-q9wRSREZ.01NzMDOxwCM0gjNzEzW}
hacker@chaining~scripting-with-default-cases:~$ cat /home/hacker/solve.sh 
#!/bin/bash

if [ "$1" == "pwn" ]
then
    echo "college"
else
    echo "nope"
fi
hacker@chaining~scripting-with-default-cases:~$ 
```
