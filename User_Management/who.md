# who command
This command is used to display the information about the currently logged in users.

## Basic Syntax
who <OPTIONS>

### Use-Cases of who command 

### To display all the information same as -b -d --login -p -r -t -T -u
```
  who -a 
```

### To display time of last boot 
```
  who -b
```

### To display column headings.
```
  who -H
```

### To display system login process.
```
  who -l
```

### To attempt to canonicalize hostnames via DNS
```
  who --lookup
```

### To display current runlevel
```
  who -r
```

### To display all login names and number of users logged on 
```
  who -q
```

### To display list of users logged in
```
  who -u
```

#WARNING: Modern versions of systemd have officially dropped utmp support due to which who from coreutils has nothing to read and simply outputs a blank line.
