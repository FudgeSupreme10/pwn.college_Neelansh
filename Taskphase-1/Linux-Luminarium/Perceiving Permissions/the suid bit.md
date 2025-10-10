# The SUID bit


<img width="1356" height="253" alt="image" src="https://github.com/user-attachments/assets/4a36847a-8cc5-4dcf-82ba-2aa3d8769c8b" />

As Seen above suid can be set using `chmod u+s [program]` command.

## My solve

Flag : `pwn.college{s25dpB-89tV_Q2p0dDenHLDUf_c.QXzEjN0wCM0gjNzEzW}`

in this we have to add the SUID bit to the `/challenge/getroot` program in order to spawn a root shell for us to `cat` the flag.

```bash
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot 
hacker@permissions~the-suid-bit:~$ /challenge/getroot 
SUCCESS! You have set the suid bit on this program, and it is running as root! 
Here is your shell...
root@permissions~the-suid-bit:~# cat 
.ICEauthority  .cache/        .john/         .local/        Desktop/       a              hello          leap/          not-the-flag   pwn            
.bash_history  .config/       .lesshst       COLLEGE        PWN            f              instructions   myflag         output.txt     the-flag       
root@permissions~the-suid-bit:~# cat 
.ICEauthority  .cache/        .john/         .local/        Desktop/       a              hello          leap/          not-the-flag   pwn            
.bash_history  .config/       .lesshst       COLLEGE        PWN            f              instructions   myflag         output.txt     the-flag       
root@permissions~the-suid-bit:~# cat not-the-flag 
pwn.college{s25dpB-89tV_Q2p0dDenHLDUf_c.QXzEjN0wCM0gjNzEzW}
root@permissions~the-suid-bit:~# cat /flag 
pwn.college{s25dpB-89tV_Q2p0dDenHLDUf_c.QXzEjN0wCM0gjNzEzW}
root@permissions~the-suid-bit:~# 
```
