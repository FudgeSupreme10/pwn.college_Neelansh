# Split-piping stderr and stdout

In this challenge we have to apply our previouly learned knowledge to get the stout of the `/challenge/hack` to `/challenge/planet` and the stderr of `/challenge/hack` to `/challenge/the`, simultaneously.

## My Solve 

Flag : `pwn.college{U7MPTnfX7CcOxdYR9TPPCewqiLE.QXxQDM2wCM0gjNzEzW}`

To do this we use the previously learnt FD and redirect it to the commands using `proccess substitution`.

<img width="777" height="99" alt="image" src="https://github.com/user-attachments/assets/80d47eb6-6d3d-44b7-9b13-afe005eed7d8" />
