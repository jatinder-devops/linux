## How to set user resource limits in linux?
we set resource limit to prevent conditions like fork bomb.
### These situation can cause:
- Application failure
- Slow system performance
- Login or SSH failures
- Service interruption
- Denial-of-service conditions
- System instability

## what are Linux resources limits ?
Define the limit how much of a particular resource a user or process can comsume.
### some commonly controlled resource.
- Number of open files
- Number of running processes
- Maximum file size
- Maximum stack size
- CPU execution time
- Core dump size
- Locked memory

## Linux uses two types of limits:

## soft limit:
## Hard limit:
### ***soft limit*** is the limit that is currently being applied to user or process by the operating system.
The user can increase this limit  when needed ,but the new value cannot be higher than the hard limit.
- ***For Example-*** The soft limit is 1000 and the hard limit is 2000 the user can increase the soft limit up to 2000,
but not beyond it
### Basic syntax 
```
ulimit <option>

```
### Basic syntax for command to set limit
```
  ulimit <OPTIONS> <value>
```

### Different use-cases of _**soft limit**_

### To display the  limits of current running shwll:
```
ulimit -a
```

### To display the size of files written by the shell and its children 
```
ulimit -f
```
#### To set the limit
```
ulimit -f <value>
```
### To display the numnber of open file
```
ulimit -n
```
### To display the Number of running processes
```
ulimit -u
```
### To display the Maximum file size
```
ulimit -m
```
### To display the Maximum stack size
```
ulimit -s
```
### To display the CPU execution time
```
ulimit -t
```
### To display the Core dump size
```
ulimit -c
```
### To display the Locked memory
```
ulimit -l
```
