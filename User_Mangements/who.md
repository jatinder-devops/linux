# who command 
**_who _** command is used to print information about the currently logged in users
##  Basic Syntax
who <option>
### Use-case of who command
### To display all the information same as -b -c --login -p -r -t -T -u
```
who -a
```
### To display time of last boot
```
who -b 
```
### To display column heading.
```
who -H
```
### To display system login process.
```
who -l
```
### To show hostnames instead of IP addresses.
```
who --lookups
```
### To show Run Level
```
who -r
```
### To display all login names and number of users logged on
```
who -q
```
### To display list of user logged in
```
who -u
```
⚠️ Modern versions of systemd have officially dropped utmp support due to which who from coreutils has nothing to read and simply outputs a blank line.
