# Detaching and Reattaching

we can detach and reattach a screen if we ever lose connection, this helps prevent work loss and is not possible without a screen.

You detach by pressing `Ctrl-A and then d` and can reattach using `screen -r`

## My Solve

Flag : `pwn.college{8xs1GJ0BGwc86RuR2UnzVs2oeCS.0lN4IDOxwCM0gjNzEzW}`

For this challenge we need to launch a screen and then detach from it and then run `/challenge/run` and the reattach the screen to get the flag.

```bash
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen
[detached from 172.pts-0.terminal-multiplexing~detaching-and-attaching]
hacker@terminal-multiplexing~detaching-and-attaching:~$ /challenge/run
Found detached screen session: 172.pts-0.terminal-multiplexing~detaching-and-attaching
Sending flag to your screen session...

Flag sent! Now reattach to your screen session with:

  screen -r

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching:~$ screen -r


hacker@terminal-multiplexing~detaching-and-attaching:~$
hacker@terminal-multiplexing~detaching-and-attaching:~$ echo Yes! Flag is: pwn.college{8xs1GJ0BGwc86RuR2UnzVs2oeCS.0lN4IDOxwCM0gjNzEzW}
Yes! Flag is: pwn.college{8xs1GJ0BGwc86RuR2UnzVs2oeCS.0lN4IDOxwCM0gjNzEzW}
hacker@terminal-multiplexing~detaching-and-attaching:~$
```

