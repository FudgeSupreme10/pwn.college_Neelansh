# Changing File Ownership

In this level we learn that each file has a specific owner, in pwn.college we are usually the `hacker` user, but some files can only get edited by the `root`, which is a hacker's ultimate goal to reach root privileges. We can change the ownership of a file using the `chown` command, which typically only the root user has access to.

## My Solve

Flag : `pwn.college{czWJxD0hup772v5AP4RcU73wMoh.QXxEjN0wCM0gjNzEzW}`

In this challenge we need to change the ownership of `/flag` from root to hacker using the `chown` command.

<img width="579" height="154" alt="image" src="https://github.com/user-attachments/assets/f7360a18-8a89-4bfe-89e6-db8494d8eaae" />

