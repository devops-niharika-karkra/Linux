# User Modification

## usermod:
is a command-line utility for modifying user account. You can use it to add a user to group, rename a user, an expiry date, and many more.

###  Command Syntax
```
  usermod [OPTIONS] USER
```

### To Add user in a supplementary group
```
  sudo usermod -aG <group> <user>
```

### To change primary group of a user
```
  sudo usermod -g <groupname> <username>
```

### To set expiration date of user
```
  sudo usermod -e <date> <username>
```

### To create/modify home directory 
```
  sudo usermod -d /path/to/home <username> 
```

### To move content to new location from current home directory
```
  sudo usermod -d /new/home/directory -m <username>
```

### To change the shell of user
```
  sudo usermod -s /to/path/shell <username>
```

### To assign a UID
```
  sudo usermod -u <id> <username>
```

### To lock a user 
```
  sudo usermod -L <username>
```

### To rename user 
```
  sudo usermod -l <oldname> <newname>
```

### To unlock user 
```
  sudo usermod -U <username>
```
