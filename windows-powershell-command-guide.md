# Windows 11 PowerShell Commands Guide

## System Information

- `systeminfo`: Display detailed configuration information about a computer and its operating system, including operating system configuration, security information, product ID, and hardware properties.

## File Operations

- `Get-ChildItem`: List files and directories in the current directory.
- `Copy-Item`: Copy files and directories.
- `Move-Item`: Move (rename) files and directories.
- `Remove-Item`: Remove files or directories.
- `New-Item`: Create new files or directories.
- `Set-ItemProperty`: Change the value of a property of an item.

## Process Management

- `Get-Process`: Get information about processes running on the local computer.
- `Stop-Process`: Stop one or more running processes.
- `Start-Process`: Start one or more processes, optionally as a specific user.

## File Permissions

- `Get-Acl`: Get the security descriptor for a file or directory.
- `Set-Acl`: Set the security descriptor for a file or directory.

## Networking

- `Test-NetConnection`: Test network connection to a computer.
- `Test-Connection`: Test the connection to a remote computer by sending ICMP echo request packets.
- `Get-NetIPAddress`: Retrieve IP address configuration information.

## Disk Usage

- `Get-Volume`: Get information about volumes on a computer.
- `Get-Disk`: Get information about disks on a computer.
- `Get-Partition`: Get information about disk partitions on a computer.

## Searching and Sorting

- `Select-String`: Search for patterns in text files.
- `Sort-Object`: Sort objects by property value.

## Piping and Redirection

- `|`: Pipe; the output of one command becomes the input to another.
- `>`: Redirect standard output (overwrite).
- `>>`: Redirect standard output (append).
- `<`: Redirect standard input.

## Examples of Piping

- `Get-ChildItem | Where-Object { $_.Name -like "*.txt" }`: List only .txt files in the current directory.
- `Get-Process | Sort-Object CPU -Descending | Select-Object -First 5`: List top 5 processes by CPU usage.

## Package Management

- `winget`: Windows Package Manager command-line tool for installing, updating, and managing software packages.

## System Monitoring and Management

- `Get-WmiObject`: Get instances of WMI classes or information about the available classes.
- `Get-EventLog`: Get the events in the event logs on a local or remote computer.
