# Package Management: apt
**_Linux Package Management_** is responsible for installing,upgrading,configuring and removing software packages.Each linux has its own package management system 
### what is a Package ?
A package in Linux is a collection of files bundled together to provide a piece of software.

### To Update a package list in repositories on your Linux operating system.
```
sudo apt update
```
### To update installed package in Linux.
```
sudo apt upgrade
```

TO avoid manual confermation
```
sudo apt upgrade -y
```
### To upgrade the package with the ability to add or remove packages to resolve conflicts.
```
sudo apt dist-upgrade <package-name>
```
### To install a package in linux.
```
sudo apt install <package-name>
```
Using -y flag when we don't required any manual confirmation.
```
sudo apt install <package-name> -y
```
### To remove package.
```
sudo apt remove  <package-name>
```
### To remove package with its all dependencies.
```
sudo apt purge <package-name>
```
### To search for packages.
```
sudo apt search <package-name>
```
### To show Package information
```
sudo apt show <package-name>
```
### To remove unnecessary packages and cache file.
```
sudo apt autoremove 
```
```
sudo apt clean 
```
### To add repository 
```
sudo add-apt-repository <NAME_OF-REPOSITORY>
```
