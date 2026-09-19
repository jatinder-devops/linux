# ACLs
**_ACLs_** stand for Access Control List. It allow us to set specific permission for individual user groups and owner. ACL allow us to set more detailed permission giving us greater flexibility and control over who can access your files and directories.
**_ACL_** help us to manage complex permission requirements easily.
Use of acl
Granular control: Assign permission to individual user or group without changing  the file's ownership.
Flexibility: Manage access for multiple users or group with different permission levels.
Enhanced Collaboration: Share files and directories securely in multi-user environments.

Use-case of acl 
In linux we have used alc with two types .
`setfacl` : Using this command we can set permisssion to files or Driectory. 
`getfacl` : Using this command we check what permission are set to files or Driectory. 

### Basic Syntax of getfacl:
```
getfacl [OPTION] <NAME-FILE/DRIECTORY>
```
### To display default Access Control List.
```
getfacl -d <NAME>
```
### To display ACLs with Numeric User and group IDs
```
getfacl -n <NAME>
```
### To view ALCs without headers
```
getrfacl -c <NAME>
```
### To list all the file recurcive acl view.
```
getfacl -R <NAME>
```
### To display ACLs in an raw format.
```
getfacl -e <NAME>
```
### To display extended attributes
```
getfacl -d <NAME>
```
### TO display ACLs for multiple files.
```
getfacl <NAME1,NAME2,NAME3,>
```
## Let's learn about setfacl in detail.
### Basic syntax
```
setfacl [option] <ACL> <file>
```
## use-case of setfacl
### ACL entries follow a specific format:
```
[entry_type]:[name]:[permission]
```
### To set ACL for a group
```
setfacl -m g:<NAME-OF-GROUP>:<permission> <NAME-OF-DIRE/FILE>
```
### To remove ACL entries.
```
setfacl -x u:<USER> <NAME>
```
### To remove all ACL entries.
```
setfacl -b <NAME>
```
### To set Default ACL for a directory
```
setfacl -d -m g:developer:<permission> <NAME>
```
### To set mask permissions.
```
setfacl -m m::<permission> <NAME>
```
### To set ACL to a directory and all its contents.
```
setfacl -R -m u:<USER-NAME>:<PERMISSION> <DIrectory>
```
