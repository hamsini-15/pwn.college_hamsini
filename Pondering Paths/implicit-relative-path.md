# Implicit Relative Path
Explicitly use relative paths with . to run programs from the current directory.

## My solve
**Flag:** `pwn.college{YUerZErz1F8i8G4oF5cO9TvgB4q.QXxUTN0wCOyAzNzEzW}`

To start off, I changed the current directory to `/` and then tried executing the `./challenge/run` command but then I recieved an error stating that I was not in the correct directory `/challenge`. After changing the directory to `/challenge` and then executing `./run` I recieved the flag

```bash
hacker@paths~implicit-relative-path:~$ cd /
hacker@paths~implicit-relative-path:/$ ./challenge/run
Incorrect...
You are not currently in the /challenge directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-path:/$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{YUerZErz1F8i8G4oF5cO9TvgB4q.QXxUTN0wCOyAzNzEzW}
hacker@paths~implicit-relative-path:/challenge$
```

## What I learned
I learned that Linux does not automatically check the current directory when executing a command with a **naked** path. For example, running `run` inside `/challenge` won’t work resulting in an error such as `bash: run: command not found`. To explicitly tell Linux to look in the current directory, we must prepend `./`before the program name, like `./run`. 

## References 
None.
