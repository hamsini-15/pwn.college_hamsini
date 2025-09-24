# The Root
This task requires us to launch the terminal and execute the `pwn` program using its absolute path

## My solve
**Flag:** `pwn.college{UdjJPvIRHSu-V7-pf8-1I21An0a.QX4cTO0wCOyAzNzEzW}`

I was required to simply execute the `/pwn` program which is the program's absolute path. 

```bash
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{UdjJPvIRHSu-V7-pf8-1I21An0a.QX4cTO0wCOyAzNzEzW}
```

## What I learned
I've learnt that a filesystem starts at `/` which consists of many other directories, configuration files, programs and flags. The `/` indocates the root directory which is also known as an **absolute path**

## References 
Add any references or videos u used while solving the challenge.
