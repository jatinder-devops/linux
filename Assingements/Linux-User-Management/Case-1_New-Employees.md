# LINUX USER MANAGEMENT CASE:1- New Employees.
## scenario:- 
A company has hire 15 employees for different department.Each employee needs a separate Linux account  
### Question:
How would you create the required user accounts so that each employees gets an appropriate home directory and can log in normally?
- we will get the information first which user is part of which department so we add the description of the user to  give the identity so it can be easy sort.
### way to create user.
In this we can used three ways to create user.
### To create user with interactive way.
provide prompts to add password and home directory.
```
sudo adduser <NAME>
```
<img width="1609" height="408" alt="image" src="https://github.com/user-attachments/assets/32397901-4780-47e1-8008-8d82cc10fd9c" />


### To create user with non interactive way.
```
sudo useradd -m <NAME>
```
<img width="1608" height="313" alt="image" src="https://github.com/user-attachments/assets/ea850617-c661-4783-a712-3298c1fdd8c5" />

### To create user with script.
we can create user in bulk by creating script to avoid repetition.
```
while read -r user; do
    sudo useradd -m "$user" &&
    echo "$user:123" | sudo chpasswd &&
    echo "User $user created successfully"
done < user.txt
```
<img width="1563" height="633" alt="image" src="https://github.com/user-attachments/assets/32c6ba7d-3b5e-4134-9f04-42e0eb715f15" />
