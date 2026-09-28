# Command: xargs

# ``xargs``
`` xargs `` is used to build and execute command lines from standard input
Some commands like grep can accept input as parameters, but some commands accepts arguments, this is place where xargs came into picture.
### Basic syntax 
```
xargs [option] [command] [initial-arguments]
```
### To create multiple files
```
echo "file1 file2 file3" | xargs touch 
```

### Create multiple directories
```
echo "dev test prod" | xargs mkdir
```
### Delete multiple files
```
echo "old1.log old2.log old3.log" | xargs rm
```
### Find and delete .tmp files
```
find /tmp -name "*.tmp" -print0 | xargs -0 rm
```

5. Search for a word in multiple files
```
find . -name "*.log" -print0 | xargs -0 grep "ERROR"
```

6. Count lines in multiple files
```
find /var/log -name "*.log" -print0 | xargs -0 wc -l
```

7. Run a command for each item
```
echo "server1 server2 server3" | xargs -n1 echo
```




## Important xargs options to learn
|Option	|Purpose|
|:-----:|:-----:|
|-n 1|	One argument per command|
|-0 |Handle filenames separated by NULL|
|-I {}|	Use a placeholder|
|-P	|Run commands in parallel|              
|-t	|Show the command before executing|
|-r|	Don't run command if input is empty|
