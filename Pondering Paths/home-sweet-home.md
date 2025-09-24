# Home Sweet Home
This challenge asks us to provide an absolute path inside our home directory `/home/hacker` as an argument to `/challenge/run`.

## My solve
**Flag:** `pwn.college{kHTzl4ryFjRZ0oXnCgH-3mp-61k.QXzMDO0wCOyAzNzEzW}`

As mentioned I wrote the `/challenge/run` command but then while executing it asked to add an argument. Inferring from the information given on pwn.college I assumed the arguement to be `~/asdf` but it gave me the hint that the argument is on 3 characters long so I then added `~/f` as the argument which gave me the flag.

```bash
hacker@paths~home-sweet-home:~$ /challenge/run
You must provide an argument to /challenge/run when you invoke it!
hacker@paths~home-sweet-home:~$ /challenge/run ~/asdf
The argument you provided must not have been longer than 3 characters it's
currently 6 characters long)!
hacker@paths~home-sweet-home:~$ /challenge/run ~/f
Writing the file to /home/hacker/f!
... and reading it back to you:
pwn.college{kHTzl4ryFjRZ0oXnCgH-3mp-61k.QXzMDO0wCOyAzNzEzW}
hacker@paths~home-sweet-home:~$
```

## What I learned
The `~` symbol is shorthand for the home directory and expands to `/home/username`. Absolute paths are required when working with filesystem arguments in challenges like this, even if a path looks short (`~`), Bash expands it correctly behind the scenes. Using shell expansions can help meet strict constraints like character limits.

## References 
None.
