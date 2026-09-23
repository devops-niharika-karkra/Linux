# Package Management: dnf 
dnf is a package manager command in Red-based Linux distros for example fedora, CentOS and RHEL.
It stands for "Dandified YUM", where  YUM is another package manager commonly used in these distributions.

## Basic Syntax
```
  sudo dnf [option] <package-name>
```

### To update your package list
```
  sudo dnf check-update
```

### To install package
```
  sudo dnf install <package-name>
```

### To remove package
```
  sudo dnf remove <package>
```

### To upgrade package installed on Linux
```
  sudo dnf upgrade
```

### To search for packages
```
  sudo dnf search <package>
```

### To show package information
```
  sudo dnf info <package>
```

### To remove packages that were automatically installed to satisfy dependencies for other packages.
```
  sudo dnf autoremove
```

### To remove all cached package files
```
  sudo dnf clean all
```

### To add repositroy
```
  sudo dnf config-manager <name>
```

### To lock a particular version of installed package
```
  sudo dnf versionlock add <package>
```

### To unlock the package upgrade
```
  sudo dnf versionlock delete <package>
```
### To temporary skip lock 
```
  sudo dnf upgrade --exclude=<package>/<package1,package2>
```
### To remove all locked packages 
```
  sudo dnf versionlock clear
```

### For wildcard patterns
```
  sudo dnf upgrade --exclude="pack*"
```
