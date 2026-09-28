# Command: find
**_find_** command is ussed to search files and directories on the basis of name, type, size, date, or other conditions.
## Basic Syntax
```
  find [path] [OPTIONS] [EXPRESSIONS]
```
In this syntax:
 - **path** is the starting point from where the search should begin
 - **options** are used to refine the search
 - **expression** is the criteria like filenames or sizes

## Use-case of find
### To find by exact file name
```
  find <directory> -name <file-name>
```

### Case-Insensitive file name search
```
  find <directory> -Iname <file-name>
```

### To find file only
```
  find <directory> -type f
```

### To find directory only 
```
  find <Path> -type d
```

### To find file by extension
```
  find <directory> -name "*.<ext>"
```

### To find empty files or directories
```
  find <directory> -empty
```

### Find file by size 
```
  find <directory> -size <value>
```

### To find file in between n number of size.
```
  find <directory> -size +<value> -size -<value>
```

- c = bytes
- k = kilobytes
- M = megabytes
- G = gigabytes

### To find files by modification time
```
  find <directory> -mtime -1
```

### To find file accessed recently
```
  find <directory> -atime -<value>
```

### To find file with specific permissions
```
  find <directory> -perm <mode>
```
- perm -mode = must have all permission bits
- perm /mode = mach any of the bits

### To find file by owner name 
```
  find <directory> -user <username>
```

