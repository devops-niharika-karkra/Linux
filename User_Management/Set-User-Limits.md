## How to set user resource limits?

We set resource limit to avoid conditions or situations like fork bomb.
These situations can cause:
  - Application Failure
  - Slow system performance
  - Login or SSH performance
  - Service interruption
  - Denial-of-service conditions
  - System instability


## What are user resource limits??
  - The user resource limit is the limit of a particular resource a user or process can consume.

###  Some commonly controlled resources:
  - Number of open files
  - Number of running processes
  - Maximum file size
  - Maximum stack size
  - CPU execution time
  - Core dump size
  - Locked memory

## Linux uses two types of user limits:
  - Soft Limit
  - Hard Limit 

## **_Soft Limit_** is the limit that is currently being applied to user or process by the operating system. The regular user can increase this limit, but new value cannot be higher than the hard limit.
  **For example**: If the hard limit is 100 then user can increase soft limit upto 100 only and cannot go beyond it.

### Basic syntax:
  ```
    ulimit <OPTIONS> 
  ```
### Basic syntax for command to set limit
```
  ulimit <OPTIONS> <value>
```
### Use-cases of soft limit: 

### To display the limits of current running shell:
```
  ulimit -a 
```

### To display the size of files written by the shell and its children:
```
  ulimit -f
```

### To set the limit 
```
  ulimit -f <value>
```

### To display the number of running processes.
```
  ulimit -u
```

### To display the Number of open files
```
  ulimit -n
```

### To display the Maximum file size
```
  ulimit -m
```

### To display the Maximum stack size
```
  ulimit -s
```

### To display the CPU execution time
```
  ulimit -t
```

### To display the Core dump size
```
  ulimit -c
```

### To display the Locked memory
```
  ulimit -l
```
