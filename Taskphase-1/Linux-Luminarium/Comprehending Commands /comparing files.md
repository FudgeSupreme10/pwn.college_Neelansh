# Comparing Files

In This challenge we will learn what the `diff` command does. The `diff` command basically compares 2 files and tells us what is different in the 2 files because u can't just basically eyeball the differences in 2 hude files yourself.

## My Solve

So We were given with 2 files which both containes 100 same fake flags the 2nd file also contains one real flag we need to find the real flag using `diff` command

Flag : `pwn.college{w6RjGREkrH5jAU0fx0dDw_PErqD.01MwMDOxwCM0gjNzEzW}`

<img width="797" height="103" alt="image" src="https://github.com/user-attachments/assets/f04e5504-8cb0-43f5-ae11-1eee08f84460" />

Here we see the `diff` command give us the real flag by comparing the 2 files instantly.
Let us analyse what `55a56` means here, it basically means that after line 55 in first file it adds line 56 of file 2 (this basically means that there is an extra line in file 2 after line 55)
