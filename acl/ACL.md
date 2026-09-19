# acl 
**_acl_** stands for Access Control List. It allow us to set specific permissions for individual user and groups. ACL Allow us to set permissions in a detailed manner giving us greater flexibility and control over who can access what.

## Uses of acl:
  - Granular control: Assign permissions to individual user or group without changing the file's ownership.
  - Flexibility: Manage access for multiple users or group with different permission levels.
  - Enhanced Collaborations: Share files and directories securely in multi-user environments.

## We have following commands to work with acl
`getacl` : We use this command to view the permissions are given to file or directory.

`setacl`: We use this command to set the permissions.

## Let's learn about getfacl in detail.

### Basic Syntax:
```
  getfacl [OPTIONS] [file|dir]
```

### To display default Access Control List.
```
  getfacl -d <Name>
```

### To display ACLs with Numeric User and group IDs
```
  getfacl -n <Name>
```

### To view ACLs without headers
```
  getfacl -c <Name>
```

### To list all the files or directories recursive acl view.
```
  getfacl -R <Name>
```

### To display ACLs in raw format. 
```
  getfacl -e <Name>
```

### To display extended attributes
```
  getfacl -d <Name>
```

### To display ACLs for multiple files.
```
  getfacl <Name1,Name2,Name3>
```

## Let's learn about setfacl in detail.

### Basic Syntax
```
  setfacl [OPTIONS] [file|dir]
```

### Use-cases of setfacl
### ACL entries follows a specific format:
```
  [entry_type]:[name]:[permissions]
```

### To set ACL for a group
```
  setfacl -m g:<name>:<permissions> <Name-of-file/dir>
```

### To remove ACL entries.
```
  setfacl -x u:<user> <Name>
```

### To remove all ACL entries.
```
  setfacl -b <Name-of-file/dir>
```

### To set default ACL for a directory
```
  setfacl -d -m g:developer:<permission> <Name>
```

### To set mask permissions.
```
  setfacl -m m::<permissions> <Name>
```

To set ACL to a directory and all its contents.
```
  setfacl -R -m u:<username>:<Permission> <Directory>
```
