# id 
## _id_ is used to print user's identity information. It includes username, uid, gid, and group memberships. 

## Basic Syntax
```
  id [OPTION] [USER]
```

## Use-Cases of id command

### To print current user's identity.
```
  id
```

### To print specific user's identity.
```
  id [user]
```

### To print effective gid.
```
  id -g [user]
```

### To print all group ids to which user belongs to.
```
  id -G [user]
```

### To print the uid of specific user 
```
  id -u [user]
```

### To display names instead of numbers
```
  id -nu [user]
```
```
  id -ng [user]
```
```
  id -nG [user]
```

### To display real ids instead of effective id 
```
  id -ru [user]
```
```
  id -rg [user]
```
```
  id -rG [user]
```
