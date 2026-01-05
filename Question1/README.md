Question 1 – Basic Environment Verification  solution

1. User Identity Verification

Command:
whoami
groups

Explanation:
The whoami command displays the currently logged-in username.
The groups command shows all the groups the current user account belongs to.


2. Workspace Validation

Command:
pwd
ls -l

Explanation:
The pwd command shows the current working directory.
The ls -l command lists all files and directories in long format with permissions and ownership details.


3. Environment Confirmation File

Command:
echo "Linux user environment verified" > user_info.txt

Explanation:
This command creates a file named user_info.txt and writes the required verification message into it.


4. File Integrity Check

Command:
wc -c user_info.txt

Explanation:
The wc -c command counts the total number of characters present in the file.


5. Learning the Tools

Command:
man mkdir

Useful Option:
-p

Explanation:
The -p option allows creating parent directories automatically if they do not already exist.


6. Home Directory Inspection

Command:
ls ~ | sort

Explanation:
This command lists all contents of the home directory and sorts them alphabetically.


7. Log Investigation

Command:
grep "admin" log.txt

Explanation:
The grep command searches for the word "admin" in the file log.txt and displays only the matching lines.


8. System Information Check

Command:
uname -r

Explanation:
This command displays the Linux kernel version currently running on the system.


9. Network Connectivity Test

Command:
ping -c 4 www.google.com

Explanation:
The ping command sends ICMP packets to verify network connectivity with an external server.


10. System Health Awareness

Command:
uptime

Explanation:
The uptime command shows how long the system has been running, the number of logged-in users, and the system load average.

