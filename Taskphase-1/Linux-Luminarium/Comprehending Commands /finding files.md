# Finding Files

Now we learn how to find files by specifying a certain criteria. To do this we use the `find` command.

## My Solve

Flag : `pwn.college{AwuqZjjpjWA3K_upz-r6Oppuz_o.QXyMDO0wCM0gjNzEzW}`

This challenge requires us to find a file named `flag` somewhere in the linux subsystem. To do this we use the following command `find / -name flag`. To break this command down, let me tell u what the 3 arguments do. The first argument `/` tells us to look in the whole subsystem `/` and the second parameter tells us to look by name.

<img width="925" height="825" alt="image" src="https://github.com/user-attachments/assets/d0b70505-00c4-4497-99ac-5e29aecd4360" />

Here we see it gave us multiple results so by going through them i found the flag.
