# Matching with []

In this module we learn about using the `[]` brackets, what these essentially do is similar to `?` wildcard but instead of just looking for any character we define the character we want to look.
*Like for Example* - If We Have three files in a directory `file_a`,`file_b`,`file_c`, and we only want to look for specific files like `a,b` so we could do something like `ls file_[ab]`, this would display the files within that subset i.e. `file_a`,`file_b`

## My Solve

Flag : `pwn.college{wLqatJQjOAT_G4JTmK3YlIbpEZO.QXzIDO0wCM0gjNzEzW}`

<img width="617" height="151" alt="image" src="https://github.com/user-attachments/assets/9fe6d1ad-ad2f-4b90-9c82-eccaeefbbf1d" />

As We Can see in the image below we had multiple files present in the `/challenge/files` folder from that we had to run a command `/challenge/run file_[bash]` to get the flag and to only find the 4 mentioned files as per the challenge.
