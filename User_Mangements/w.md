#  #w 
**_w_** is the command which display a summarized view of who is logged in and what processes they are currently executing,along with important system statistic such as uptime and load averages.
### Basic Syntax
```
w 
```

### To show the user detail

## The output detail
- USER: Name of the logged-in user
- TTY: Terminal session type (ttyX for physical consoles, pts/X for SSH or terminal emulators)
- FROM: Login source (IP address, hostname, or :0 for local) of the user
- LOGIN@: Login time of the user
- IDLE: Time user has been inactive
- JCPU: Total CPU time used by all processes attached to the terminal
- PCPU: CPU time used by the command listed in WHAT
- WHAT: Current process the user running in the session

## The w Command Can be Used:
- To see who is logged in and from where
- To track what command or process each user is executing
- To detect idle or forgotten sessions
- To verify unexpected remote logins
- To diagnose load or performance issues

### use-case of **_w_** command
### To display short format.
```
w -s
```
### To ignores  the username while figuring out the current process and cpu times.
```
w -u
```
### No need to print header
```
w -h
```
### To find logged-in users by checking their terminals.
```
w -t
```
### To display IP address instead of hostname for from field.
```
w -i
```

### To display pid of the login process
```
w -p
```
