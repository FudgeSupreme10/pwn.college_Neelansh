# Hijacking commands

Here like in the first task of this module `/challenge/run` will try and run the `rm` ,instead we can try and modify it to instead print the flag.

## My Solve

Flag : `pwn.college{Mzx1Kr4NRlRDOgiSRymmG4DvyTQ.QX3cjM1wCM0gjNzEzW}`

first we need to find the path of `cat` command and modify `rm` command to print /flag using cat command by the following method : 

```
hacker@path~hijacking-commands:~$ which cat
/run/dojo/bin/cat
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ chmod a=rwx rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{Mzx1Kr4NRlRDOgiSRymmG4DvyTQ.QX3cjM1wCM0gjNzEzW}
hacker@path~hijacking-commands:~$ 
```
