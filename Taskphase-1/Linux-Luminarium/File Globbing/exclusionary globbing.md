# Exclusionary Globbing

We know how to look for files matching with a letter, here we learn how to exclude files matching with a specific letter(s) provided. To do so we use `!` inside the `[]` (in newer versions `^` works instead of `!`).

## My Solve

Flag - `pwn.college{wV8BKM4dO_u-AHzJ2qSe3f_6TuO.QX2IDO0wCM0gjNzEzW}`

In this challenge we need to pass an argument with `/challenge/run` and filter out those files which do not start with the letters `p,w,n`, to do so is very simple all we have to do is pass a command `/challenge/run [!pwn]*` to get the flag

<img width="681" height="208" alt="image" src="https://github.com/user-attachments/assets/5a558436-ef69-4751-bafc-fcbeffb98eef" />
