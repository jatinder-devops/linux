# operator in linux

## In linux ***operator*** allow us to connect multiple commands, redirect data, and control execution logic directly from the terminal

### command chaining and control operaators

### ; (Semicolon):

  - Runs multiple commands sequentially, shell waits for command to finish, regardless of previous command succeeded or failed.
  
  - example:
    ```
      mkdir new_folder ; cd new_folder
    ```

### && (Logical AND): 

  - Runs the second command only if the first command executes successfully

  - Example:
  ```
    sudo apt install update && sudo apt upgrade -y
  ```

### || (Logical OR):

  - Run the second command only if the first command fails.

  - Example:
    ```
      sudo apt install tree || sudo snap install tree
    ```

### & (Ampersand): 

  - Sends the command to run in the background, freeing the terminal for user to perform another task.

  - Example:
    ```
      sleep 50 &
    ```

---

#  Redirection Operators

These operators change where a command reads its input from or where it sends its output.

### | (Pipe):

  - Takes the output of the first command and passes it as input to the next.

  - Example:
    ```
      ls -l | grep ".txt"
    ```
### > (Overwrite):
  - Redirect the output of  the command and **overwrites** the file if it already exists
  - Example:
    ```
    echo "Hello world!" > heelo.txt
    ```
    
### >> (Append):
- redirect the output of the command and **Appends** it to the target file.

- Example:
  ```
  echo "This is jatinder goswami." >> hello.tst 
  ```
### < (Input)

- Redirects standard input from file to command to read from a file instead of keyboard.

- Example:
  ```
  xargs mkdir < folder.txt
  ```
### 2> ( error redirection )

- Redirects standard error only

- Example:
```
rm -r example.txt 2> error.log
```

### &> (combined output redirection):

- redirects both standard output and error to same location
  
- Example:
  ```
  (mkdir example.txt && rm -r example.txt) &> file.log
  ```
---
# Grouping & substitution operators
- These operators are used to decide the environment and situation in which your command are execute.

### () [Parentheses]:
Runs commands inside a subshell. Variables changed inside will not affect your main shell.
Example:
```
(cd /tmp && ls)
```
### 

  
