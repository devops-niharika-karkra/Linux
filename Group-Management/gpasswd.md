# Command: gpasswd
**_gpasswd_** command is used to set/remove password, add/remove users in groups, and  add restrictions to groups.

## Basic Syntax:
```
  gpasswd [OPTION] [group]
```

## Use-Cases of gpasswd

### To add a user to group
```
  gpasswd -a <username> <groupname>
```

### To remove user from group
```
  gpasswd -r <username> <groupname>
```

### To set a password for a group 
```
  sudo gpasswd <groupname>
```

### To remove the password from a group
```
  sudo gpasswd -r <groupname>
```

### To restrict the access to group
```
  sudo gpasswd -R <groupname>
```

### To set the list of administrative users
```
  sudo gpasswd -A <user1, user2, user3,...> <groupname>
```

### To set the list of group members
```
  sudo gpasswd -M <user1, user2, user3,...> <groupname>
```
