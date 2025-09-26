# Searching for Manuals

In this challenge we learn that the man page for challenge command is hidden under a different name, so now we need to find it by finding where the searchable database for the man is and how to access it. To do this we must go through the manpage of the `man` command.

## My Solve

Flag - `pwn.college{UFWnNwnqov4UGxwICElFHsxQwRZ.QX2EDO0wCM0gjNzEzW}`

<img width="1274" height="58" alt="image" src="https://github.com/user-attachments/assets/e5d0d2bc-9fd1-4b4c-aedd-a3138842fd66" />

Upon Searching a bit we find that the `-k` arguement can be used to search for the hidden manpage. So by using `man -k /challenge/challenge` we discover the hidden man page command

<img width="735" height="105" alt="image" src="https://github.com/user-attachments/assets/9033ff0a-52a0-432e-a0c6-be6e5629dbb9" />
