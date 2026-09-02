# Command: cp
***cp*** stand for copy. It allows you to copy files, folder, and directories within the Linux system.

## Basic Syntax
```
  cp [options] <source> <destination>
```

## Use-Case of cp

### To copy the file into new file
```
  cp <source_file> <destination_file>
```

### To copy the file to a directory
```
  cp <source_file> path/to/directory 
```

### To copy multiple files in a Directory
```
  cp <file1> <file2> <file3> /path/to/directory
```

### To copy an entire directory to a specific location
```
  cp -r /Source/Destination /Destination/folder
```

### To ask for confirmation before coping the file.
```
  cp -i <file1> <file2>
```

### To display the output what files are being copied.
```
  cp -v <file1> <file2>
```

### Retains the original file modifications times, access times, and permissions.
```
  cp -p <file1> <file2>
```

### You can use wildcards like * to copy multiple files that match a specific extension or pattern. 
For example, to copy all text files into a backup folder
```
  cp *.txt /destination 
```
