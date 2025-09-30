# Duplicating Piped data with tee

The `tee` command is a very useful command to debug the data as well as writing to 2 seperate files at the same time.

## My Solve

Flag : `pwn.college{AZ8T8erAwTF4PgsPOXcvBFkkRDg.QXxITO0wCM0gjNzEzW}`

In this challenge we have we use tee to intercept pwn and get its secret code and pipe it into /challenge/college and then `cat pwn` to get the secret code and then to use the secret code like shown below to get the flag.

<img width="737" height="259" alt="image" src="https://github.com/user-attachments/assets/bbd19097-ec44-4d01-8740-c70d8bf3ed92" />
