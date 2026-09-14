# chage 
## _chage_ command short for "change age " of user . This command is used to get information about user account and password age and more.

## Basic Syntax 
```
chage <OPTION> [User-NAme]
```
### Use-Case of chage command 
### To view user's current account aging information
```
sudo chage -l [ USER-NAME]
```
### To set all the value through interactive mode.
```
sudo chage -i <USER-NAME>
```
### To set last password change date 
```
sudo chage -d <yyyy-mm-dd> [username]
```
### To set account expiry date 
```
sudo chage -E <USER-NAME>
```

### To set minimum number of day .
```
sudo chage -m <USER-NAME>
```
### To set maximum number of day
```
sudo chage -M <USER_NAME>
```
### To set inactivity after password expiry before account locked.
```
sudo chage -I < USER-NAME>
```
### To set warning days before password change.
```
sudo chage -W <USER-NAME>
```
### To fix user on a broken computer or a backup computer drive plugged-into your computer.
```
sudo chage -R <USER-NAME>
```
