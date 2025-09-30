# Appending Output

As we learned previously that `>` saves the output to the given file, but if we run it again and again to the same file it will rewrite the output everytime so to append the output instead of rewriting it, we use `>>` instead of `>`.

## My Solve

Flag : `pwn.college{Ixhlz7oY74-xsftjWOpO1qo3axK.QX3ATO0wCM0gjNzEzW}`

In this challenge we need to append the output of `/challenge/run` to `/home/hacker/the-flag` to get the flag, but if we rewrite the first half of the flag would not be saved anymore in the file.

<img width="884" height="562" alt="image" src="https://github.com/user-attachments/assets/3cc4b423-3e6d-4de8-935c-6a5eb7ba1ed2" />
