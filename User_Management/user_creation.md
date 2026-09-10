# User Creation

## Ways to create user in Linux:

  - **_useradd_**: This method of creating user is non-interactive, i.e we have to create the things like password, home-directory, etc manually.
  - **_adduser_**: This method of creating user is interactive, i.e prompts you step-by-step.

## Lets look at the difference between these two methods:

|    Features    |     useradd     |    adduser    |
|:--------------:|:---------------:|:-------------:|
| Interactivity  | Non-Interactive | Interactive   |
| Best for       | Automation & Bash-scripting | Quick manual user |
| Home-Directory | not created by default (requires -m to flag) | Automatically created |
| Password setup | set with passwd cmd | prompts you to set a password |
| Availability   | Universal- available in all distros | Provides debian, ubuntu, RHEL, CentOS, etc |

---

## Use-Cases of useradd:

### Creating only user
 ```
   sudo useradd <username>
 ```

<img width="630" height="92" alt="image" src="https://github.com/user-attachments/assets/88c9ed78-d7e3-4341-850f-e12e0ca09117" />

### Deleting user
```
  sudo userdel <username>
```

<img width="641" height="28" alt="image" src="https://github.com/user-attachments/assets/dc2b3855-2661-43f9-ac74-e9636ea8cce3" />

### Creating user with home directory
  This command helps to assign a pre-defined directory as a home-directory of user manually.
```
  sudo useradd -d path/to/dir <username>
```

<img width="776" height="346" alt="image" src="https://github.com/user-attachments/assets/d76267f5-dbdb-4234-a9c2-5bfc6681860f" />

### Deleting user with home directory
home directory must have the ownership of user
```
  sudo userdel -r <username>
```

<img width="782" height="122" alt="image" src="https://github.com/user-attachments/assets/750502cc-bc94-4ee9-927d-be7812982d30" />

### Creating user with home directory.
No need to assign any directory manually
```
  sudo useradd -m <username>
```
<img width="782" height="146" alt="image" src="https://github.com/user-attachments/assets/2fae1372-dff1-4f27-a0d8-f6fdce998876" />

### Deleting user with home directory
```
  sudo usermod -r <user-name>
```

<img width="783" height="175" alt="image" src="https://github.com/user-attachments/assets/fa4e3aac-b267-4e9b-9971-b56e965d239c" />

### creating user with password

```
  sudo useradd -m -p $(openssl passwd -6 "123456") demo 
```
<img width="1028" height="185" alt="image" src="https://github.com/user-attachments/assets/180c3972-2203-43c6-acce-848ce4ec7107" />

### Creating user to get the prompt to change password on first login
```
  sudo useradd -m -p $(openssl passwd -6 "123456") demo && sudo chage -d -0 <user-name>
  or
  sudo passwd -e <user-name>
```

### Creating user with an expiry date
```
  sudo useradd -e <date> <user-name>
```

### creating user with description 
```
  sudo useradd -c "Write user description here..." <user-name>
```

### Create a User with a Specific Login Shell
```
  sudo useradd -s /bin/<shell-name> <user>
```

## Use-Cases of adduser

### Creating an user
```
  sudo adduser <username>
```
Once you run this command a user creation wizard runs and you will have to fill all the necessary information it will ask for. Otherwise you will get difficulty in sorting user.

<img width="700" height="450" alt="image" src="https://github.com/user-attachments/assets/e13f26a8-aab8-4bff-aa71-c84037675306" />

### Creating an user with a specific login shell
```
  sudo adduser <username> --shell </path/to/shell>
```

<img width="700" height="400" alt="image" src="https://github.com/user-attachments/assets/90f80614-f8d2-4b7d-8a67-05ae29449dee" />

### Creating user without home directory
```
  sudo adduser --no-create-home <username>
```

<img width="700" height="400" alt="image" src="https://github.com/user-attachments/assets/b87f3899-b748-4a65-a592-083af5b59ef7" />

### Creating user with different configuration file
```
  sudo adduser <username> --conf <filename.conf>
```

### 
