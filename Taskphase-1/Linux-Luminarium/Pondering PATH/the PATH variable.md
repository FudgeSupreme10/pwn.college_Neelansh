# The PATH variable

The system stores all the commands such as `ls` or `cd` in the PATH variable where it searches for it, but if we empty the path out, then it won't run, which can destroy our system.

## My Solve

Flag : `pwn.college{UNIdXKjDzssCl3gO211yhho-r1V.QX2cDM1wCM0gjNzEzW}`

in this challenge we need to stop `/challenge/run` from running rm to remove the flag, we can do this by emptying the PATH variable like shown below : 

```bash
Connected!                                                                        
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/
DESCRIPTION.md  run             
hacker@path~the-path-variable:~$ /challenge/
DESCRIPTION.md  run             
hacker@path~the-path-variable:~$ /challenge/run 
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{UNIdXKjDzssCl3gO211yhho-r1V.QX2cDM1wCM0gjNzEzW}
hacker@path~the-path-variable:~$ 
```
