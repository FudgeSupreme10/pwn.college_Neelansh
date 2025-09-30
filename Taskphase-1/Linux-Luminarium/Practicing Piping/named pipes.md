# Named Pipes

Here we learn how to create a FIFO which is basically a persistent named Pipe.

## My Solve

Flag : `pwn.college{sB0BXQmSJow35US9EuSOOc61Ydm.01MzMDOxwCM0gjNzEzW}`

in this challenge we were tasked with creating a FIFO at `/tmp/flag_fifo` and redirecting `/challenge/run` stdout to that FIFO so that reading from the FIFO reveals the flag.

First Terminal (redirecting output/writing) : 

<img width="583" height="232" alt="image" src="https://github.com/user-attachments/assets/99d2fe3a-f054-49b8-8c13-a1179d8c1a20" />

Other Terminal  (Reading) : 

<img width="544" height="166" alt="image" src="https://github.com/user-attachments/assets/e50a1cde-7925-46a4-b706-ba2ad6c98d37" />
