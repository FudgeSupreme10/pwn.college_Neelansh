# Mixing Globs

This is a challenge module where we have to apply all we have previously learnt to get the flag. Our Job is to pass an argument in `/challenge/run` command like previously but it should 6 or less than 6 character long, and should cover the words `"challenging", "educational", and "pwning"`.

## My Solve

Flag - `pwn.college{w8LW--4YNHJqKBHrgHBJWExT3b0.QX1IDO0wCM0gjNzEzW}`

<img width="602" height="128" alt="image" src="https://github.com/user-attachments/assets/52c47d42-f9c8-43df-b499-44681e0e60de" />

Now we know that we have to use `[]` wildcard to get the `c,e,p` and also need to use `*` wildcard to complete the rest of the word. so if we combine this we get `[cep]*` which is an argument with only 6 characters and perfect for our challenge so we pass the following command to get the flag `/challenge/run [cep]*` to get the flag.
