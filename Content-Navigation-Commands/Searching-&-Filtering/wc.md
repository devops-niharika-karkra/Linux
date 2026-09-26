# Command: wc 
The **wc** command is used to count the number of words, lines, characters, and bytes in a file or standard input. 

## Basic syntax
```
 wc [OPTIONS] [filename]
```

### To count the number of lines, words and characters in a file in order:
```
 wc file.txt
```

### To count the number of directories in a directory
```
 ls -F | grep / | wc -l
```

|Short Flag | Long Flag | Description |
|-----------|-----------|-------------|
|-c|	--bytes	|print the byte counts|
|-m| --chars|	print the character counts|
|-l|	--lines|	print the newline counts|
|-|	--files0-from=F|	read input from the files specified by NUL-terminated names in file F. If F is - then read names from standard input|
|-L| --max-line-length|	print the maximum display width|
|-w|	--words|	print the word counts|
