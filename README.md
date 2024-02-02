# Linux-most-useful-commands
All the Most useful Linux commands and Tools for a DevOps Engineer are needed.

##                                                                                 VI (VIM) EDITOR COMMANDS:

### NAVIGATION

`h` : Move cursor left
`j` : Move cursor dow
`k` : Move cursor up
`l` : Move cursor right

### EDITING

`i` : Insert mode (start inserting before the cursor)
`a` : Append mode (start inserting after the cursor)
`x` : Delete character at the cursor
`dd` : Delete the current line
`yy` : Yank (copy) the current line
`p` : Paste the yanked or deleted text

### SAVE AND QUIT

`h`	: Move cursor left
`j`	: Move cursor dow
`k`	: Move cursor up
`l`	: Move cursor right

SAVE AND QUIT

`h` : Move cursor left
`j` : Move cursor dow
`k` : Move cursor up
`l` : Move cursor right

### SEARCH AND REPLACE

/pattern` : Search for 'pattern'
`:s/old/new/g` : Replace 'old' with 'new' in the entire file

### UNDO AND REDO

`u`: Undo
`Ctrl + r` : Redo

### COPY AND PASTE (VISUAL MODE)

`v` : Enter Visual mode
`V` : Enter Visual Line mode
`y` : Yank selected text

### MOVING BETWEEN WORDS

`0` : Move to the beginning of the line
`$` : Move to the end of the line
`:n` : Move to line number 'n'

### NAVIGATING BY LINE

`0` : Move to the beginning of the line
`$` : Move to the end of the line
`:n` : Move to line number 'n'

### OPEN AND SAVE FILES

`:e filename` : Open a file
`:w filename` : Save as a different filename

### EXIT WITHOUT SAVING CHANGES

`:q!` : Quit without saving changes


##                                                                    NANO EDITOR SHORTCUTS

### NAVIGATION

`Alt + A` : Mark text for copying
`Ctrl + K` : Cut marked text
`Ctrl + U` : Paste cut text

### EDITING

`Ctrl + k` : Cut (delete) the current line
`Ctrl + u` : Paste the cut text
`Ctrl + o` : Write changes to the file
`Ctrl + x` : Exit nano

### SEARCH AND REPLACE

`Ctrl + w` : Search for text
`Ctrl + \` : Replace text

### COPY AND PASTE

`Ctrl + f` : Move forward one page
`Ctrl + b` : Move backward one page
`Ctrl + arrow keys` : Move cursor by word

### EDITING

`Ctrl + k` : Cut (delete) the current line
`Ctrl + u` : Paste the cut text
`Ctrl + o` : Write changes to the file
`Ctrl + x` : Exit nano

### LINE NUMBERS

Alt + ,` : Go to line number

HELP

`Ctrl + X` : Close nano (it will ask to save changes)

##                                                                                   LINUX COMMAND FOR DEVOPS

1. ls - List Files and Directories: List the contents of a directory.
```bash
ls -l
```
3. cd - Change Directory: Navigate to a different directory.
```bash cd /home/user/documents ```

5. pwd - Print Working Directory: Display the current directory's full path.
Example: pwd

6. mkdir - Make Directory: Create a new directory.
Example: mkdir new_folder

7. rm - Remove: Delete files or directories.
Example: rm file.txt

9. cat - Concatenate and Display: View the content of a file.
Example: cat file.txt

10. nano - Text Editor: Open a text file for editing.
Example: nano file.txt

11. grep - Search Text: Search for text patterns in files.
Example: grep "pattern" file.txt

12. find - Search Files and Directories: Search for files and directories.
Example: find /path/to/search -name "file_name"

13. chmod - Change File Permissions: Modify file permissions.
Example: chmod 755 file.sh

14. chown - Change Ownership: Change the owner and group of a file or directory.
Example: chown user:group file.txt

15. ps - Process Status: Display running processes.
Example: ps aux

16. top - Monitor System Activity: Monitor system processes in real-time.
Example: top

17. kill - Terminate Processes: Terminate a process using its ID.
Example: kill PID

18. wget - Download Files: Download files from the internet.
Example: wget https://example.com/file.zip

19. curl - Transfer Data with URLs: Transfer data to or from a server.
Example: curl -O https://example.com/file.txt

20. tar - Archive and Extract: Create or extract compressed archive files.
Example: tar -czvf archive.tar.gz folder

21. ssh - Secure Shell: Connect to a remote server securely.
Example: ssh user@remote_host

22. scp - Securely Copy Files: Copy files between local and remote systems using SSH.
Example: scp file.txt user@remote_host:/path

23. rsync - Remote Sync: Synchronize files and directories between systems.
Example: rsync -avz local_folder/ user@remote_host:remote_folder/

24. df - Disk Free Space: Display disk space usage.
Example: df -h

25. du - Disk Usage: Show the size of files and directories.
Example: du -sh /path/to/directory

26. ifconfig - Network Configuration: Display or configure network interfaces (deprecated, use ip).
Example: ifconfig

27. ip - IP Configuration: Manage IP addresses and network settings.
Example: ip addr show

28. netstat - Network Statistics: Display network connections and statistics (deprecated, use ss).
Example: netstat -tuln

29. systemctl - System Control: Manage system services using systemd.
Example: systemctl start service_name

30. journalctl - Systemd Journal: View system logs using systemd's journal.
Example: journalctl -u service_name

31. cron - Schedule Tasks: Manage scheduled tasks.
Example: crontab -e

32. at - Execute Commands Later: Run commands at a specified time.
Example: echo "command" | at 15:30

33. ping - Network Connectivity: Check network connectivity to a host.
Example: ping google.com

