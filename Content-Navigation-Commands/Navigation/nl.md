# Command  ``nl``
The ``nl`` (number lines) command is used to display the contents of a file with line numbers.

## Basic syntax:
```
nl [OPTIONS] [file]
```
### Number all lines

### By default, blank lines are not numbered.
```
nl file.txt
```
### To number every line:
```
nl -b a file.txt
```
### Start numbering from a specific number
```
nl -v 100 file.txt
```

### Change the increment
```
nl -i 5 file.txt
```
### Add leading zeros
```
nl -n rz -w 3 file.txt
```

### Practical DevOps Examples
Check line numbers in a configuration file
```
nl /etc/ssh/sshd_config
```
### Number a shell script
```
nl deploy.sh
```

### Combine nl with a pipe

### You can number the output of another command:
```
  grep -i "error" app.log | nl
```
