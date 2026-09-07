# vim
*vim*: stands for 'Vi IMproved'. It is a free and open-source text editor. It is an enhanced version of vi. It is easy to work in this.
It also keeps the record of all the files or work done using the file called vim.info. 

### To open the file using vim 
```
  vim <file name> 
```

## Vim can be used in different modes. Let's have a look at them:

### Default mode: When we open a file in vim. It opens in default mode. In this mode, one can navigate, copy, and delete in a file.
<img width="993" height="663" alt="image" src="https://github.com/user-attachments/assets/5d7126eb-e669-4158-a5b2-6e9c2babb1b0" />

### Insert mode: One press "i" to enter in this mode. In this mode we can insert characters in file. 
<img width="993" height="663" alt="image" src="https://github.com/user-attachments/assets/460efa6a-d7a9-45cd-96ef-695d12c69117" />

### Command-line mode: To enter in this mode, press ":"
<img width="993" height="663" alt="image" src="https://github.com/user-attachments/assets/67fe0c0f-7451-4936-9b6f-7c18e8561f5c" />

---
## Commands that we use in vim in command-line mode: 

### To save a file:
```
  :w
```

### To quit a file.
```
  :q
```

### To save and quit a file.
```
  :qw
```

### To exit forcefully.
```
  :q!
```

### To search a word 
```
  :/<word-to-search>
```

### To do case-insensitive searching
```
  :set ignorecase
  :/<word-to-search
  :set ignorecase! #to return back to normal
```

### To search and replace word
```
  :%s/<search-word>/<replace-word>/
  :%s/<word-to-search>/<word-to-replace-with/g    #to replace words globally
```

### To display line number
```
  :set nu
  or
  :set number
```

### To display relative line number
```
  :set rnu
  or
  :set relativenumber
```

### To remove line number
```
  :set nu!
  :set nonumber
  :set nonu
```

### To remove relative line number
```
  :set rnu!
  :set norelativenumber
  :set nornu
```

---
## Commands to use in vim's normal or default mode 

###  Keys used to move cursor through-out a file 
### h: Used for left
### j: Used for down
### k: Used for up
### l: Used for right

### To delete characters: 
```
  x  #To delete single character or character under cursor
  d  #To delete single 
```
