### Ubuntu Commands
* apt-get update 
	- downloads latest apt-get index
* apt-get upgrade
	- installs latest version of all installed software
* apt-get install
	- installs something from the ubuntu known locations

### User Management
* sudo su -
    - switch into root user
* sudo <i>cmd</i> 
    - run command as super user
* visudo
    - edit sudoers file
* adduser <i>login</i>
    - adds a user
    
### Variables
* export "variable"=value
    - add a variable
* echo $"variable"
    - print a variable name
* unset $"variable"
	- remove variable
* Defined variables
    - $HOME
	   - home dir
	- $PATH
        - search for 

### profile settings
* sudo vi /etc/profile
    - will update profile for all users
* export PATH=$PATH:New Path
    - add path
* source /etc/profile
    - apply update profile settings
* sudo vi ~/.profile
	- will update profile for the current user

### vi commands
* i - input mode
* esc - exit to command mode
* : - run a command
    - w - write
	- q - quit
	- / start searching	
	- N - search down
	- n - search up
    - zz - center on found value

### process commands
* ps aux
    - list all process
* command with &
    - run in background
* jobs
    - list background jobs
* fg/bg 
	- move background job to foreground/background
* fg/bg #
	- move background job of number # to the foreground/background
* ctrl - z - suspend a job
* kill %1
	- kill suspended job #1
* which
    - shows where an executable is
    -  -a shows all found versions of the executable, not just the first one.

### searching commands
* ls
    - h - human readable sizes
    - p - suffix '/' for folders
    - A - all but . and ..
    - l - list format
    - r reverse
    - R recursive
* grep
    - E - extended regex (could use egrep)
* which
    - shows where an executable is
    -  -a shows all found versions of the executable, not just the first one.
* find
    - find {phrase}
        - type 
            - f - files
            - d - directories
    - you can do a lot with find         
* sort
* tail
    - tail -n 1
        list the last 1 result
* head
    - tail -n 1 
        list the first result
    - tail -f 
        tail forever - as a file is written to, there it keeps reading. very useful for log files

### services
* init.d folder contains folders that are subsystems like web server, http, network, etc.
* sudo service <i>serviceName</i> <i>start|stop|restart</i>
	- do something to a running service
		- ex: sudo service pdfreactor restart
* the '.d' suffix indicates configuration that could have been one configuration file that has been split up into multiple directories and files
* the 'init.d' folder is executed by the System V init tools (SysVinit). Some OSes are replacing it with UpStart
