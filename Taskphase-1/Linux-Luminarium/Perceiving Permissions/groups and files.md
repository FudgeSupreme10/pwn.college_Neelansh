# Groups and Files

Here we learn that group ownership can be changed with the `chgrp` (change group) command.

## My Solve

Flag : `pwn.college{I-K2v2m-m_kGFxSXqI9KGg5Wn9e.QXxcjM1wCM0gjNzEzW}`

In this level, I have made the flag readable by whatever group owns it, but this group is currently root. Luckily, I have also made it possible for you to invoke chgrp as the hacker user! Change the group ownership of the flag file, and read the flag.

<img width="524" height="383" alt="image" src="https://github.com/user-attachments/assets/fef72f10-faed-4c3d-8c13-acc1956d95eb" />
