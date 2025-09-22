This module will teach you the basics of Linux file paths, like how to ponder about different paths and 

# Challenges

## The Root

Flag : `pwn.college{s3Arx7VrQxCrhRuNrakxTVi-K5o.QX4cTO0wCM0gjNzEzW}`

<img width="479" height="84" alt="image" src="https://github.com/user-attachments/assets/2e9250ab-d596-4fed-b002-d67aed0998bc" />

We use absolute paths to execute /pwn to execute the file and get the flag

## Program and Absolute Path

Flag : `pwn.college{4XzDHYb2Hmx6aAARHUPJ0jywDtO.QX1QTN0wCM0gjNzEzW}`

<img width="495" height="102" alt="image" src="https://github.com/user-attachments/assets/deff59b8-7bce-4fd4-8775-60d1b2cee9d7" />

now we use the same absolute path concept and try and execute a file which is in a different directory such as here the file is in the challenge directory

## Position Thy Self

Flag : `pwn.college{gJXtzl4emAjntyEWcJFXuXxkLeb.QX2QTN0wCM0gjNzEzW}`

<img width="574" height="190" alt="image" src="https://github.com/user-attachments/assets/82b4b549-64b2-4247-9e0b-d7e18a7e9a94" />

The Challenge Asks u to execute the `/challenge/run` file from a different path of it's choosing

## Position Elsewhere

Flag : `pwn.college{UgU97FTm_PsFYqldS9ulHIEB7_u.QX3QTN0wCM0gjNzEzW}`

<img width="653" height="190" alt="image" src="https://github.com/user-attachments/assets/dd1d8654-7a95-4fa4-8972-e34be3c5546c" />

Same as Previous Challenge just a different path

## Position Yet Elsewhere

Flag : `pwn.college{0uIv-JqGCkI7RJjAtjWJ9ygz1qk.QX4QTN0wCM0gjNzEzW}

<img width="625" height="211" alt="image" src="https://github.com/user-attachments/assets/b17e9b0b-1b5d-4692-8ce0-2ec5eef136db" />

Same as the last 2 challenges

## Implicit Relative Paths, from /

Flag : `pwn.college{YFskCdCz6QUdXqYQxd2xc2qSM-L.QX5QTN0wCM0gjNzEzW}`

<img width="561" height="115" alt="image" src="https://github.com/user-attachments/assets/c268a081-8d2b-4409-89be-3c0a3768272c" />

In this challenge we learn about relative paths, these are those paths which do not start with a `/` and do depend on ur current working directory.

## Explicit Relative Paths, from /

Flag : `pwn.college{UhkFdFtFhg7SwhqZKrwjVlzIRmm.QXwUTN0wCM0gjNzEzW}`

<img width="575" height="110" alt="image" src="https://github.com/user-attachments/assets/df293beb-7dff-4444-8862-59fd0a31d4a8" />

All relative paths are identical to each other so `./challenge/run` will do the same thing as `/challenge/run`

## Implicit Relative Paths

Flag : `pwn.college{wXClj1PFZ2K1ZC12oDhmNHT0KFX.QXxUTN0wCM0gjNzEzW}`

<img width="506" height="162" alt="image" src="https://github.com/user-attachments/assets/ef3dddf1-2334-42b9-9b6f-6161bdd5d8fa" />

In This We Go To The Directly The Program is in, but if we just try to run the program in the current working directory `nakedly` it will not run as a safety mechanism put up by linux we will have to use `./run` command instead of `run`.

## Home sweet home

Flag : `pwn.college{gk0Xj3deoJHTJztb_wyUOlkYSEZ.QXzMDO0wCM0gjNzEzW}`

<img width="514" height="177" alt="image" src="https://github.com/user-attachments/assets/c2379373-c091-4f66-8efc-9ff1e860242a" />

Here we learn about `~` , this is a shorthand for `/home/hacker` here `hacker` is the current user. Hence by typing `~/f` as an argument for the command /challenge/run, which copies the flag to the specified location in the argument to solve the challenge.
