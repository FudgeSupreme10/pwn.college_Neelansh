# Bashrc Backdoor

In this module we learn that during startup linux executes the `.bashrc` file found in `/home/[user]/` directory, we as hackers could use this knowledge to modify it keep access of a system.

## My Solve

Flag : `pwn.college{4gJQEga6eCpFRB2ndD-jMF6pzDR.0VMzEzNxwCM0gjNzEzW}`

In this challenge, we have access to `Zardus`'s `.bashrc` file which we can use to read `/flag` accessible only to zardus. (To Simulate zardus logging in we need to run `/challenge/victim`).

```shell
hacker@shenanigans~bashrc-backdoor:~$ nano /home/zardus/.bashrc 
hacker@shenanigans~bashrc-backdoor:~$ /challenge/victim 
Username: zardus
Password: ***********
pwn.college{4gJQEga6eCpFRB2ndD-jMF6pzDR.0VMzEzNxwCM0gjNzEzW}
zardus@shenanigans~bashrc-backdoor:~$ exit
logout
hacker@shenanigans~bashrc-backdoor:~$ 
```
