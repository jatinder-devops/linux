# find
**_find_** command is used to search file and directories on the basis of name,type,size,date,or other conditions.
## Basic syntax of find
```
find [path] [options] [expression]
```
- **_path_**: where to start searching
- **_options_**: refine your search
- **_Expression_**: criteria like filenames or sizes
  
## Use-case of find 
### To find by Exact file name
```
find <directory> -name <file-name>
```
### Case-Insensitive file name search
```
find <directory> -iname <file-name>
```
### To find file only
```
find <directory> -type f
```
### To find directory only
```
find <PATH> -type d
```
### To find file by extension
```
find <directory> -name "*.<extension-name>"
```
### Find empty files or directories
```
find <directories> -empty
```
### Find file by size.
```
find <directories> -size <value>
```
### Find file in between n number of size
```
find <directories> -size +<value> -size -<value>
```
- c = bytes
- k = kilobytes
- M = megabytes
- G = gigabytes
### Find files by modification time
```
find <directory> -mtime -<value>
```
### Find file accessed recently 
```
file <directory> -atime -<value>
```
### Find file with specific permission
```
file <directory> -perm <mode>
```
- perm -mode = must have all permission bits
- perm /mode = match any of the bits
### Find file by owner name
```
find <directory> -user <username>
```
