# Reading Shell Scripts

Here we learn how to read the shell script and find the password hardcoded inside the script to get the flag.

## My Solve

Flag : `pwn.college{sH8rXodX8baxrtIUBFMg6-zBVWS.0lMwgDOxwCM0gjNzEzW}`

First we read the script using `cat` and then use the password to get the flag as shown below : 

```bash
hacker@chaining~reading-shell-scripts:~$ cat /challenge/run 
#!/opt/pwn.college/bash

read GUESS
if [ "$GUESS" == "hack the PLANET" ]
then
        echo "CORRECT! Your flag:"
        cat /flag
else
        echo "Read the /challenge/run file to figure out the correct password!"
fi
hacker@chaining~reading-shell-scripts:~$ /challenge/run hack the PLANET
^C
hacker@chaining~reading-shell-scripts:~$ /challenge/run
hack the PLANET
CORRECT! Your flag:
pwn.college{sH8rXodX8baxrtIUBFMg6-zBVWS.0lMwgDOxwCM0gjNzEzW}
hacker@chaining~reading-shell-scripts:~$ 
```
