# An Epic Filesystem Quest

This is a challenge which basically tests us on all the command we learned previously such as `ls`, `cat`, `cd`.

## My Solve

Flag : `pwn.college{wfki_192K2-FvnC-Q8uubztrAb5.QX5IDO0wCM0gjNzEzW}`

First we `cd` to the `/` directory as instructed. After going to `/` we use `ls` to list all the files.

<img width="1224" height="52" alt="image" src="https://github.com/user-attachments/assets/1d40a57d-5307-4e04-b4ea-c111414641b8" />

Now we see a File Called `REVELATION` so we read it using `cat`.

<img width="1171" height="84" alt="image" src="https://github.com/user-attachments/assets/e763f8aa-8b94-4fde-aefa-2f3157026d16" />

 Now we see the next clue is in `/opt/linux/linux-5.4/drivers/block`. but it also says u can't cd to it to read, so by using `ls` we find the file which contains the next clue.

 <img width="1511" height="92" alt="image" src="https://github.com/user-attachments/assets/2b9a09c6-99de-43cb-beec-90a29907b1c9" />

Here we See file Called `WHISPER-TRAPPED`, this must be it, the file we are looking for so as we can't cd into the directory we `cat` the file using it's `absolute path`.

<img width="1072" height="113" alt="image" src="https://github.com/user-attachments/assets/de9dd940-9841-4498-bbae-325b7a6aaf56" />

That worked now we see that the next clue is in `/usr/share/racket/pkgs/gui-lib/scribble/private/compiled` and is hidden. So using `ls -a /usr/share/racket/pkgs/gui-lib/scribble/private/compiled` we find our file.

<img width="867" height="57" alt="image" src="https://github.com/user-attachments/assets/4bcf83f5-f6f8-43f1-9293-44cd3a20f97f" />

Now we see the `.SPOILER` file, so i read it using `cat` and we find our next clue.

<img width="918" height="96" alt="image" src="https://github.com/user-attachments/assets/baf48384-2c25-4267-9041-196ada845121" />

According to this our next clue is in `/usr/share/racket/pkgs/parser-tools-lib/parser-tools/examples/compiled` and which won't become readable until and unless we `cd` into the directory.

So after changing our directory to ` cd /usr/share/racket/pkgs/parser-tools-lib/parser-tools/examples/compiled`, we find the next Clue File named `LEAD`, on `catting` the file, we find our next clue

<img width="990" height="108" alt="image" src="https://github.com/user-attachments/assets/82467a01-8d24-45fe-8747-a828ad2d9a3d" />

Now after doing the same thing over and over again, we finnaly get the flag

<img width="1731" height="731" alt="image" src="https://github.com/user-attachments/assets/c9003dc1-819a-4270-969f-239ee9948732" />

