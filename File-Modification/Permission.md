# File Permissions
## In Linux, file permissions helps us to define who can read, write and execute file and directories.
### There are three basic file permissions:
  - **_Read_**: Denoted by (r or 4), provides the permission to view the file.
  - **_Write_**: Denoted by (w or 2), provides the permission to modify or write the file.
  - **_Execute_**: Denoted by (x or 1), provides the permissions to run the file as a program.

 |Permissions|Symbolic|Numeric|
 |:---------:|:------:|:-----:|
 |Read|r|4|
 |Write|w|2|
 |Execute|x|1|

 File Permission: Operation Chart

 |Operators| Definition|
 |:-------:|:---------:|
 |+| Add permission|
 |-| Remove permission|
 |=| Set the permission to the specified value|


## Permissions are assigned to three categories of users:
  - user (owner)
  - group
  - other

## **chmod** command is used to change the file permissions.

## Basic Syntax 
```
  chmod [OPTIONS] [mode] [file]
```

## Use-Cases of chmod command

### To add permissions to all user, group and other.
```
chmod a+rwx <File-Name>
```
```
chmod a+r <file-name> #read permission to all user.
```
```
chmod a+w <File-name> #write permission to all user.
```
```
chmod a+x <File-name> #Execute permission to all user.
```
To remove all permission to all user, group and other.
```
chmod a-rwx <File-Name>
```
```
chmod a-r <file-name> #Remove read permission of all .
```
```
chmod a-w <File-name> #Remove write permission of all .
```
```
chmod a-x <File-name> #Remove Execute permission of user.
```
### To add/remove permission to user only.
```
chmod u+/- [mode] <File-name>
```
### To add/remove permission to group only.
```
chmod g+/- [mode] <File-name>
```
###  To add/remove permission to other only.
```
chmod o+/- [mode] <File-name>
```
# To set permission with octal notations.
### To set permission to all read,write and Execute with octal notation.
```
chmod 777 <>
```
