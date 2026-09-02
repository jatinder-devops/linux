# Tree 
The **tree** command is a powerful Linux utility that lets you display directories and their contents in a tree-like format. This is extremely helpful for organizing, understanding, or documenting file structures—especially when dealing with nested directories.

If **tree** is not already installed , use the following command
```
sudo apt update && sudo apt install tree 
```
### for display only directories 
```
tree -d
```
### for display hidden files 
```
tree -a
```

### for display  colored content in folder 
```
tree -c
```
 for display file and folder upto n where n is number of levels
```
tree -l <n>
```
### to display output in file 
```
tree -o <file_name>
```
### for display the folder which has number of item specified in the commmnad 
```
tree --filelime <value>
```
