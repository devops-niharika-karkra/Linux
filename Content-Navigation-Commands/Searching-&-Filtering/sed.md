# Command: sed 

**_sed_** stands for stream editor. It is used to perform basic text transformations on an input stream. 

## Basic Syntax
```
  sed [OPTIONS] 'COMMAND' [INPUTFILE...]
```

## Use-case of sed command 
### To replace a specific word globally in a file
```
  sed 's/old-word/new-word/g' <filename>
```

<img width="796" height="202" alt="image" src="https://github.com/user-attachments/assets/dc4aefe8-c89e-4b52-938b-ba58eeeac2ec" />

### To replace only the first occurrence of word in a sentence
```
  sed 's/old-word/new-word' <filename>
```

<img width="796" height="202" alt="image" src="https://github.com/user-attachments/assets/fd27559f-3a98-4422-817a-b50a1d1c0e76" />

### To replace the word at particular number of occurrence 
```
  sed 's/old-word/new-word/n' <filename> 
```
where n is the number of occurrence 

### To replace word from a specific line number
```
  sed 'ns/old-word/new-word/' <filename>
```
where n is the number of line 

### To delete a particular line say n in this example
```
  sed 'nd' <filename>
```

### To delete a last line
```
  sed '$d' <filename>
```

### To delete line from range x to y
```
  sed 'x,yd' <filename>
```

### To delete from nth to last line 
```
  sed 'nth,$d' <filenme>
```

### To delete matching line
```
  sed '/pattern/d' <filename>
```

