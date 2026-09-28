# locate
``locate`` almost works like the librarian in a library. 
When you ask the librarian for a book, 
he/she can find it for you in the entire library very efficiently because the books are sorted by some order.

## Basic syntax of locate
```
locate [option] pattern
```
## Use-case of locate
### To find the file with a specific name 
```
locate <name>
```
### To find file with specific extension
```
locate '*.extension'
```
### To find the file if we know last n number of character
```
locate '*<characters>'
```
### To displays the number of matched items
```
locate -c '*.<Name>'
```
### To set the upper limit for searching items
```
locate -l [value] '.<Name>'

```
### To do a case-insensitive search
```
locate -i <NaMe.mD>
```
###
