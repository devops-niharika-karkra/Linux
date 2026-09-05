# Operators in Linux
In Linux, **Operators** allow us to connect multiple commands, redirect data, and control execution logic directly from the terminal.

## Command Chaining and Control Operators
These operators manage how and when consecutive commands are eecuted.

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

##  Redirection Operators
These operators change where a command reads its input from or where it sends its output.

### | (Pipe):
  - Takes the output of the first command and passes it as input to the next.

  - Example:
    ```
      ls -l | grep ".txt"
    ```
### > (Overwrite):
  - Redirect the output of the command and **Overwrites** the file if it already exists.

  - Example:
    ```
      echo "Hello World!" > hello.txt
    ```

### >> (Append):
  - Redirect the output of the command and **Appends** it to the target file.

  - Example:
    ```
      echo "This is Niharika." >> hello.txt
    ```

### < (Input):
  - Redirects standard input, forces command to read from a file instead of keyword.

  - Example:
    ```
      xargs mkdir < folder.txt
    ```

### 2> (error redirection):
  - Redirects standard error only.

  - Example:
    ```
      rm -r example.txt 2> error.log
    ```

### &> (Combined output redirection):
  - Redirects both standard output and error to same location.

  - Example:
    ```
        (mkdir -v example && rm example) &> file.log
    ```
---

## Grouping and substitution operator 
  - These operators are used to decide the environment and situation in which your commands are executed.

### () (Parentheses): 
  - Runs commands inside a subshell. Variables changed inside will not affect your main shell.

  - Example:
  ```
    (cd /tmp && ls)
  ```
### {} (curly braces): 
  - Groups commands to run together in the current shell context.

  - Example:
    ```
      {touch file1.txt; echo "Hello World" > file1.txt; cat file1.txt }
    ```
