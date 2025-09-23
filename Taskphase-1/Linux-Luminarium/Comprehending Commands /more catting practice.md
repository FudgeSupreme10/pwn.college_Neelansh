# More Catting Practice

## My Solve

Flag : `pwn.college{IbgDE-BtvEHMKjtRlMQc_1byqHY.QXwITO0wCM0gjNzEzW}`

<img width="634" height="163" alt="image" src="https://github.com/user-attachments/assets/3c6a670f-a9fe-4ebe-b3f0-8d1fbf423fad" />

So In this challenge the flag was hidden at `/usr/include/elfutils/` and i couldn't just cd into the directory to cat the flag so instead i used it's full
absolute path to get the content of the flag as shown in the image above by using the following command `cat /usr/include/elfutils/flag`.
