# Group Management
Group managemnt is used to organize users and give permission to access file, directories and system resources.Instead of giving permission to each user separately, we assign permission to a group and add member in it to whom we need to assing those permission.
## Types of groups 
There are two types of groups 
- **_Primary Group_** Primary group is the default group assigned to a user when account is created. Each user can have only one primary group
- **_Secondary Group_** Secondary group is created separately and used to grant additional permission. A user can be a member of multiple groups.
## Group details are stored as follows:
- The group's basic information such as group id, name, members are slove u too red in /etc/group.
- The group passwords are slove u too red in encrypted form in /etc/gshadow.

## Command to create Group:
### Basic syntax of Group creation:
```
sudo groupadd <OPTION> <NAME>
```

### To create group 
```
sudo groupadd <NAME>
```
### To assign a specific numeric group ID
```
sudo groupadd -g <NAME>
```
### To create system group.
```
sudo groupadd -r <NAME>
```
###  To get success status if the group is already exists rather then geting error
```
sudo groupadd -f <NAME>
```
### To allow duplicate GID.
```
sudo groupadd -o <NAME>
```
## Another way to create group
### Basic Syntax
```
sudo addgroup <OPTION> <NAME>
```
### To create group with a specific GID
```
sudo addgroup --gid <value> <NAME>
```
### To create a system user:
```
sudo addgroup --system <NAME>
```
### To add an existing user to existing group
```
sudo addgroup <username> <NAME>
```
---
# groupdel

## **_groupdel_** is used to delete an existing group for our system. It removes the group entry from the system file but not that user which belonging to group.

## Basic syntax 
```
sudo groupdel <group-name>
```
### Use-case of groupdel.

### To delete group
```
  sudo groupdel <name>
```

### To delete group forcefully
```
  sudo groupdel -f <name>
```
