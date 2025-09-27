# Matching With ?

In The Previous Module when working with `*`, it worked as a wildcard for a whole word but here the `?` is just a wildcard for a single letter.
For Example : if we have a file named as `file_crypto` and we use `cat file_*` that will open the file but if we did `cat file_?` that would not work instead we would have to do something like `file_?rypto` as it is a wildcard for only a single letter.

## My Solve

Flag - `pwn.college{ApxORTQecrcEuPXVznpQImnDxFM.QXyIDO0wCM0gjNzEzW}`

<img width="694" height="245" alt="image" src="https://github.com/user-attachments/assets/6e01992e-baf9-4339-ad99-f46f6aa7d16c" />

In the challenge we had to replace c and l with `?` to go to the `/challenge` directory and then run `/challenge/run` to get the flag.
