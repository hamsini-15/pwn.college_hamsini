# Program and Absolute Paths
 We are required to execute a program in the given directory

## My solve
**Flag:** `pwn.college{k3qjoQt3BHAxzV4WsMFC-YW1TXq.QX1QTN0wCOyAzNzEzW}`

 In this challenge, the program is located in the `challenge` directory which is inside the root `/`. The program named `run` is in the `challenge` directory. The task here is to execute the `/challenge/run` command which is the absolute directory

```bash
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{k3qjoQt3BHAxzV4WsMFC-YW1TXq.QX1QTN0wCOyAzNzEzW}
hacker@paths~program-and-absolute-paths:~$
```

## What I learned
From this challenge I learnt the importance of **absolute paths** in Linux. Absolute paths always start from the root (`/`) and point to the exact location of a file or program.

## References 
None
