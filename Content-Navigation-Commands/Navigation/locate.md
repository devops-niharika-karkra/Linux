# Command: locate
**locate** command in Linux is a fast and efficient tool used to find files by their name. It searches through a pre-built database 
of file paths instead of scanning the entire filesystem.

## Basic Syntax
```
  locate [OPTIONS] pattern
```

## Use-case of locate
### To locate the file with a specific name 
```
  locate <name>
```

### To locate file with with specific extension 
```
  locate '*.<ext>'
```

### To locate the file if we know last n number of character 
```
  locate '*<characters>'  
```

### To display the number of matching entries 
```
  locate -c '*<name>'
```

### To set the upper limit for searching items
```
  locate -l [value] '<.name>'
```

### To set a case-insensitive search 
```
  locate -i <NaMe.md>
```
