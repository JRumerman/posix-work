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
