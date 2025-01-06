important  Windows commands for daily usage :
---------------------------------------------

### dir
Lists files and directories in the current directory.
Example: `dir`

### cd
Changes the current working directory.
Example: `cd C:\Users\User\Documents`

### echo %cd%
Prints the current working directory.
Example: `echo %cd%`

### mkdir
Creates a new directory.
Example: `mkdir new_directory`

### rmdir
Removes an empty directory.
Example: `rmdir empty_directory`

### del
Removes files.
Example: `del file.txt`

### rmdir /s
Removes a directory and its contents.
Example: `rmdir /s directory`

### copy
Copies files or directories.
Example: `copy file.txt new_file.txt`

### xcopy
Copies files and directories, including subdirectories.
Example: `xcopy directory new_directory /e`

### move
Moves or renames files or directories.
Example: `move file.txt new_file.txt`

### type
Displays the contents of a file.
Example: `type file.txt`

### more
Allows you to view the contents of a file one page at a time.
Example: `more file.txt`

### more
Displays the first few lines of a file (using `more` with a limit).
Example: `more +1 file.txt` (manually stop after a few lines)

### more
Displays the last few lines of a file (using `more` and navigating to the end).
Example: `more file.txt` (manually navigate)

### findstr
Searches for a pattern in a file.
Example: `findstr "pattern" file.txt`

### dir /s
Finds files or directories that match specific criteria.
Example: `dir /s *.txt`

### tasklist
Displays information about running processes.
Example: `tasklist`

### taskkill
Sends a signal to terminate a process.
Example: `taskkill /PID PID`

### icacls
Changes the permissions of a file or directory.
Example: `icacls file.txt /grant User:F`

### takeown
Changes the owner of a file or directory.
Example: `takeown /F file.txt`

### tar
Archives files into a tarball (if available via Windows Subsystem for Linux or third-party tools).
Example: `tar -czvf archive.tar.gz file1.txt file2.txt`

### unzip
Extracts files from a zip archive.
Example: `tar -xf archive.zip` (with third-party tools) or `Expand-Archive` (PowerShell)

### taskmgr
Displays information about system processes and resource usage.
Example: `taskmgr`

### systeminfo
Displays information about system memory usage.
Example: `systeminfo | findstr "Total Physical Memory"`

### wmic logicaldisk get size,freespace,caption
Displays information about disk space usage.
Example: `wmic logicaldisk get size,freespace,caption`

### dir /s
Displays information about disk usage for specific directories.
Example: `dir /s C:\Users\User\Documents`

### ping
Checks connectivity to a network host.
Example: `ping google.com`

### mstsc
Securely connects to a remote server.
Example: `mstsc /v:server`

### pscp
Copies files securely between hosts (using PuTTY tools).
Example: `pscp file.txt user@server:/path/to/destination`

### curl
Retrieves data from a URL.
Example: `curl https://www.example.com`

### wget
Downloads files from the internet (requires wget to be installed).
Example: `wget https://www.example.com/file.txt`

### choco
Manages software packages (requires Chocolatey).
Example: `choco upgrade all`

### services.msc
Manages system services.
Example: `services.msc`

### wevtutil
Displays system logs.
Example: `wevtutil qe System /c:10 /f:text /rd:true`

### ipconfig
Displays information about network interfaces.
Example: `ipconfig`

### netsh
Displays and configures IP addresses, routes, and tunnels.
Example: `netsh interface ip show config`

### route
Displays and configures network routing.
Example: `route print`

### netstat
Displays information about network connections and socket usage.
Example: `netstat -an`

### netsh advfirewall
Manages firewall rules.
Example: `netsh advfirewall firewall add rule name="Allow SSH" protocol=TCP dir=in localport=22 action=allow`

### hostname
Displays or sets the hostname of the system.
Example: `hostname`

### systeminfo
Displays information about the Windows OS.
Example: `systeminfo`

### date /t
Displays the current date.
Example: `date /t`

### time /t
Displays the current time.
Example: `time /t`

### whoami
Displays the name of the current user.
Example: `whoami`

