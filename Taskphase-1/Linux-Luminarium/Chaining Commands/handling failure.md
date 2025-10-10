# Handling Failure

We previously learnt about `&&` command which runs if first command SUCCEEDS here it is just opposite `||` runs when first command FAILS.

## My Solve

Flag : `pwn.college{4xj3OQzT9PnmAq60jHhygk4WMC2.01M0MDOxwCM0gjNzEzW}`

In this challenge, you need to chain /challenge/first-failure and /challenge/second using the || operator.

```bash
hacker@chaining~building-on-success:~$ 
Connected!                                                                        
hacker@chaining~handling-failure:~$ /challenge/first-failure || /challenge/second 
Nice chaining! Flag: pwn.college{4xj3OQzT9PnmAq60jHhygk4WMC2.01M0MDOxwCM0gjNzEzW}
hacker@chaining~handling-failure:~$ 
```
