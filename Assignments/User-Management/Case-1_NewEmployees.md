# Case-1 New Employees

### Scenario:
  A company has hired 15 employees for different departments. Each employee needs a separate Linux account.

### Question: 
  How would you create the required user accounts so that each employee gets an appropriate home directory and can login normally?

### Solution:
  First of all, collect all information about users and then will create the user.

### Ways to create user.
In this we can used three ways to create user. 
### To create user with interactive way.
Provide prompts to add password and home directory.
```
    sudo adduser <NAME>
```

<img width="745" height="350" alt="Screenshot from 2026-09-21 16-46-14" src="https://github.com/user-attachments/assets/74734f33-550f-4972-998f-5e04d6690ef8" />

### To create user with non interactive way.
Adding details for user like password, home directory, and many more manually.
```
  sudo useradd -m <NAME>
```

<img width="857" height="198" alt="Screenshot from 2026-09-21 16-48-47" src="https://github.com/user-attachments/assets/e0548b8c-82c9-41cc-8c84-df390340e140" />

### To create user with script.
we can create users in bulk by writing a script to avoid repetition.
```
while read -r user
do
  sudo useradd -m "$user"
  echo "$user:123" | sudo chpasswd
done < users.txt
```

<img width="985" height="641" alt="Screenshot from 2026-09-21 16-50-47" src="https://github.com/user-attachments/assets/27b0e54c-ac9a-46fa-9fc3-36ae44b08208" />

