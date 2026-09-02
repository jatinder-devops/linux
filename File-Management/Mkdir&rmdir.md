# #mkdir
## ***mkdir*** stand for Make Directory. it is used to create one or multiple directories.
### syntax
```
mkdir <options> <dir-name>
```
### For creating single directory
```
mkdir <dir-name>
```
### For creating multiple directory 
```
mkdir <dir-name1 dir-name2>
```
### For creating parent directory
```
mkdir -p <dir1/dir2/dir3>
```
### For confirmation when  directory creation is completed
```
mkdir -v <dir-name>
```
### for creating multiple directory using array
```
mkdir dir{1..3}
```
This will create three directory in single time 

 ---
# rmdir
### ***rmdir*** is stand for remove directory and it let you delete empty directories.

#### To remove an empty directory:

```
rmdir <directory-name>
```
For removing parent directory
```
rmdir -p /parent/child
```
### To display message after removing the directory
```
rmdir -v dir1 dir2 dir3
```



