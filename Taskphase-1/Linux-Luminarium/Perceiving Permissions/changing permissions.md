# Changing Permissions

In this module we learn each file has permissions like here below : 
```bash
-rw-r--r-- 1 hacker hacker    0 May 22 13:42 college_file
```
as seen college_file has `r`ead,`w`rite permissions with user who owns the file (hacker), and has only `r`ead permission with group owner (hacker) and has only `r`ead permission with everyone else.
We can change this using `chmod` command.

## My Solve

Flag : `pwn.college{Y0K1P-y6LyOMbZCnLa0odN6uIof.QXzcjM1wCM0gjNzEzW}`

In this challenge we have to change permission of `/flag` file so that anyone can read it as it is owned by root user and group. To do this we will user the following command `chmod o+r /flag` to change it's permissions, usually chmod can only be executed by those who have execute permission of the file, but here we are allowed to for the challenge.

```bash
hacker@permissions~changing-permissions:~$ ls -l /flag 
-r-------- 1 root root 60 Oct 10 15:55 /flag
hacker@permissions~changing-permissions:~$ chmod o+r /flag 
hacker@permissions~changing-permissions:~$ cat /flag 
pwn.college{Y0K1P-y6LyOMbZCnLa0odN6uIof.QXzcjM1wCM0gjNzEzW}
hacker@permissions~changing-permissions:~$ 
```
