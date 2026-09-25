# Command: cut
**_cut_** command is used to extract specific parts of each line from a line or input based on byte position, character position 
and fields separated by a delimiter like space, tabs or custom character.

## Basic Syntax:
```
  cut OPTION... [FILE]..
```

## Use-case of cut 

### Extract by byte position
```
  cut -b <number-of-bytes> <filename>
```
here, number of bytes can be specified in group of numbers separated by commas, range of numbers like (1-4), 
from beginning to end (1-), or from beginning to specific position (-4).

### Extract by character position.
```
  cut -c <number-of-characters> <filename>
```
here, number of characters can be specified in group of numbers separated by commas, range of numbers like (1-4), 
from beginning to end (1-), or from beginning to specific position (-4).

### Extract by field
```
  cut -d "delimiter" -f (field number) file.txt
```
here, number of fields can be specified in group of numbers separated by commas, range of numbers like (1-4), 
from beginning to end (1-), or from beginning to specific position (-4).

### Invert the Selected Fields or Characters, it prints everything except the selected fields
```
  cut --complement -d "delimiter" -f (field number) file.txt
```

### Change the Output Field Separator
```
  cut -d "delimiter" -f (field number) file.txt --output-delimiter=''
```
