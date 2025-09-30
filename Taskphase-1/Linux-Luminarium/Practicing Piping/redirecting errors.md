# Redirecting Errors

In this module we learn how to redirect errors through piping using File Descriptors, We have already been using them without knowing about them. The common ones are : 
<img width="353" height="128" alt="image" src="https://github.com/user-attachments/assets/90ea966f-c437-4da5-8e89-7d3cb4e7ece4" />

Here we see that `1>` is for standard output and is the samething as `>`. To get the errors we use `2>`. We can also use multiple FDs in the same command aswell.

## My Solve

Flag : `pwn.college{UegoMmMahoMrfXsVjNNH0Yg_T2-.QX3YTN0wCM0gjNzEzW}`

In this challenge we are tasked with sending the error to `instructions` file and the output to `myflag` from the `/challenge/run` command, if done correctly the flag will be there in `myflag` file.

<img width="753" height="415" alt="image" src="https://github.com/user-attachments/assets/63f15c74-a27f-422f-b755-cc21c2bf05cc" />
