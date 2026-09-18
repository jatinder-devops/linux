## groupmod 
**_groupmod_** is a linux command that is used to modify the properties of existing group on our system 
what will we do with this command 
- Change the group name
- Group id
- attributes
## Basic syntax 
```
groupmod [OPTION] <group-name>
```
### Use-cases of groupmod

### To add users as member of the group.
```
sudo groupmod -U <user1,user2,user3....>
```
### To append users to the exixting numbers list of a group
```
sudo groupmod -a <user1,user2.user3...>
```
### To rename a group

```
sudo groupmod -n <OLD-NAME> <NEW_NAME>
```
### To change the group ID to the specified value.
```
sudo groupmod -g <GROUP_NAME>
```
### To change group password 
```
sudo groupmod -p [pasword] <GROUP-NAME>
```
