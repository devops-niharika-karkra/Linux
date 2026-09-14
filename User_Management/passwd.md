# passwd Command

## _passwd_ command is used to create or reset the passwd of user. 

## Basic syntax:
```
  passwd [OPTIONS] [USER]
```

## Use-Cases of passwd command

### To change your own passwd:
```
  passwd
```

### To change another user's password:
```
  sudo passwd [user]
```

### To force a user to change password on next login
```
  sudo passwd -e [user]
```

### To set age of password
```
  sudo passwd -x [number of days] [user]
```

### To set minimum number of days between password changes
```
  sudo passwd -n [number of days] [user]
```

### To set the warning days before a password expires
```
  sudo passwd -w [number of days] [user]
```

### To lock the user's account
```
  sudo passwd -l <username>
```

### To unlock the user's account
```
  sudo passwd -u <username>
```

### To set no password or delete password
```
  sudo passwd -d <username>
```

### To show status of user account
```
  sudo passwd -S <username>
```

<img width="460" height="53" alt="image" src="https://github.com/user-attachments/assets/87aa4fa3-d2a2-4d9a-87a7-cdade217068d" />

|Field|Example Value|Description|
|:---:|:-----------:|:---------|
|Status| P | Usable Password|
|| L | Locked |
|| NP | No Password |
|Last Changed| 2026-07-06 | The date the password was last changed|
|Min age|0|Minimum days required before the password can be changed|
|Max age|99999|Maximum days the password remain valid|
|Warning|7|Number of days before expiration when user gets warning|
|Inactive|-1|Number of days until which user can set password after pass expiration before account deactivation|


