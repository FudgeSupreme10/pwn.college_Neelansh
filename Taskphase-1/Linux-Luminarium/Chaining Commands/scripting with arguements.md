# Scripting with Arguements

Scripts become much more powerful when they can accept arguments

<img width="786" height="205" alt="image" src="https://github.com/user-attachments/assets/accb386a-5e61-40cf-a2c0-f6c4a45b8575" />

## My Solve

Flag : `pwn.college{QdTHbDpyqF4SeFvkXxh9gAu_Bfp.0VNzMDOxwCM0gjNzEzW}`

For this challenge we have to write a script `/home/hacker/solve.sh` that takes 2 arguments and outputs them in reverse order.

```bash
hacker@chaining~scripting-with-arguments:~$ nano /home/hacker/solve.sh
hacker@chaining~scripting-with-arguments:~$ nano /home/hacker/solve.sh
hacker@chaining~scripting-with-arguments:~$ chmod a+x /home/hacker/solve.sh 
hacker@chaining~scripting-with-arguments:~$ /challenge/run 
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{QdTHbDpyqF4SeFvkXxh9gAu_Bfp.0VNzMDOxwCM0gjNzEzW}
hacker@chaining~scripting-with-arguments:~$ cat /home/hacker/solve.sh 
#!/bin/bash

echo $2 $1
hacker@chaining~scripting-with-arguments:~$ 
```
