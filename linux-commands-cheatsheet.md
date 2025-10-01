**comprehensive list of important Linux commands with their usage**, grouped by category so it’s easier to revise:



# 📌 **Basic Linux Commands**

| Command        | Usage                                                  |
| -------------- | ------------------------------------------------------ |
| `pwd`          | Prints the current working directory.                  |
| `ls`           | Lists files and directories in the current directory.  |
| `ls -l`        | Lists in long format (permissions, owner, size, date). |
| `ls -a`        | Lists hidden files also.                               |
| `cd <dir>`     | Changes the current directory.                         |
| `cd ..`        | Moves one directory up.                                |
| `cd ~`         | Goes to the home directory.                            |
| `mkdir <dir>`  | Creates a new directory.                               |
| `rmdir <dir>`  | Deletes an empty directory.                            |
| `touch <file>` | Creates a new empty file.                              |
| `echo "text"`  | Prints text to the terminal.                           |
| `clear`        | Clears the terminal screen.                            |


# 📌 **File Operations**

| Command                | Usage                                               |
| ---------------------- | --------------------------------------------------- |
| `cat <file>`           | Displays file content.                              |
| `more <file>`          | Views file content page by page.                    |
| `less <file>`          | Similar to `more` but allows scrolling up and down. |
| `head -n <num> <file>` | Displays first *n* lines of a file.                 |
| `tail -n <num> <file>` | Displays last *n* lines of a file.                  |
| `cp <src> <dest>`      | Copies a file or directory.                         |
| `mv <src> <dest>`      | Moves or renames a file or directory.               |
| `rm <file>`            | Removes a file.                                     |
| `rm -r <dir>`          | Removes a directory recursively.                    |
| `file <filename>`      | Shows file type.                                    |
| `wc <file>`            | Counts words, lines, characters.                    |



# 📌 **Permissions & Ownership**

| Command                   | Usage                            |
| ------------------------- | -------------------------------- |
| `ls -l`                   | Shows file permissions.          |
| `chmod 755 <file>`        | Changes permissions (rwxr-xr-x). |
| `chown user:group <file>` | Changes file ownership.          |
| `umask`                   | Shows/sets default permissions.  |



# 📌 **Searching & Finding Files**

| Command                       | Usage                                   |
| ----------------------------- | --------------------------------------- |
| `find /path -name <filename>` | Finds file by name.                     |
| `locate <filename>`           | Quickly finds file using database.      |
| `grep "text" <file>`          | Searches for text inside a file.        |
| `grep -r "text" <dir>`        | Searches recursively in a directory.    |
| `which <command>`             | Shows path of a command.                |
| `whereis <command>`           | Shows location of command and man page. |



# 📌 **Process Management**

| Command         | Usage                                             |
| --------------- | ------------------------------------------------- |
| `ps`            | Lists running processes.                          |
| `ps aux`        | Lists all processes with details.                 |
| `top`           | Displays running processes dynamically.           |
| `htop`          | Better interactive version of top (if installed). |
| `kill <pid>`    | Kills a process with process ID.                  |
| `kill -9 <pid>` | Force kills a process.                            |
| `jobs`          | Lists background jobs.                            |
| `fg %1`         | Brings job 1 to foreground.                       |
| `bg %1`         | Resumes job 1 in background.                      |



# 📌 **Networking**

| Command                       | Usage                                              |
| ----------------------------- | -------------------------------------------------- |
| `ping <host>`                 | Tests connectivity to a host.                      |
| `curl <url>`                  | Fetches content from a URL.                        |
| `wget <url>`                  | Downloads files from the internet.                 |
| `ifconfig`                    | Shows network interfaces (deprecated, use `ip a`). |
| `ip a`                        | Shows IP addresses.                                |
| `netstat -tulnp`              | Shows open ports and listening services.           |
| `ssh user@host`               | Connects to remote server via SSH.                 |
| `scp <src> <user@host:/path>` | Copies files over SSH.                             |



# 📌 **Disk & Storage**

| Command                | Usage                                      |
| ---------------------- | ------------------------------------------ |
| `df -h`                | Shows disk usage in human-readable format. |
| `du -sh <dir>`         | Shows size of a directory.                 |
| `mount <device> <dir>` | Mounts a device.                           |
| `umount <device>`      | Unmounts a device.                         |
| `lsblk`                | Lists block devices.                       |
| `fdisk -l`             | Lists partitions.                          |



# 📌 **User Management**

| Command              | Usage                      |
| -------------------- | -------------------------- |
| `whoami`             | Shows current user.        |
| `who`                | Shows logged-in users.     |
| `id`                 | Shows user ID and groups.  |
| `adduser <username>` | Adds a new user.           |
| `passwd <username>`  | Changes user password.     |
| `su <user>`          | Switches to another user.  |
| `sudo <command>`     | Runs command as superuser. |



# 📌 **Archiving & Compression**

| Command                       | Usage                           |
| ----------------------------- | ------------------------------- |
| `tar -cvf file.tar <dir>`     | Creates tar archive.            |
| `tar -xvf file.tar`           | Extracts tar archive.           |
| `tar -czvf file.tar.gz <dir>` | Creates compressed tar archive. |
| `tar -xzvf file.tar.gz`       | Extracts compressed archive.    |
| `zip file.zip <file>`         | Creates zip archive.            |
| `unzip file.zip`              | Extracts zip archive.           |



# 📌 **Package Management**

(Depends on Linux distribution)

### Ubuntu/Debian

| Command             | Usage                        |
| ------------------- | ---------------------------- |
| `apt update`        | Updates package list.        |
| `apt upgrade`       | Upgrades installed packages. |
| `apt install <pkg>` | Installs a package.          |
| `apt remove <pkg>`  | Removes a package.           |

### RedHat/CentOS

| Command             | Usage               |
| ------------------- | ------------------- |
| `yum install <pkg>` | Installs a package. |
| `yum remove <pkg>`  | Removes a package.  |



# 📌 **System Info & Monitoring**

| Command    | Usage                   |
| ---------- | ----------------------- |
| `uname -a` | Shows system info.      |
| `hostname` | Shows system hostname.  |
| `uptime`   | Shows system uptime.    |
| `free -h`  | Shows memory usage.     |
| `vmstat`   | Performance statistics. |
| `iostat`   | CPU & I/O stats.        |
| `dmesg`    | Kernel boot messages.   |



# 📌 **Other Useful Commands**

| Command             | Usage                            |
| ------------------- | -------------------------------- |
| `history`           | Shows command history.           |
| `alias ll="ls -la"` | Creates shortcut alias.          |
| `date`              | Shows current date and time.     |
| `cal`               | Displays calendar.               |
| `man <command>`     | Opens manual page for a command. |
| `exit`              | Logs out of terminal.            |


✅ This list covers **most commonly used Linux commands** you’ll need for administration, development, or interviews.

