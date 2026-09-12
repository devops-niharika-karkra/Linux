# w Command
**_w_** is a command displays who is logged on and what they are doing.

### Basic output detail:

- USER: Name of the logged-in user
- TTY: Terminal session type (ttyX for physical consoles, pts/X for SSH or terminal emulators)
- FROM: Login source (IP address, hostname, or :0 for local) of the user
- LOGIN@: Login time of the user
- IDLE: Time user has been inactive
- JCPU: Total CPU time used by all processes attached to the terminal
- PCPU: CPU time used by the command listed in WHAT
- WHAT: Current process the user running in the session
  
### The w Command Can be Used:

- To see who is logged in and from where
- To track what command or process each user is executing
- To detect idle or forgotten sessions
- To verify unexpected remote logins
- To diagnose load or performance issues

