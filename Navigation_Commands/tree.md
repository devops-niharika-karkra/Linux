# Command: Tree

This command is used to show all the sub directories and files of a directory in an organized tree structure.

If the tree in not already installed, then you can run the following to command to install it:
```
  sudo apt update && sudo apt install tree
```

## UseCases Of Tree Command

### To display only directories
```
  tree -d
```

### To display all files including hidden
```
  tree -a
```

### To display files in human-readable format
```
  tree -h
```

### To display colored content in folder
```
  tree -C
```

### To display files and folders upto n where n is number of levels. 
```
  tree -L <n>
```

### To display output in a file
```
  tree -o <file_name>
```

### To hide the folder which has number of items more than the specified number 
```
  tree --filelimit <number>
```
