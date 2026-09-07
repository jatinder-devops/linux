# vim 
## ***vim*** stands for Vi IMproved.
It is a free and open text editor. It is enhanced version of vi. It is easy but require knowledge to work using this tool. Its save all of our working information in the vim.info file.

### To open  the file using vim.
```
vim <file.txt>
```
## vim can be used in three different mode.
### #Normal
### #Insert
### #command line mode
---
### To get into insert mode.
Press i when we enter into the file.
### To get exit from insert mode.
Press ***esc*** key 
### To save (write) a file 
```
:w
```
### To quit the file 
```
:q
```
### To save and quit a file
```
:wq
```
### To force quit if you want to quit without saving the file.
```
:q!
```
### To search a word
```
:/<word-to-search>
```
### To do case-insenitive seaching

```
:set ignorecase
:/<word-to-seach
:set 'ignorcase' #to return back normal
```
### To search and replace text
```
:%s/<search-word>/<replace-word>/
:%s/<word-to-search>/word-to-replace-withl/g #to replace word globally
```
### To display line number 
```
:set nu
or
:set number
```
### To display relative line number 
```
:set rnu
or
:set relativenumber 
```
### To remove line number
```
:set nu!
:set nonumber
:set nonu
```
### To remove relative line number
```
:set rnu!
:set norelativenumber
:set nornu
```


---
## Some other useful shortcuts (In the normal mode):
## keys used to move cursor in file
### h: is used for  left 
### j: is used for down 
### k: is used for up
### l: is used for right
 
## To delete characters using command
```
D        #used for delete single line
x        #used for delete single character
dd       #used for delete single line 
(num)dd  #used for delete for multi line
```

## To copy and past in the file 
```
yy It yanks (Vim's term for copy) the current line.
p  It is used for past 
```
