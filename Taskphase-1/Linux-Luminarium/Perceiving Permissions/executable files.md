# Executable Files

Previously we learnt how to change permission to read files, using the same process here we have to make a file executable.

## My Solve

Flag : `pwn.college{wbBsrXph0gn2Nd4l_SSdEWv2IhC.QXyEjN0wCM0gjNzEzW}`

In this challenge, the `/challenge/run` program will give us the flag, but we must first make it executable, we can do that using `chmod`, and get `/challenge/run` to output the flag.

```bash
hacker@permissions~executable-files:~$ chmod u+x /challenge/run 
hacker@permissions~executable-files:~$ /challenge/run 
Successful execution! Here is your flag:
pwn.college{wbBsrXph0gn2Nd4l_SSdEWv2IhC.QXyEjN0wCM0gjNzEzW}
hacker@permissions~executable-files:~$ ls -l /challenge/run 
-r-xr--r-x 1 hacker hacker 32 Jan 14  2025 /challenge/run
hacker@permissions~executable-files:~$ 
```
