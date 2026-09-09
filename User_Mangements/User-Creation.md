#  ***user creation*** 
## Different ways to create user in linux:
- useradd: This method of creating user is non-interactive i.e we have to create the things like password home-directory.
  etc manually.
- adduser: This method of creating  user interactive i.e prompts you step by step.

  ## Here is the different between useradd and adduser:
|    Fetures        |         useradd         |         adduser          |
|:-----------------:|:-----------------------:|:------------------------:|
| Interactivity     | Non-Interactive         |   Interactive            |
| Best used for     | Automation and scripting| Quick Manual user        |
| Home Directory    | Not created by default (requires -m to flag) |  created Automatically|
| Password Setup    | Set with passwd cmd | prompts you to set a password |
| Availabiliy       | Universal-availibal in all distros | provides debian, ubuntu, RHEL,CentOS,etc|

## usecase of useradd command
### creating user with 
```
sudo useradd <urename>
```
<img width="568" height="66" alt="image" src="https://github.com/user-attachments/assets/5cc2e386-4f59-4faa-a3a7-872ffdaf55cd" />

### For deleting user
```
sudo userdel <user-name>
```
<img width="568" height="66" alt="image" src="https://github.com/user-attachments/assets/bf11ac6e-103c-4033-83e5-c9b1d0ac8464" />

### User create with home directory.
To assign pre-defined directory using this command 
```
sudo useradd -d <path/to/dir> username
```
<img width="816" height="300" alt="image" src="https://github.com/user-attachments/assets/ea5e586f-29ff-4b6e-b319-69148a6538c6" />

 ### For deleting user with home directory
 User must be owner of the directory
```
sudo userdel -r test
```
<img width="826" height="147" alt="image" src="https://github.com/user-attachments/assets/3ee19a97-6434-471b-a1ad-2ddabea60f2a" />


### user create with home directory
 NO need to assign to manually directory.
```
sudo useradd -m username
```
<img width="666" height="154" alt="image" src="https://github.com/user-attachments/assets/b3df1944-f036-4e9f-91ba-c4f9fdba64d7" />

### User deleting with home directory.
```
sudo useradd -r <user-name>

```

<img width="706" height="210" alt="image" src="https://github.com/user-attachments/assets/7efdefcf-54f4-4b62-8fba-825b8cfc7aae" />

### User create with password 
⚠️Be careful using this command because it can expose your password on your terminal 
```
sudo useradd -m -p $(openssl passwd -6 "123456") test

```
<img width="1177" height="208" alt="image" src="https://github.com/user-attachments/assets/b5478aa3-98ad-4063-8518-c71dc3416707" />

### creating user to get the prompt to change password on first login 

```
sudo chage -d 0 <user-name>
sudo passwd -e <user-name>
```
### creating user with an expiry date
```
sudo user add -e <date> <user-name>

```
### create user with description
```
sudo useradd -c "Description" <user-name>

```
### Create a User with a Specific Login Shell
```
sudo useradd -s /bin/<shell-name> <user-name>
```
