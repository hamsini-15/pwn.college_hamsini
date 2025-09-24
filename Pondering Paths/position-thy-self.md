# Position thy self
Here we learn about the current working directory and how to use the `cd` command to more around the filesystem

## My solve
**Flag:** `pwn.college{8v9S7VMCZDjf9sF_aPBeFSg7dQi.QX2QTN0wCOyAzNzEzW}`

As I was instructed I first executed the `/challenge/run` command. Upon executing that I was given an error message saying that I was in the wrong directory. From there I used the `cd` command to change the directory to `/usr/share/doc/fontconfig` and then executed it and got the required flag.

```bash
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc/fontconfig directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usr/share/doc/fontconfig
hacker@paths~position-thy-self:/usr/share/doc/fontconfig$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{8v9S7VMCZDjf9sF_aPBeFSg7dQi.QX2QTN0wCOyAzNzEzW}
hacker@paths~position-thy-self:/usr/share/doc/fontconfig$
```

## What I learned
In this task I learnt the importance of **current directory** in Linux. Commands and programs run differently based on the directory selected. Therefore making it important to ensure the correct directory is sued to avoid errors. The `cd` command allows me to change the directory based on the requirments and the prompt (`~`,`/`) shows which directory I am in currently

## References 
Add any references or videos u used while solving the challenge.
