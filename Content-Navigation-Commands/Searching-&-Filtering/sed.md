# sed
The **_sed_** command is used to search, replace, add, and delete text or lines in a file.
## Basic syntax 
```
sed [OPTIONS] 'COMMAND' [INPUTFILE...]
```
## Use-case of sed command 

### To replace a specific word globally in a file
```
sed 's/old-word/new-word/g'
```
<img width="1059" height="232" alt="image" src="https://github.com/user-attachments/assets/fad76396-dfa9-4e4d-a103-d06fa631a2f6" />

### To replace only the first occurrence of word in a sentence
```
sed 's/old-word/new-word' <file-name>
```

<img width="1059" height="232" alt="image" src="https://github.com/user-attachments/assets/88b5ec44-421f-4afb-9fb7-59a9d2b6096c" />

### To replace the word at paticular occurrence
```
sed 's/old-word/new-world/n' <file-name>
```
where n is the number of occurrence 
### To replace word from a specific line number 
```
sed 'ns/old-user/new-word/' <file-name>
```
when n is the number of line

## To delete using sed 

### TO delete a particular line say n in the example 
```
sed 'nd' <filename>
```
### To delete a last line 
```
sed '$d' <file-name>
```
### To delete line from range x to y
```
sed 'x,yd' <file-name>
```
### To delete from nth to last time 
```
sed 'nth,$d' <filename>
```
### To delete matching line 
```
sed 'pattern/d' <filename>
```
