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
### To show only filename that don't matched with content searched.
```
grep -L "pattern" <path/to/file> 
```
### To always show filename
```
grep -H "pattern" <path/to/file> 
```
### To hides the filename
```
grep -h "pattern" <path/to/file> 
```
### To stop after a spercified number of matching lines
```
grep -m "pattern" <path/to/file> 
```
### To suppresses error messages
```
grep -s "pattern" <path/to/file> 
```
## Regular expression Option 
### To Enables Extended Regular Expressions
```
grep -E 'pattren
```
### Treats the pattern as a fixed string, not regex
```
grep -F "pattern" <path/to/file>
```
### To Use Basic Regular Expressions; default mode
```
grep -G "pattern" <path/to/file>
```
### To use perl-compatible regular expressions

```
grep -P "pattern"{value} <path/to/file>
```

### Search for multiple patterns
```
grep -e 'patterns' -e 'pattern2 <file-name>
```
### To read search patterns from a file
```
grep -f "patterns" <file-name>
```
## Advance options
### To show byte offset of matching
```
grep -b "pattren" <file-name>
```
### To treats NULL character as the line separator
```
grep -z "pattren" <file-name>
```
### To flushes output after every line
```
grep --line-buffer "pattren" <file-name>
```
### To  set a lable for standard input
```
cat <file-name> | grep --lable=<file-name> "pattern" <path/to/file>
```
### To control binary-files handling
```
grep  --binary-file=type "pattern" <file-name>
```
