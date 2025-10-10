# Building On Success

In previous module we learned that every process exits with a exit code, so here we use `&&`, which will only run the 2nd command if the first command succeeds (exits with exit code 0).

## My Solve

Flag : `Flag: pwn.college{0GDRhl0jDiX7uWry7-8TdWDdXYK.0lM0MDOxwCM0gjNzEzW}`

In this challenge, you need to chain the programs /challenge/first-success and /challenge/second using the && operator.

```bash
hacker@chaining~building-on-success:~$ /challenge/first-success 
hacker@chaining~building-on-success:~$ /challenge/second 
Error: /challenge/first-success must be successfully chained with 
/challenge/second using &&
hacker@chaining~building-on-success:~$ /challenge/first-success && /challenge/second 
Nice chaining! Flag: pwn.college{0GDRhl0jDiX7uWry7-8TdWDdXYK.0lM0MDOxwCM0gjNzEzW}
hacker@chaining~building-on-success:~$ 
```
