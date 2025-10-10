# Your First Shell Script

Here we learn how to run a shell script created by containing the output of both `/challenge/pwn` and `/challenge/college` into `x.sh`.

## My Solve

Flag : `pwn.college{47icOAY9rx0NfIgbPQnj_Sp3UEk.QXxcDO0wCM0gjNzEzW}`

In this challenge we should run /challenge/pwn and then /challenge/college, but this time in a shell script.

```bash
hacker@chaining~your-first-shell-script:~$ echo /challenge/pwn > x.sh ; echo /challenge/college >> x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh 
Great job, you've written your first shell script! Here is the flag:
pwn.college{47icOAY9rx0NfIgbPQnj_Sp3UEk.QXxcDO0wCM0gjNzEzW}
hacker@chaining~your-first-shell-script:~$ 
```
