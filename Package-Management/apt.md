# Package Manager: apt

**Linux Package Management** is  responsible for installing, configuring and removing software packages. Each Linux has its own package management system.

### What is a package?
A package in Linux is a collection of files bundled together to provide a piece of software.

### To update package list in Linux
```
  sudo apt update
```

### To update installed packages in Linux
```
  sudo apt upgrade 
```
to avoid manual confirmation add -y to command


### To upgrade the package with the ability to add or remove dependencies to resolve conflicts.
```
  sudo apt dist-upgrade <package-name>
```

### To install a package in Linux
```
  sudo apt install <package>
```

### To install a package with automatic confirmation
```
  sudo apt install <package>  -y
```

### To reinstall a package
```
  sudo apt reinstall <package>
```

### To remove package.
```
  sudo apt remove <package> 
```

### To remove packages with its all dependencies.
```
  sudo apt purge <package-name>
```

### To search for packages 
```
  sudo apt search <packages>
```

### To show information regarding packages.
```
  sudo apt show <packages>
```

### To remove the packages that were installed as dependencies with other packages and no longer needed.
```
  sudo apt autoremove
```

### To delete all cached package files
```
  sudo apt clean
```

### To remove the packages that are no longer useful.
```
  sudo apt autoclean
```

### To add repository
```
  sudo add-get-repository <name-of-repository>
```

### To lock package version to avoid upgrade 
```
  sudo apt-mark hold <package>
```

### To unlock a package
```
  sudo apt-mark unhold <package>
```

### To view all locked packages 
```
  sudo apt-mark showhold
```
