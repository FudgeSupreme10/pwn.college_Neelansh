# Deleting Newlines

As we learned in the previous module `tr` could be used to delete a character, but here we learm that it can also delete newlines using the escape character `\n`.

## My Solve

Flag : `pwn.college{cyA8BRDCsAXUXMwtSuTIjNf4RqW.0VNxEzNxwCM0gjNzEzW}`

Our challenge here is to delete all the newlines present in the output of `/challenge/run` using the following command with help of `tr` : `/challenge/run | tr -d "\n"`

<img width="979" height="64" alt="image" src="https://github.com/user-attachments/assets/8d2b900e-4b3b-45a5-bc23-94185e175703" />
