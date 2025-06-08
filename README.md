## Shell Scripting
#### Basic commands:
- `pwd` : Prints the current working directory path. 
- `ls` : Lists files and folders in the current directory.  
- `ls -ltr` : Lists files and folders with its properties. 
- `clear` : Clears the terminal screen.
- `chmod` : Changes file permissions, commonly used to make scripts executable.
- `man` : Shows manual/help page for a command.
- `whoami` : Shows current logged-in user.

#### Processing and management commands:
- `free` : Shows memory usage.  
- `nproc` : Displays the number of CPU cores.  
- `df` : Shows disk usage of mounted file systems.  
- `top` : Displays real-time system processes and resource usage.
- `ps -ef` : Lists all running processes with full details.  
- `ps -ef | grep "processname"` : Searches for a specific process by name.  
- `kill <pid>` : Terminates the process with the given process ID.  
- `trap` : Defines actions to take when the script receives specific signals. 

#### Working with files and directories:
- `touch filename` : Creates a new empty file.  
- `vi filename` : Opens file in vi editor for editing.  
- `wq!` : Saves and exits the vi editor forcefully.  
- `cat filename` : Displays the content of a file.  
- `mkdir dirname` : Creates a new directory.  
- `rm filename` : Deletes a file.  
- `rmdir` or `rm -r dirname` : Recursively deletes a directory and its contents. 
- `cd` : Changes to a different directory

  - `cd /path/to/directory` : Go to a specific directory using absolute path.
  - `cd directory_name` : Go to a directory using relative path.
  - `cd ..` : Move one level up to the parent directory.
  - `cd ../..` : Move two levels up in the directory hierarchy.
  - `cd ~` or just `cd` : Go to the current user's home directory.
  - `cd -` : Switch to the previous directory.
  - `cd /` : Go to the root directory.
  - `cd ~/Desktop` : Go to the Desktop directory inside home.
  - `cd ~username` : Go to another user's home directory (if accessible).
  - `cd .` : Stay in the current directory (useful in scripting for clarity).
- `mv oldname newname` : Renames a file or moves it to another location.  
- `mv file /path/to/dir` : Moves a file into another directory. 
- `sort filename` : sorts the content of the file. 

##### Shebangs and Shell Types:
- `#!/bin/bash` : Runs the script using the Bash shell.  
- `#!/bin/dash` : Runs the script using Dash (a faster, lightweight shell).  
- `#!/bin/sh` : Runs the script using the default system shell (usually Bash or Dash).  
- `#!/bin/ksh` : Runs the script using KornShell (KSH), used in some Unix systems.

#### Script control and debugging:
- `set -x` : Prints each command and its arguments as they are executed (debug mode).  
- `set -e` : Stops script execution if any command returns a non-zero exit status.  
- `set -o pipefail` : Makes the script fail if any command in a pipeline fails.  
- `set -exo pipefail` : Combines `-e`, `-x`, and `-o pipefail` for robust and verbose debugging.  

#### Text processing and searching:
- `awk` : A text-processing tool used for filtering and extracting data from files.  
- `|` (pipe) : Passes output of one command as input to another (used with grep, awk, etc.).  
- `script | grep 5` : Example of filtering the output of a script for lines containing "5".  
- `getmeusernames | grep` : Searches usernames from a command’s output (example placeholder).  

#### Downloading and networking:
- `curl` : Transfers data from or to a server using protocols like HTTP, FTP.  
- `wget` : Downloads files from the web via HTTP, HTTPS, or FTP.  

#### Permissions and privilege elevation:
- `sudo` : Runs a command with superuser privileges.  
- `sudo su` : Switches to the root user with full administrative access. 
