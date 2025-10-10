# Process exit code

Every process that exits gives an exit code which a user could use to check if it has exited correctly or has given an error. To get the exit code we use `echo $?`.

## My Solve

Flag : `pwn.college{Y491_HGBs__CWABCYlB-l1b2Ekk.QX5YDO1wCM0gjNzEzW}`

In this challenge we need to get the exit code of `/challenge/get-code` and then pass it as an argument to `/challenge/submit-code` to get the flag.

<img width="632" height="171" alt="image" src="https://github.com/user-attachments/assets/364f0e99-cb2e-4a27-8533-ff887986b8ff" />
