# Package Management:dnf
_**dnf**_ is the  package manager for Red Hat-basesd Systems.
- Red Hat-based System such as CentOS and Fedora, use yum or dnf (the next generation version of yum ) for packege management. Here's how to use dnf.
## Basic syntax
```
sudo dnf [option] {packege-name}
```
  ### To update your Package List
  ```
  sudo dnf check-update
  ```
### To install Package
```
sudo dnf install {package-name}
```
### To remove package 
```
sudo dnf remove {package-name}
```
### To upgrade package installed on Linux
```
sudo dnf upgrade
```
### To search for Packages
```
sudo dnf search {package-name}
```
### To show Package Information
```
sudo dnf info {package-name}
```
### To remove  packages that were automatically installed to satisfy dependencies for other packages.
```
sudo dnf autoremove
```
### To remove all cached package files
```
sudo dnf clean all
```