### runas
Executes a command as another user.
Example: `runas /user:Administrator cmd`

### net user
Adds a new user account.
Example: `net user new_user password /add`

### net user
Changes the password for a user account.
Example: `net user user *`

### net user
Modifies user account properties.
Example: `net user username /active:no`



===============================================================================================================
Equivalent Linux commands:
------------------------------->


### ls

Lists files and directories in the current directory.
Example: `ls`

### cd
Changes the current working directory.
Example: `cd /home/user/Documents`

### pwd
Prints the current working directory.
Example: `pwd`

### mkdir
Creates a new directory.
Example: `mkdir new_directory`

### rmdir
Removes an empty directory.
Example: `rmdir empty_directory`

### rm
Removes files or directories.
Example: `rm file.txt` or `rm -r directory`

### touch
Creates a new empty file.
Example: `touch new_file.txt`

### cp
Copies files or directories.
Example: `cp file.txt new_file.txt` or `cp -r directory new_directory`

### mv
Moves or renames files or directories.
Example: `mv file.txt new_file.txt` or `mv directory new_directory`

### cat
Displays the contents of a file.
Example: `cat file.txt`

### less
Allows you to view the contents of a file one page at a time.
Example: `less file.txt`

### head
Displays the first few lines of a file.
Example: `head file.txt`

### tail
Displays the last few lines of a file.
Example: `tail file.txt`

### grep
Searches for a pattern in a file.
Example: `grep "pattern" file.txt`

### find
Finds files or directories that match specific criteria.
Example: `find /home/user -name "*.txt"`

### ps
Displays information about running processes.
Example: `ps aux`

### kill
Sends a signal to terminate a process.
Example: `kill PID`

### chmod
Changes the permissions of a file or directory.
Example: `chmod 755 file.txt`

### chown
Changes the owner of a file or directory.
Example: `chown user:group file.txt`

### tar
Archives files into a tarball.
Example: `tar -czvf archive.tar.gz file1.txt file2.txt`

### unzip
Extracts files from a zip archive.
Example: `unzip archive.zip`

### top
Displays information about system processes and resource usage.
Example: `top`

### free
Displays information about memory usage.
Example: `free -m`

### df
Displays information about disk space usage.
Example: `df -h`

### du
Displays information about disk usage for specific directories.
Example: `du -sh /home/user/Documents`

### ping
Checks connectivity to a network host.
Example: `ping google.com`

### ssh
Securely connects to a remote server.
Example: `ssh user@server`

### scp
Copies files securely between hosts.
Example: `scp file.txt user@server:/path/to/destination`

### curl
Retrieves data from a URL.
Example: `curl https://www.example.com`

### wget
Downloads files from the internet.
Example: `wget https://www.example.com/file.txt`

### apt
Manages software packages on Debian-based systems.
Example: `apt update && apt upgrade`

### yum
Manages software packages on Red Hat-based systems.
Example: `yum update`

### systemctl
Manages system services on systemd-based systems.
Example: `systemctl start service`

### journalctl
Displays system logs.
Example: `journalctl -xe`

### ifconfig
Displays information about network interfaces.
Example: `ifconfig`

### ip
Displays and configures IP addresses, routes, and tunnels.
Example: `ip addr show`

### route
Displays and configures network routing.
Example: `route -n`

### netstat
Displays information about network connections and socket usage.
Example: `netstat -an`

### iptables
Manages firewall rules.
Example: `iptables -A INPUT -p tcp --dport 22 -j ACCEPT`

### hostname
Displays or sets the hostname of the system.
Example: `hostname`

### uname
Displays information about the Linux kernel.
Example: `uname -a`

### date
Displays the current date and time.
Example: `date`

### whoami
Displays the name of the current user.
Example: `whoami`

### su
Switches to another user account.
Example: `su - user`

### sudo
Executes a command as another user with elevated privileges.
Example: `sudo command`

### adduser
Adds a new user account.
Example: `adduser new_user`

### passwd
Changes the password for a user account.
Example: `passwd user`

### usermod
Modifies user account properties

