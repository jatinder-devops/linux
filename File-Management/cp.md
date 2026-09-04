#cp
## cp stand for copy. It allows you to copy files, folders, and directories within the Linux system.
## basic syntax  
```
cp [options] <source> <desitination>
```
### use-case of cp 
```
cp <source_file> <destination-file>
```
### To copy file into new file 
```
cp <source_file> path/to/directory
```
### To copy multiple file  in a Directory
```
cp file1 file2 file3 /path/to/directory
```
### to copy an entire directory 
```
cp -r /source/folder /destination
```
### ask for confirmation before copy the file 
```
cp -i <file1> file2>
```
### To display the output what files are being coped
```
cp -v <file1> file2> 
```
### Retains the original file modifications times, access times, and permissions.
```
cp -p <file1> <file2>
```
### You can use wildcards like * to copy multiple files that match a specific extension or pattern.
For example, to copy all text files into a backup folder
```
cp *.txt /destination
```
