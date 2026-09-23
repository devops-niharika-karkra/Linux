# Command: grep 
The name grep stands for "Global Regular Expression Print" that scans files line by line and prints lines that match a given pattern.

## Basic Syntax
```
  grep [options] pattern [file...]
```

## Use-case of grep command

### Basic search in a file
```
  grep 'pattern' <filename>
```

### case-insensitive Search
```
  grep -i 'pattern' search
```

### To show Line Numbers
```
  grep -n 'patterns' <filename>
```

### To count matching lines 
```
  grep -c 'patterns' <filename>
```

### To show lines that do not match 
```
  grep -v 'pattern' <filename>
```

### To match the complete word
```
  grep -w 'pattern' <filename>
```

### To match complete line 
```
  grep -x 'patterns' <filename>
```

## File/Directory
### To search inside directories
```
  grep -r "pattern" <path/to/file>
```

### To recursive search and follows symbolic links
```
  grep -R "pattern" <path/to/file>
```

### To show only filename containing the match
```
  grep -l "pattern" <filename>
```

### To show only filename that don't match with content searched
```
  grep -L "pattern" <filename>
```

## Regular expression
### Search for multiple patterns 
```
  grep -e 'pattern1' -e 'pattern2' <filename>
```

