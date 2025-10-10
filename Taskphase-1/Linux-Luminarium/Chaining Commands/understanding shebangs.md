# Understanding Shebangs

When a program is invoked in Linux, the Linux kernel first inspects the file to determine how it should be run. This does NOT use the extension (which is why you don't have to name your shell scripts with a .sh extension, or your Python scripts with a .py extension, or so on). Rather, Linux looks at the first few bytes of the file for this information.

Like in a linux bash script it sees `#!` which is often refered to as a shebang, so it treats it as a program and then `/bin/bash` is used to identify it is a bash script.

## My Solve

Flag : `pwn.college{gsNIumLRB4SWsiPAa4x0DoPZmD3.0VOzMDOxwCM0gjNzEzW}`

For this challenge, create a script at /home/hacker/solve.sh that has a proper shebang and outputs "hack the planet". Remember to make it executable, then run /challenge/run to verify your script works correctly!

```bash
hacker@chaining~understanding-shebangs:~$ nano /home/hacker/solve.sh
hacker@chaining~understanding-shebangs:~$ /challenge/run 
Error: /home/hacker/solve.sh is not executable!
Hint: Use 'chmod' to make it executable
hacker@chaining~understanding-shebangs:~$ chmod a+x /home/hacker/solve.sh 
hacker@chaining~understanding-shebangs:~$ /challenge/run 
Testing your script...
Perfect! Your flag:
Flag: pwn.college{gsNIumLRB4SWsiPAa4x0DoPZmD3.0VOzMDOxwCM0gjNzEzW}

hacker@chaining~understanding-shebangs:~$ 
```
