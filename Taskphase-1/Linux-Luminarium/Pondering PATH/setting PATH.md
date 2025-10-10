# Setting PATH

In this module we learn how to add our own scripts to the path so we can call them using their barename.

## My Solve

Flag : `pwn.college{UHRfvCrxqDBDdW1upuTIN2odstC.QX1cjM1wCM0gjNzEzW}`

In this challenge we need to add scripts in `/challenge/more_commands` to the path and then run `/challenge/run` to get the flag.

```bash
Connected!                                                                        
hacker@path~setting-path:~$ PATH="/challenge/more_commands"
hacker@path~setting-path:~$ /challenge/run 
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{UHRfvCrxqDBDdW1upuTIN2odstC.QX1cjM1wCM0gjNzEzW}
hacker@path~setting-path:~$ 
```
