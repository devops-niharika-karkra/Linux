# chage command
## _chage_ stands for 'change age' of user. This command is used to get information about user account and password age.

## Basic syntax 
```
  chage [options] [User]
```

## Use-Case of chage command

### To list user's current account aging information
```
  chage -l <user>
```

### To get an interactive mode to set all the values for account's age
```
  chage -i <user>
```

### To set last password change date
```
  sudo chage -d <date> <user>
```

### To set account expiry date
```
  sudo chage -E <date> <user> 
```

### To set minimum number of day
```
  sudo chage -m <Username>
```

### To set maximum number of day
```
  sudo chage -M <username>
```

### To set inactivity period after password expiry
```
  sudo chage -i <username>
```

### To set warning days before password change
```
  sudo chage -W <username>
```

### To fix user on a broken computer or a backup computer drive plugged-into your computer.
```
  sudo chage -R <username>
```
