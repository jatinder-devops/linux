# command: grep
The name grep stands for "Global Regular Expression print" that scan files line by lines and prints lines that match a given pattern.  This command is useful in scenarios where you want to search large files or logs. 
## Basic syntax
```
grep [options] pattern [file..]
```
Use-case of grep command.
### Basic search in a file
```
grep 'pattern' <file-name>
```
### case-insensitive Search.
```
grep -i 'pattern' search
```
### To show Line Numbers
```
grep -n 'patterns' <file-name>
```
### To count matching lines
```
grep -c 'patterns' <file-name>
```
### To show lines that do not match
```
grep -v 'patterns' <file-name>
```
### To match the complete word
```
grep -w 'patterns' <file-name>
```
### To match complete line 
```
grep -x 'patterns' <file-name>
```

## File/Directory
### To search inside directories recursivly
```
grep -r "pattern" <path/to/file>
```
### To recursive search and follows symbolic links 
```
grep -R "pattern" <path/to/file>
```
### To show only filename containing the match 
```
grep -l "pattern" <path/to/file> 
```
### To show only filename that don 

## Regular expression Option 
### Search for multiple patterns
```
grep -e 'patterns' -e 'pattern2 <file-name>
```
