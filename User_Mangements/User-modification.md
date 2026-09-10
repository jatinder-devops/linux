# User-Modification 

## usermod 
Is  a command-line-utiltiy for modifying user account. you can use it to add a user to group, change the default shell
,rename a user,set an expiry date ,lock or unlock user and more.

To create new use,see [user-creation](https://github.com/jatinder-devops/linux/blob/ad36e778ce403911f9cd43b90a768d5e1b34fe17/User_Mangements/User-Creation.md )

### command syntax
```
usermod [option] USER
```
### To add user in a supplementary group
```
sudo usermod -aG <group> <user> 
```
### To change user's primary group
```
sudo usermod -g <group> <user>
```
### To set expiration date of user 
```
sudo usermod -e <date-user> <user-name
```
### To add a command field
```
usermod -c "This is devops " <user-name>
```
### To modify user's Home Directory 
```
sudo usermod -d /new/home/directory <user-name 
```
### To move home Directory contents
```
sudo usermod -d /new/
```
