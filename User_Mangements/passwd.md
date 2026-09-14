#  passwd
## _passwd_ command is use to create or reset the password of user.
### Basic Syntax
```
passwd [option] [USER]
```
### use-cases of password command 
### To change your own password 
```
passwd 
```
### To change another user's password 
```
sudo passwd <user-name>
```
### To force a user to change password on next login 
```
sudo passwd -e [user-name]
```
### To set age of password (maximum number of day)
```
sudo -x [number of day] <user-name>
```
### To set minimum number of days password
```
sudo passwd -n [number of day] <user-name>
```
### To set the warning days before a password expires.
```
sudo passwd -w [number of day]<user-name>
```
### To lock the user's account
```
sudo passwd  -l <user name>
```
### To unlock the user's account 
```
sudo passwd -u < user name >
```
### To set no password 
```
sudo passwd -d <user-name>
```
### To show the status of user account.
```
sudo passwd -S <user-name>
```
<img width="733" height="105" alt="image" src="https://github.com/user-attachments/assets/30069b87-04dd-47af-a1a6-c3be97f920c0" />

|Field| Example Value|Description|
|:---:|:------------:|:---------|
|jatinder| alice|The login name of account|
|status| p| <ul type=none><li> P=usable password </li> <li>L=Account locked </li> <li> NP =No password </li> </ul>|
|Last Changed| 2026-04-27| The date the password was last modified|
|Min Age| 0 |Minimum days required before the password can be changed|
|Max Age | 99999| Maximum days the password remains vaild before it explain|
|Warning|7|Number of days before expiration that the user gets a warning.|
|Inactivity| 7| Number of days after expiration before the account is deactivated.|
