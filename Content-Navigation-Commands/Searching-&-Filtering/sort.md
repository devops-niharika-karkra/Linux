# Command: sort
**_sort_** command is used to sort a file, arranging the records in a particular order assuming the contents are ASCII.

## Basic Syntax 
```
  sort [OPTION]... [FILE]...
```

## Use-Cases of sort
### To sort the file alphabetically
```
  sort <filename>
```

### To get the output in a file
```
  sort -o <filename>
```

### To reverse the order of sort
```
  sort -r <filename>
```

### To sort file numerically
```
  sort -n <filename>
```

### To sort a file based on specific column number
```
  sort -k<number> <filename>
```

### To sort the file and remove duplicates
```
  sort -u <filename>
```

