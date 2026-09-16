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
chmod 777 <File-name>
```
### Table of octal notations

| Octal Value | Binary | Symbolic | Meaning |
| :---: | :---: | :---: | :--- |
| **0** | `000` | `---` | No permissions at all |
| **1** | `001` | `--x` | Execute only |
| **2** | `010` | `-w-` | Write only |
| **3** | `011` | `-wx` | Write and Execute (2 + 1) |
| **4** | `100` | `r--` | Read only |
| **5** | `101` | `r-x` | Read and Execute (4 + 1) |
| **6** | `110` | `rw-` | Read and Write (4 + 2) |
| **7** | `111` | `rwx` | Read, Write, and Execute (4 + 2 + 1) |

## Stickybit 
### To prevent file deletion and renaming inside a shared directory.
```
chmod -t <Name-file>
```
### To set permission with reference file
```
chmod --reference=<refer-file-name>  <file-name>
```
### To set permission recursively in a directory
```
chmod -R <permission> <directory-name>
```
In the case of parent child case.
```
chmod -R <permisson> </file/child-file>
```
### To set permission of all directories in particular location
```
find <path/to/directory> -type d -exec chmod <permission> {} \;
```
### To set permission of all files in particular location
```
find <path/to/directory> -type f -exec chmod <permission> {} \;
```
