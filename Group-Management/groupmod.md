#  Command: groupmod
**_groupmod_** is a Linux command that is used to modify the properties of group.
This command can help in doing:
  - Change the group name
  - Group id
  - Attributes

## Basic Syntax
```
  usermod [OPTIONS] [Groupname]
```

## Use-cases of groupmod

### To add users as members of the group 
```
  sudo groupmod -U <user1,user2,user3,...>
```

### To append users to the existing members list of a group
```
  sudo groupmod -a <user1,user2,user3,..>
```

### To rename a group
```
  sudo groupmod -n new_name old_name
```

### To change groug ID to the specified value.
```
  sudo groupadd -g <gid> <groupname>
```

### To change the group password.
```
  sudo groupadd -p <password> <groupname>
```
