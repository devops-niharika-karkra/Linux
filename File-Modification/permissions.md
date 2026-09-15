# File Permissions
## In Linux, file permissions helps us to define who can read, write and execute file and directories.
### There are three basic file permissions:
  - **_Read_**: Denoted by (r or 4), provides the permission to view the file.
  - **_Write_**: Denoted by (w or 2), provides the permission to modify or write the file.
  - **_Execute_**: Denoted by (x or 1), provides the permissions to run the file as a program.

 |Permissions|Symbolic|Numeric|
 |:---------:|:------:|:-----:|
 |Read|r|4|
 |Write|w|2|
 |Execute|x|1|

 File Permission: Operation Chart

 |Operators| Definition|
 |:-------:|:---------:|
 |+| Add permission|
 |-| Remove permission|
 |=| Set the permission to the specified value|


## Permissions are assigned to three categories of users:
  - user (owner)
  - group
  - other

## **chmod** command is used to change the file permissions.

## Basic Syntax 
```
  chmod [OPTIONS] [mode] [file]
```

## Use-Cases of chmod command

### To add permissions to all user, group and others.     
```
  chmod a+rwx <filename>  # All three permissions
```
```
  chmod a+r <filename>  #read permission
```
```
  chmod a+w <filename> #write permissions
```
```
  chmod a+x <filename> #execute permissions 
```
### To remove all permissions of all user, groupp and other.
```
  chmod a-rwx <filename>  #All three permissions
```
```
  chmod a-r <filename>  #read permission
```
```
  chmod a-w <filename>  #write permissions 
```
```
  chmod a-x <filename>  #execute permissions
```

### To add/remove permissions to user only.
```
  chmod u+/-[mode] <filename>  
```

### To add/remove permissions to group only.
```
  chmod g+/-[mode] <filename>
```

### To add/remove permissions to other only.
```
  chmod o+/-[mode] <filename>
```

## To set permissions using octal notations
```
  chmod [0-7] <filename>
```

# 0-7 Octal notations 

| 0-7 | Permissions | 
|:---:|:-----------:|
|0|---|
|1|--x|
|2|-w-|
|3|-wx|
|4|r--|
|5|r-x|
|6|rw-|
|7|rwx|
