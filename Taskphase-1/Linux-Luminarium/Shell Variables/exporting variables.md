# Exporting Variables

As we know the variables we use are temporary and do not carry over a child shell, to carry them over we could use the `export` command.

## My Solve

Flag : `pwn.college{MfA9KOeBMCM0eb8-TZckNxfmrX6.QXyYTN0wCM0gjNzEzW}`

In this challenge we must invoke /challenge/run with the PWN variable exported and set to the value COLLEGE, and the COLLEGE variable set to the value PWN but not exported. To do this we follow the steps in the image below.

<img width="578" height="202" alt="image" src="https://github.com/user-attachments/assets/1d5d3739-2a71-43d1-87dc-0bcfe5e3f43e" />
