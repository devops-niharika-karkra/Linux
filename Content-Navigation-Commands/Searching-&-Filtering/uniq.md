# command: uniq
The **_uniq_** command in Linux use to detect the adjacent duplicate line and also deletes the duplicate lines. 

## Basic Syntax:

```
uniq [OPTION] [INPUT[OUTPUT]]
```

## Use-cases of uniq: 

### In order to omit the repeated lines from a file, the syntax would be the following:

```
uniq kt.txt
```

### In order to tell the number of times a line was repeated, the syntax would be the following:

```
uniq -c kt.txt
```

### In order to print repeated lines, the syntax would be the following:

```
uniq -d kt.txt
```

### In order to print unique lines, the syntax would be the following: 

```
uniq -u kt.txt
```

### In order to allows the N fields to be skipped while comparing uniqueness of the lines, the syntax would be the following:

```
uniq -f 2 kt.txt
```

### In order to allows the N characters to be skipped while comparing uniqueness of the lines, the syntax would be the following:

```
uniq -s 5 kt.txt
```

### In order to to make the comparison case-insensitive, the syntax would be the following:

```
uniq -i kt.txt
```
