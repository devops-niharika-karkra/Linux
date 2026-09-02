# Command: mkdir
***mkdir*** stands for make directory. It is used to create one or multiple directories 

### Syntax
```
  mkdir [options] <dir_name>
```

### For creating single directory
```
  mkdir <dir-name>
```

### For creating multiple directories
```
  mkdir <dir1> <dir2> <dir3>
```

### For creating parent directory
```
  mkdir -p parent/child
```

### For getting confirmation when directory creation is completed
```
  mkdir -v <dir_name>
```

### For creating multiple directories using array
```
  mkdir dir{1..3}
```

---

# rmdir

***rmdir*** stands for remove directory. It let you delete empty directories.

### To remove an empty directory:
```
  rmdir <directory-name>
```

### For removing parent directory
```
  rmdir -p parent/child
```
### To display the message after removing the directory
```
  rmdir -v dir1 dir2 dir3
```
