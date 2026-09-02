# #touch
***touch*** is used for creating empty file. 
"We need to specify the file extension to define the file type, such as .html, .py, or .sh. Without an extension, touch creates a file with no extension by default. If the file already exists, its timestamp will update to the exact time the command was executed."
### Here are some popular extensions 


 
| .html     | html file Hyper Text Markup Language  | 
| :-------- | :------------------------------------ | 
| .css      | css file cascading style sheet        |
| .sh       | Shell script                          | 
| .py       |  Python                               |

## use-cases of touch command 
### To create a single empty file 
```
touch <file-name>
```
### To create multiple file 
```
touch <file-name1 file-name2>
```
### To create multiple file using array
```
touch file-name{1..10}
```
It create 10 file in single time.
