# Cracking Passwords

Previously passwords were stored with the usernames in `/challenge/passwd`, but now due to safety concerns they are stored in `/etc/shadow` which is only accessible by root user and have been encrypted in the form of hashes.

## My Solve

Flag : `pwn.college{EMtD2EZstSrqvoWF2Icw1N4afr9.QX3UDN1wCM0gjNzEzW}`

Our task in this challenge is to crack the password of `Zardus` user using `John the Ripper` tool and then switch to `zardus` and run `/challenge/run` to get the flag.

<img width="634" height="245" alt="image" src="https://github.com/user-attachments/assets/409af5b0-93b5-4d16-9e37-fc1fc4a86062" />
