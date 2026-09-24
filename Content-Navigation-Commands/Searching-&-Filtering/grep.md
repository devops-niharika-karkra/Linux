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

### To always show filename
```
  grep -H "pattern" <path/to/file>
```

### To hide the filename
```
  grep -h "pattern" <path/to/file>
```

### To stop after a specified number of matching lines
```
  grep -m "pattern" <path/to/file>
```

### To suppress error messages
```
  grep -s "pattern" <path/to/file>
```

## Regular expression
### To enable extended regular expressions
```
  grep -E 'pattern'
```

### To treat the patterns a fixed string, not regex
```
  grep -F "pattern" <path/to/file>
```

### To use basic regular expression; default mode
```
  grep -G "pattern" <path/to/file>
```

### To use perl-compatible regular expressions
```
  grep -P "pattern"{value} <path/to/file>
```

### Search for multiple patterns 
```
  grep -e 'pattern1' -e 'pattern2' <filename>
```

### To read search patterns from a file
```
  grep -f "patterns" <filename>
```

## Advanced options

### To show byte offset of matching
```
  grep -b "pattern" <filename>
```

### To treat NULL character as the line separator
```
  grep -z "pattern"  <filename>
```

### To flush output after every line
```
  grep --line-buffer "pattern" <filename>
```

### To set a label for standard input
```
  cat <filename> | grep --label=<filename> "pattern" <path/to/file>
```

### To control binary-files handling
```
  grep --binary-file=type "pattern" <filename>
```
