Question 3 – Links and Disk Usage Management  solution

File Creation

Command:
echo "This is some sample data for link testing." > ~/sample_data.txt

Explanation:
This command creates a file named sample_data.txt in the home directory and writes sample text into it.

Hard Link Creation

Command:
ln ~/sample_data.txt ~/sample_hard.txt

Explanation:
This command creates a hard link named sample_hard.txt pointing to the same inode as sample_data.txt.

Symbolic Link Creation

Command:
ln -s ~/sample_data.txt ~/sample_soft.txt

Explanation:
This command creates a symbolic (soft) link named sample_soft.txt that points to the original file sample_data.txt.

Inode Verification

Command:
ls -i ~/sample_data.txt ~/sample_hard.txt ~/sample_soft.txt

Explanation:
The ls -i command displays inode numbers of the files, allowing comparison between original, hard link, and symbolic link.

Inode Analysis

Explanation:
sample_data.txt and sample_hard.txt share the same inode number because a hard link points to the same file data on disk.
sample_soft.txt has a different inode because it only stores the path reference to the original file.

File Metadata Inspection

Command:
ls -l ~/sample_data.txt

Explanation:
This command displays detailed file metadata such as permissions, ownership, file size, and timestamps for sample_data.txt.

Disk Usage Check

Command:
du -h ~

Explanation:
The du -h command displays disk usage of the home directory in a human-readable format.

File Size Overview

Command:
ls -lh ~

Explanation:
The ls -lh command shows the sizes of all files in the home directory in a human-readable format.

Link Deletion Test

Command:
rm ~/sample_soft.txt
ls ~/sample_data.txt

Explanation:
The rm command deletes the symbolic link sample_soft.txt.
Listing sample_data.txt confirms that the original file remains unaffected.

Disk Utility Demonstration

Command:
du -sh ~
df -h

Explanation:
The du -sh command shows the total disk space used by the home directory.
The df -h command displays overall filesystem disk usage, including total space, used space, and available space.
