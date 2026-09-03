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
  - 

