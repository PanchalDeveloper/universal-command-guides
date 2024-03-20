# Linux Commands Guide

## System Information

- `uname -a`: Display all system information
- `hostname`: Show or set the system's host name
- `uptime`: Tell how long the system has been running
- `whoami`: Print the user name associated with the current effective user ID

## File Operations

- `ls`: List directory contents
- `cp`: Copy files and directories
- `mv`: Move (rename) files
- `rm`: Remove files or directories
- `mkdir`: Create new directories
- `touch`: Change file timestamps or create empty files

## Process Management

- `ps`: Report a snapshot of the current processes
- `top`: Display Linux processes
- `kill`: Send a signal to a process
- `pkill`: Send a signal to a process based on name or other attributes

## File Permissions

- `chmod`: Change file mode bits
- `chown`: Change file owner and group
- `umask`: Set the default file permissions

## Networking

- `ping`: Send ICMP ECHO_REQUEST to network hosts
- `ifconfig`: Configure a network interface
- `netstat`: Print network connections, routing tables, interface statistics, masquerade connections, and multicast memberships
- `ss`: Another utility to investigate sockets

## Disk Usage

- `df`: Report file system disk space usage
- `du`: Estimate file space usage

## Searching and Sorting

- `grep`: Print lines that match patterns
- `find`: Search for files in a directory hierarchy
- `sort`: Sort lines of text files

## Piping and Redirection

- `|`: Pipe; the output of one command becomes the input to another
- `>`: Redirect standard output (overwrite)
- `>>`: Redirect standard output (append)
- `<`: Redirect standard input

## Examples of Piping

- `ls -l | less`: View a paginated list of detailed directory contents
- `ps aux | grep firefox`: Find all processes related to Firefox
- `cat file.txt | sort | uniq`: Sort a file and remove duplicate lines

## Package Management

- `sudo apt update`: Update package lists
- `sudo apt upgrade`: Upgrade all packages
- `sudo apt install [package]`: Install a new package
- `sudo apt remove [package]`: Remove an installed package

## System Monitoring and Management

- `htop`: Interactive process viewer (similar to `top` but more advanced)
- `iotop`: View I/O usage information
- `nmon`: Performance monitoring tool
