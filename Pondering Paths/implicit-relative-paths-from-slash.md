# Implicit Relative Paths from '/'
This challenge introduces the idea of relative paths. Unlike absolute paths, these paths depend upon the current working directory.

## My solve
**Flag:** `pwn.college{cuaw7_R_2zG8TDAf789L3PvteQD.QX5QTN0wCOyAzNzEzW}`

I first executed the `/challenge/run` command. Upon which I encountered an error message stating that I wasnt in the `/` directory. After using `cd /` I then made the command `/challenge/run` command relative to that by removing the first `/` as we are already in that directory

```bash
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{cuaw7_R_2zG8TDAf789L3PvteQD.QX5QTN0wCOyAzNzEzW}
hacker@paths~implicit-relative-paths-from-:/$
```

## What I learned
Relative paths (coming from the name 'relative') depend on where I am currently located in the file system. This exercise taught me the difference between absolute and relative paths. Additionally, if my working directory is `/` then the relative paths are just the directory names after the first `/`.

## References 
None.
