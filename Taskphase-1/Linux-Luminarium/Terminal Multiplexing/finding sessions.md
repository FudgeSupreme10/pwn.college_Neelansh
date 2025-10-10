# Finding Sessions

If we have multiple screens, we can check which screen to reattach to using `screen -ls`.

## My Solve

Flag : `pwn.college{cF7ViZssYlKqrd6ZxEtE7fcqnk2.01N4IDOxwCM0gjNzEzW}`

In this challenge i have to find the screen which has the flag from the 3 available screens

```bash
hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
        144.session_b83ac15939dd5664    (Detached)
        147.session_bfb2f537a117464a    (Detached)
        150.session_338e9e51de8dee42    (Detached)
3 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 144
[detached from 144.session_b83ac15939dd5664]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 147
[detached from 147.session_bfb2f537a117464a]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r 150
[detached from 150.session_338e9e51de8dee42]
hacker@terminal-multiplexing~finding-sessions:~$ 
```
