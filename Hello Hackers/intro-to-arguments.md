# Intro to Arguments
This challenges requires us to pass commands with arguments and observe the difference in the outputs. 

## My solve
**Flag:** `pwn.college{w8L5SKprVvglGmPurURB5o84QE7.QX4YjM1wCOyAzNzEzW}`

The `echo` command can take an infinite ammount of arugments. For example the command `echo Hello` has one argument `Hello` and will return `Hello` to the terminal. `echo Hello Hackers!` prints `Hello Hackers!`. In this case 2 arguments are taken which are `Hello` and `Hackers!`.

```bash
hacker@hello~intro-to-arguments:~$ hello hackers
Success! Here is your flag:
pwn.college{w8L5SKprVvglGmPurURB5o84QE7.QX4YjM1wCOyAzNzEzW}
hacker@hello~intro-to-arguments:~$ 
```

## What I learned
An **argument** is nothing but the additional data passed with a fucntion. Always, the first word is the function and the following words are the argument(s). The `echo` command does nothing but repeats or **echoes** the arguments given to it on the terminal and can take an infinte number of arguments to it.

## References 
None
