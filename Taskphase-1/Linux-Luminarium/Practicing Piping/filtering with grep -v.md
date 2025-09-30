# Filtering with grep -v

Previously we learned how to filter lines matching with the word we grepped, now here we learn how to filter out the lines matching those patters using `grep -v`

## My Solve

Flag : `pwn.college{MgPCrmCqXTXbQRHyv3rqedcYL_J.0FOxEzNxwCM0gjNzEzW}`

In this challenge we have to grep through the `/challenge/run` command's output but the issue is that the challenge has thousands of decoy flags, which we have to filter out using the word `DECOY` to get the flag.

<img width="505" height="84" alt="image" src="https://github.com/user-attachments/assets/6b4dd49a-12be-49e5-a6aa-77efcfa7742e" />
