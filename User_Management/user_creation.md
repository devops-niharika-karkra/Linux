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

## Discussing both the methods in details:

  - 
