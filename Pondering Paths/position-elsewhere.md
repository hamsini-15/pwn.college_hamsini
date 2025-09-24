# Position elsewhere
Similar to the previous challenge, this challenge tests my understanding on current working directory.

## My solve
**Flag:** `pwn.college{AiqOUOKL3tn__EKqXCIJTYk14oM.QX3QTN0wCOyAzNzEzW}`

Like in the previous challenge I first executed the `/challenge/run` command which resulted in an error stating that I was not in the correct directory which was the `/etc` directory. Using the `cd` command I switched the directory and retrieved the flag.

```bash
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /etc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /etc
hacker@paths~position-elsewhere:/etc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{AiqOUOKL3tn__EKqXCIJTYk14oM.QX3QTN0wCOyAzNzEzW}
hacker@paths~position-elsewhere:/etc$
```

## What I learned
Similar to the previous challenge, this challenge enforced that a process's current working directory affects the programs behaviour. For example comparing the previous challenge and this one, the change in the current directory from `/usr/share/doc/fontconfig` to `/etc` made a difference in the output of the command `/challenge/run`

## References 
None.
