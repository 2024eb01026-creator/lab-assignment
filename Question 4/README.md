Question 4 – System Monitoring and Process Management  solution

System Uptime Verification

Command:
uptime

Explanation:
The uptime command displays how long the system has been running since the last boot.

User Process Listing

Command:
ps -u $USER

Explanation:
This command lists all processes that are currently running under the logged-in user account.

CPU Usage Analysis

Command:
top -u $USER

Explanation:
The top command shows real-time process information, and the process using the highest CPU can be identified from the %CPU column.

Background Process Execution

Command:
sleep 300 &

Explanation:
This command starts a sleep process in the background, and the ampersand (&) confirms it is running as a background job.

Process Priority Management

Command:
renice 5 -p <PID>

Explanation:
The renice command changes the priority (niceness) of a running process, and the updated priority is displayed after execution.

Memory Usage Monitoring

Command:
free -h

Explanation:
The free -h command displays system memory usage in a human-readable format including total, used, and available memory.

Disk Space Inspection

Command:
df -h ~

Explanation:
This command shows disk space usage of the filesystem where the home directory is located.

Shell Identification

Command:
echo $SHELL

Explanation:
This command displays the name and path of the shell currently being used by the user.

Output Redirection

Command:
uname -a > system_report.txt

Explanation:
This command redirects the output of system information into a file named system_report.txt.

Disk Usage Visualization

Command:
ncdu ~

Explanation:
The ncdu command provides an interactive, visual representation of disk usage within the home directory, helping identify large files and directories.
