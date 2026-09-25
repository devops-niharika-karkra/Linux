# Command: awk
**_awk_** is text-processing command used to analyze, filter, and manipulate structured data such as logs, CSV files, and command output.

## Basic Syntax
```
  awk [options] 'pattern {actions}' input-file > output-file
```

### Show servers with CPU > 80 
```
  awk'$3 > 80 {print $1, @3}' server.txt
```

### Count servers
```
awk 'END {print NR}' server.txt
```
### Skip header and show file
```
awk 'NR > 1 {print $1,$2}' file.txt
```
### Count ERROR lines
```
awk '/ERROR/ {count++} END {print count}' app.log
```
### Calculate total
```
awk '{sum += $5} END {print sum}' data.txt
```
### some other command
```
awk 'NR > 1'
```
```
awk 'NR == 2'
```
```
awk 'BEGIN {...}'
```
```
awk 'END {...}'
```

