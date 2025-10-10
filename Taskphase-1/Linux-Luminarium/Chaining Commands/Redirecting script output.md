## Redirecting script output

In this challenge we are supposed to input the commands into a shell script, pipe its output to another command which prints the flag.

## My Solve

Flag : `pwn.college{gUt5iLCjT5jJyjKyx-rquax0i3W.QX4ETO0wCM0gjNzEzW}`

In this level, we will practice piping (|) from your script to another program. Like before, you need to create a script that calls the /challenge/pwn command followed by the /challenge/college command, and pipe the output of the script into a single invocation of the /challenge/solve command!

```bash
hacker@chaining~redirecting-script-output:~$ (echo /challenge/pwn ;echo /challenge/college ) >> x.sh && bash x.sh | /challenge/solve 
Correct! Here is your flag:
pwn.college{gUt5iLCjT5jJyjKyx-rquax0i3W.QX4ETO0wCM0gjNzEzW}
hacker@chaining~redirecting-script-output:~$ 
```
