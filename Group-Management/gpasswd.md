# gpasswd
**_gpasswd_** command is user to set password, add/remove user in groups and restrictions to groups.
## Basic Syntax.
```
gpasswd [OPTION] [group]
```
## Use-case of gpasswd 

### To add a user to group
```
sudo gpasswd -a <USER-NAME> <GROUP_NAME>
```
### To remove a user form group
```
sudo gpasswd -d <USER-NAME> <GROUP_NAME>
```
### To set a password for a group.
```
sudo gpasswd <GROUP-NAME>
```
### To remove the password from a group
```
sudo gpasswd -r <GROUP_NAME>
```
### To restrict the access to group
```
sudo gpasswd -R <GROUP-NAME>
```
### To set the list  of administrative user 
```
sudo gpasswd -A <user1 user1 user3....> <group-name>
```
### To set the list of group member
```
sudo gpasswd -M  <user1, user2, user3,...> <groupname>
```
