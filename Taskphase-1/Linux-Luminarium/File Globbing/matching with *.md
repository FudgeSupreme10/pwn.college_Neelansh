# Matching with *

Globbing is basically referencing a file without typing it all out. So now in this module we learn how to `glob` with `*`. A Command Shell when it encounters a `*`, it treats it as a wildcard and tries to match it with a file that fits the pattern.

## My solve

Flag - `pwn.college{Y01lMs6t9YzTX5tjsr6tfoUSmX7.QXxIDO0wCM0gjNzEzW}`

In this challenge we have to cd to `/challenge` directory without using more than 4 characters in `cd`, so to achieve that we use `cd /ch*` which will automatically try and match the pattern and find the file `challenge` as seen below

<img width="604" height="137" alt="image" src="https://github.com/user-attachments/assets/585472c0-0564-41ce-96a6-4ec4d665e03e" />

