# Group Management
**Group management** is used to organize users and give permissions to access files, directories and system resources. Instead of giving permissions to each user separately, we assign permissions to a Group and add members in it to whom we need to assign those permissions.

## Types of Groups
There are two types of Groups i.e.,
  - **Primary Group**: Primary Group is the default Group assigned to a user when account is created. Each user can have only one primary Group. 
  - **Secondary Group**: Secondary Group is created separately and used to grant additional permission. A user can be a member of multiple Groups.

## Group details are stored as follows:
  - The Group's basic information such as Group id, name, members are stored in /etc/Group.
  - The Group passwords are stored in encrypted form in /etc/gshadow.


## Commands to create secondary Group
  

