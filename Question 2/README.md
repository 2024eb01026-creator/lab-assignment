Question 2 – File and Directory Management solution

Project Workspace Setup

Command:
mkdir ~/documents

Explanation:
This command creates a directory named documents inside the home directory to store project-related files.

File Creation

Command:
cd ~/documents
touch plan.txt

Explanation:
The cd command navigates into the documents directory and the touch command creates an empty file named plan.txt.

Content Addition

Command:
echo "This is a sample project plan note." > plan.txt

Explanation:
This command writes a sample text into the plan.txt file, replacing any existing content.

File Metadata Verification

Command:
ls -l plan.txt

Explanation:
The ls -l command displays file permissions, ownership, and other metadata, confirming that the file belongs to the current user.

File Duplication

Command:
cp plan.txt plan_copy.txt

Explanation:
This command creates a duplicate of plan.txt named plan_copy.txt in the same directory.

Directory Renaming

Command:
cd ~
mv documents project_documents

Explanation:
The mv command renames the documents directory to project_documents to better reflect the project scope.

Archival Structure

Command:
mkdir ~/project_documents/archive

Explanation:
This command creates a subdirectory named archive inside the project_documents directory.

File Organization

Command:
mv ~/project_documents/plan_copy.txt ~/project_documents/archive/

Explanation:
This command moves the copied file plan_copy.txt into the archive subdirectory.

Recursive Listing

Command:
ls -R ~/project_documents

Explanation:
The ls -R command lists all files and subdirectories inside project_documents recursively, showing the complete directory structure.

Path Verification

Command:
realpath ~/project_documents/archive/plan_copy.txt

Explanation:
The realpath command displays the absolute path of the plan_copy.txt file after it has been moved to the archive directory.
