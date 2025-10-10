# Executable Bash Scripts

Here we learn how to execute bash scripts without using `bash` command and making them execuable using `chmod`.

## My Solve

Flag : `pwn.college{wmX0js708b43E1B_MXPYFbKc9vw.QX0cjM1wCM0gjNzEzW}`

in this challenge we had to write a bash script that executes `/challenge/solve` without using `bash` command and making it executable using `chmod a=rwx x.sh` and then run it.

```bash
hacker@chaining~executable-shell-scripts:~$ echo "/challenge/solve" > x.sh
hacker@chaining~executable-shell-scripts:~$ chmod a=rwx x.sh 
hacker@chaining~executable-shell-scripts:~$ ./x.sh 
Congratulations on your shell script execution! Your flag:
pwn.college{wmX0js708b43E1B_MXPYFbKc9vw.QX0cjM1wCM0gjNzEzW}
hacker@chaining~executable-shell-scripts:~$ 
```