34. traceroute - Trace Route: Trace the route packets take to reach a host.
Example: traceroute google.com

35. curl - Check Website Connectivity: Check if a website is up.
Example: curl -Is https://example.com | head -n 1

36. dig - Domain Information Groper: Retrieve DNS information for a domain.
Example: dig example.com

37. hostname - Display or Set Hostname: Display or change the system's hostname.
Example: hostname

38. who - Display Users: Display currently logged-in users.
Example: who

39. useradd - Add User: Create a new user account.
Example: useradd newuser

40. usermod - Modify User: Modify user account properties.
Example: usermod -aG groupname username

41. passwd - Change Password: Change user password.
Example: passwd username

43. lsof - List Open Files: List open files and processes using them.
Example: ```bash lsof -i :port ```

44. nc - Netcat: Networking utility to read and write data across network connections.
Example: ```bash echo "Hello" | nc host port ```

45. scp - Secure Copy Between Hosts: Copy files securely between hosts.
Example: ```bash scp file.txt user@remote_host:/path ```

46. sed - Stream Editor: Text manipulation using regex.
Example: ```bash sed 's/old/new/g' file.txt ```

47. awk - Text Processing: Pattern scanning and text processing.
Example: ```bash awk '{print $2}' file.txt ```

48. cut - Text Column Extraction: Extract specific columns from text.
Example: ```bash cut -d"," -f2 file.csv ```

## LINUX NETWORKING COMMAND

### nslookup:

Purpose: Query DNS to obtain domain-related information.
Example: ```bash `nslookup example.com` ```
Explanation: Useful for troubleshooting DNS issues, checking domain
information, and resolving IP addresses.

### dig (Domain Information Groper):

Purpose: A versatile DNS tool for querying DNS servers.
Example: ```bash `dig example.com` ```
Explanation: Provides detailed DNS information, useful for debugging and
obtaining specific record types

##                                                                           CONNECTIVITY TESTING COMMAND

### telnet:

Purpose: Connect to a remote server to test network connectivity.
Example: ```bash `telnet example.com 80` ```
Explanation: Useful for checking if a specific port on a remote server is reachable.

##                                                                           CONNECTIVITY TESTING COMMAND

### ncc:

Purpose: Trace the route packets take to reach a destination.
Example: ```bash `traceroute example.com` ```
Explanation: Helps identify network issues and understand the path packets
take through the internet.

##                                                                             IP ADDRESS CONFIGURATION

### ifconfig:

Purpose: Display and configure network interfaces.
Example: ```bash `ifconfig` ```
Explanation: View current network interface configurations and assign IP addresses.

### ip:

Purpose: A versatile command for network configuration.
Example: ```bash `ip addr show` ```
Explanation: Provides more detailed information than ifconfig and allows advanced network configuration.

##                                                                                NETWORK TOOLS

### netcat (nc):

Purpose: Establish TCP/UDP connections, making it a versatile networking tool.
Example: ```bash `nc -zv example.com 80` ```
Explanation: Useful for checking if a port is open and for simple network testing.

### netstat:

Purpose: Display network statistics and connections.
Example: ```bash `netstat -tulpn` ```
Explanation: Helps monitor active network connections, ports, and routing tables.

### tcpdump:

Purpose: Capture and analyze network traffic.
Example: ```bash `tcpdump -i eth0` ```
Explanation: Useful for debugging network issues, analyzing packets, and monitoring network activity.

### wget:

Purpose: Download files from the internet.
Example: ```bash `wget https://example.com/file.txt` ```
Explanation: Simplifies downloading files, is useful for fetching resources from the web.

curl:

Purpose: Transfer data from or to a server.
Example: ```bash `curl https://example.com/api` ```
Explanation: Supports a variety of protocols and is handy for testing APIs and fetching web content.

##                                                               ACL , ARP, AND ROUTE TABLE COMMANDS:

### ACL (Access Control List):

Purpose: Set permissions on files or directories.
Example: ```bash `setfacl -m u:jane:rw file.txt` ```
Explanation: Allows fine-grained control over file and directory permissions.

ACL (Access Control List):

Purpose: Set permissions on files or directories.
Example: ```bash `setfacl -m u:jane:rw file.txt` ```
Explanation: Allows fine-grained control over file and directory permissions.

### ARP Table:

Purpose: Display or manipulate the ARP cache.
Example: ```bash `arp -a` ```
Explanation: Shows a mapping between IP addresses and MAC addresses on the local network.
.
### Route Table:

Purpose: Display or manipulate the IP routing table.
Example: ```bash `route -n` ```
Explanation: Helps monitor active network connections, ports, and routing tables.

##                                                                                     NAMESPACE

### Create a veth virtual-interface pair
```bash
sudo ip link add 'myns-1-eth0' type veth peer name 'myns-2-eth0'
```
### Assign the interfaces to the namespaces
```bash
sudo ip link set 'myns-1-eth0' netns 'mynamespace-1'
sudo ip link set 'myns-2-eth0' netns 'mynamespace-2'
```
### Assign an address to the network interface
```bash
sudo ip netns exec 'mynamespace-1' ip addr add 192.168.1.1/24 dev eth0
```
### Assign the interfaces to the namespaces

```bash
sudo ip link set 'myns-1-eth0' netns 'mynamespace-1'
sudo ip link set 'myns-2-eth0' netns 'mynamespace-2'
```


### Bring up the interfaces (the veth interfaces and the loopback interfaces)
```bash
sudo ip netns exec 'mynamespace-1' ip link set 'lo' up
sudo ip netns exec 'mynamespace-1' ip link set 'eth0' up
```











