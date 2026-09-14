# id 
## _id_ is used to print the user id of the user along with the group id. it is handy tool for system admin and devops 
to retrive information of user available in Linux machine.

### Basic syntax 
```
id <option> <user-name>
```
## Use-cases of id 

### To print current user's identity.
```
id 
```
### To print specific user's identity.
```
id [user-name]
```
### To print effective  g[id].
```
id -g [user]
```
### To print all group ids to  which user belongs to.
```
id -G [user]
```
### To print the uid of specific user 
```
id -u [user-name]
```
### To display a name of instead of numbers
```
id -nu [user-name]
```
```
id -ng [user-name]
```
```
id -nG [user-name]
```
### To display real ids instead of effective id 
```
id -ru [user]
```
```
id -rg [user]
```
```
id -rG [user]
```
