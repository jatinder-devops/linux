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
