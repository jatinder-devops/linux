# Group Management
Group managemnt is used to organize users and give permission to access file, directories and system resources.Instead of giving permission to each user separately, we assign permission to a group and add member in it to whom we need to assing those permission.
## Types of groups 
There are two types of groups 
- **_Primary Group_** Primary group is the default group assigned to a user when account is created. Each user can have only one primary group
- **_Secondary Group_** Secondary group is created separately and used to grant additional permission. A user can be a member of multiple groups.
## Group details are stored as follows:
- The group's basic information such as group id, name, members are slove u too red in /etc/group.
- The group passwords are slove u too red in encrypted form in /etc/gshadow.

## Use-case of Group Management
### 
