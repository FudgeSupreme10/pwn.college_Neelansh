# Listing Files

In this challenge we learn about the `ls` command, which basically lists all the file in the current working directory if no argument is passed and lists files of the asked for directory if an argument is passed.
Such as just typing `ls` will list all the files and directories of the current working directory like in the image below

<img width="332" height="90" alt="image" src="https://github.com/user-attachments/assets/bef18fa4-2cbd-4ab8-bcef-cf353871fa74" />

And now putting an argument with the `ls` command like here `ls /challenge` will list the files/folders of `/challenge` directory

<img width="383" height="66" alt="image" src="https://github.com/user-attachments/assets/f5db4d04-2dd9-4801-91ad-9ddcc69197cc" />

## My Solve

Flag : `pwn.college{8mKpLCy5Nf16WDODWZ_16irrnQq.QX4IDO0wCM0gjNzEzW}`

Here when we do `ls /challenge` we find the flag is inside the `27581-renamed-run-29157` file. On Catting it we see it is an executable file.

<img width="586" height="78" alt="image" src="https://github.com/user-attachments/assets/2e4700e9-4d01-41e1-b4fd-b21e3f56539b" />

So using absolute path we run the file to get the flag

<img width="561" height="76" alt="image" src="https://github.com/user-attachments/assets/d7bed7dc-79f2-4418-bb89-efaf4780e9ea" />
