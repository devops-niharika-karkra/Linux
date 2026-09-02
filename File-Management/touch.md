# Command: Touch
***touch*** is used for creating empty file. 
We need to specify the file extension to define the type of file like .html, .py, .sh, etc. 
Without extension touch by default create a txt file. 

### Here are some popular extensions that we use,

| .html  | html files (Hyper Text Markup Language) |
| :----: | :------------------------------------ |
| .css   | css files (Cascading Style Sheet)       |
| .sh    | shell script                            |
| .py    | python                                  |
    
## Use-Cases of touch command

### To create a single empty file
```
  touch <filename>
```

### To create multiple files
```
  touch <file1> <file2> <file3>
```

### To create multiple files using an array
```
  touch {file1..10}
```
It create 10 file in single time

