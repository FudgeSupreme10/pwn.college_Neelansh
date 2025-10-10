# Extracting specific sections of text

In this module we learn how to extract specific columns of data like the first, third or even the 69th column. We can accomplish this using `cut`.

## My Solve

Flag : `pwn.college{QZsmzpZ7BFZn6JTVWgL__ETZQAw.01NxEzNxwCM0gjNzEzW}`

In this challenge, the `/challenge/run` program will give you a bunch of lines with random numbers and single characters (characters of the flag) as columns. Use `cut` to extract the flag characters, then pipe them to `tr -d "\n"`

<img width="973" height="91" alt="image" src="https://github.com/user-attachments/assets/df1df226-6693-4c64-9ee4-443538e66afe" />
