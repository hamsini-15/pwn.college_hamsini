# Explicit Relative Paths from '/'
Understanding the use of `.` in relative paths when navigating directories.

## My solve
**Flag:** `pwn.college{k1EuvIXAXcSJauvpoyhdlqIiD_F.QXwUTN0wCOyAzNzEzW}`

As per the challenge name I changed the current working directory to `/`. Based on the information given on pwn.college, `./challenge/run` is the same as `/challenge/run` hence I executed the `./challenge/run` command.

```bash
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{k1EuvIXAXcSJauvpoyhdlqIiD_F.QXwUTN0wCOyAzNzEzW}
hacker@paths~explicit-relative-paths-from-:/$
```

## What I learned
I learned how relative paths in Linux work with the special directory entries `.` (current directory) and `..` (parent directory). This challenge reinforced that paths like `challenge`, `./challenge`, and even longer forms such as `../../../challenge` all point to the same location if used correctly. It showed me how absolute and relative paths can be written in different ways but still resolve to the same directory, depending on the current working directory.

## References 
None.

