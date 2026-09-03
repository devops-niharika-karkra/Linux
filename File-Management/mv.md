# Command: mv
***mv*** stand for moving a directory. This command is used to move a file from current location
to desired location and also to rename a file or directory in the same location.

## Basic Syntax
```
  mv [Options] source destination
```

## Use-Cases of mv

### To rename the file 
```
  mv old-file.txt new-file.txt
```

### To move file from current location to destination location
```
  mv <file-name> path/to/destination
```

### To get promts before overwiting
```
mv -i <source_file> <destination_file>

```
### To get no prevents before overwriting
```
mv -n <source_file> <destination_file>

```
### To show output what is being done 
```
mv -v <source_file> <destination_file>

```
### To move multiple file in single directory
```
mv <file1 file2 file3 destination_directory>

```
### mv command using wildcard 
```
mv *.txt destination_directory

```

### Renaming Multiple Files
With a bit of creativity, you can rename multiple files:
```
for file in *.txt; do mv "$file" "${file%.txt}.bak"; done
```
### Use mv -u to move files only when the source file is newer than the destination file or when the destination file is missing.
Combine mv with find to move files based on criteria:
```
find . -name "*.log" -exec mv {} log_files/ \;

