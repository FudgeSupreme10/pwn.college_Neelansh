# Finding Commands

here we learn the use of `which` command which looks for the command passed as an argument and finds it's path in $PATH.

## My Solve

Flag : `pwn.college{YIICvT1GxA9r3B6MEzZ9NNQ7uX_.01NzEzNxwCM0gjNzEzW}`

In this challlenge we need to find the path of `win` command then `cd` into it and then `cat` the flag file present inside it.

```bash
hacker@path~finding-commands:~$ which win
/challenge/paths/5307/win
hacker@path~finding-commands:~$ cdd /challenge/paths/5307/
bash: cdd: command not found
hacker@path~finding-commands:~$ cd /challenge/paths/5307/
hacker@path~finding-commands:/challenge/paths/5307$ ls
flag  win
hacker@path~finding-commands:/challenge/paths/5307$ cat flag 
pwn.college{YIICvT1GxA9r3B6MEzZ9NNQ7uX_.01NzEzNxwCM0gjNzEzW}
hacker@path~finding-commands:/challenge/paths/5307$ 
```
