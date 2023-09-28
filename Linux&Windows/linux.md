| Command              | Description                               | Example Usage                                    |
| -------------------- | ----------------------------------------- | ------------------------------------------------ |
| `ls`                 | List files and directories in the current directory. | `ls` - List files and directories in the current directory. `ls /path/to/directory` - List files and directories in a specific directory. |
| `pwd`                | Print the working directory (current directory). | `pwd` - Display the current working directory. |
| `cd`                 | Change the current directory. | `cd /path/to/directory` - Change the current directory to the specified path. `cd ..` - Move up one directory level. |
| `mkdir`              | Create a new directory. | `mkdir new_directory` - Create a new directory named "new_directory". |
| `touch`              | Create an empty file or update the timestamp of an existing file. | `touch new_file.txt` - Create a new empty file named "new_file.txt". |
| `rm`                 | Remove files or directories. | `rm file.txt` - Remove a file named "file.txt". `rm -r directory` - Remove a directory and its contents recursively. |
| `cp`                 | Copy files or directories. | `cp file.txt new_location/` - Copy a file to a new location. `cp -r directory/ new_location/` - Copy a directory and its contents to a new location. |
| `mv`                 | Move or rename files or directories. | `mv file.txt new_name.txt` - Rename a file. `mv file.txt new_location/` - Move a file to a new location. |
| `cat`                | Concatenate and display file content. | `cat file.txt` - Display the contents of a file. |
| `more` or `less`     | Display file content one screen at a time. | `more file.txt` - View file content one screen at a time using "more". `less file.txt` - View file content one screen at a time using "less". |
| `head`               | Display the beginning of a file. | `head file.txt` - Display the first few lines of a file. |
| `tail`               | Display the end of a file. | `tail file.txt` - Display the last few lines of a file. |
| `grep`               | Search for text patterns in files. | `grep pattern file.txt` - Search for a pattern in a file. |
| `find`               | Search for files and directories. | `find /path/to/search -name "*.txt"` - Search for files with a specific extension in a directory. |
| `ps`                 | List currently running processes. | `ps` - List all running processes. |
| `top`                | Display real-time system usage and process information. | `top` - Display real-time system statistics and process information. |
| `kill`               | Terminate processes by their process ID (PID). | `kill PID` - Terminate a process by its PID. |
| `chmod`              | Change file permissions. | `chmod 644 file.txt` - Change file permissions to read and write for the owner, and read-only for others. |
| `chown`              | Change file ownership. | `chown user:group file.txt` - Change the owner and group of a file. |
| `df`                 | Display disk space usage. | `df -h` - Display disk space usage in human-readable format. |
| `du`                 | Display file and directory space usage. | `du -sh directory/` - Display the total disk usage of a directory. |
| `tar`                | Archive and compress files. | `tar -czvf archive.tar.gz files/` - Create a compressed tarball of files. |
| `gzip` or `gunzip`   | Compress or decompress files. | `gzip file.txt` - Compress a file. `gunzip file.txt.gz` - Decompress a compressed file. |
| `man`                | Display manual pages for commands. | `man ls` - Display the manual page for the `ls` command. |
| `ssh`                | Securely connect to remote servers. | `ssh user@hostname` - Securely connect to a remote server. |
| `scp`                | Securely copy files between local and remote systems. | `scp file.txt user@hostname:/path/to/destination/` - Copy a file to a remote server. |
| `rsync`              | Synchronize files and directories between systems. | `rsync -av source/ destination/` - Synchronize files and directories between local and remote systems. |
| `wget` or `curl`     | Download files from the internet. | `wget URL` - Download a file from a URL using `wget`. `curl -O URL` - Download a file from a URL using `curl`. |
| `ping`               | Test network connectivity to a host. | `ping google.com` - Test network connectivity to Google's website. |
| `ifconfig`           | Display or configure network interfaces. | `ifconfig` - Display information about network interfaces. |
| `netstat`            | Display network statistics. | `netstat -tuln` - Display a list of open network ports. |
| `who`                | Display information about logged-in users. | `who` - List users currently logged in. |
| `date`               | Display or set the system date and time. | `date` - Display the current date and time. `date -s "2023-09-28 14:30"` - Set the system date and time. |
| `shutdown`           | Shutdown or restart the system. | `shutdown -h now` - Shut down the system immediately. |
| `reboot`             | Reboot the system. | `reboot` - Reboot the system. |
