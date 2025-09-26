# Symbolic Links

In this module we learn about symbolic links, they basically link one file at a particular location to another file which can have a different name and has a different path as the file it's linking to.

## My Solve

Flag : `pwn.college{kHrJ4Q394Vbuxkryv8ml_gVB4-e.QX5ETN1wCM0gjNzEzW}`

<img width="618" height="284" alt="image" src="https://github.com/user-attachments/assets/d0f800d5-859e-4da0-b272-c61c97ad6f56" />

The challenge basically asked us to create a `symbolic link` of `/flag` to `/home/hacker/not-the-flag` and then we had to run the `/challenge/catflag` which was basically displaying out the contents of `~/not-the-flag`

