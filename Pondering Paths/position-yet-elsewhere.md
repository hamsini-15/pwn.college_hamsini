# Position yet elsewhere
This challenge again focuses on the current working directory.

## My solve
**Flag:** `pwn.college{AvdRTxIqtMtEQyAsfzKrRqBZT38.QX4QTN0wCOyAzNzEzW}`

I started by running `/challenge/run`, and the program told me which directory I needed to be in (` /usr/aarch64-linux-gnu/include/gnu`). I then used the cd command to move into that directory and then executed the command `/challenge/run`

```bash
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/aarch64-linux-gnu/include/gnu directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /usr/aarch64-linux-gnu/include/gnu
hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu/include/gnu$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{AvdRTxIqtMtEQyAsfzKrRqBZT38.QX4QTN0wCOyAzNzEzW}
hacker@paths~position-yet-elsewhere:/usr/aarch64-linux-gnu/include/gnu$
```

## What I learned
This challenege, along with the previous 2 taught me how to use the `cd` command and how important directories are.

## References 
None.
