# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting
name: dharshini K

regno:23010696
# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/78f911d4-9eb9-42db-a762-376764c039b9)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/6733ae66-dde6-453b-8147-417133c3ca64)
![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/25a1f238-4439-419c-afd3-4146816954f3)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/615ba95b-4650-4c26-ad0e-83f0aac86a1b)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/1c6aa0bf-68ef-4376-b21f-8168f4449b04)

![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/11a60b0b-9973-4232-9ae8-b637d01a3104)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents


![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/e915e6d8-1546-46cd-b42e-514286544cff)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![image](https://github.com/dharshini-29/Windows-basic-commands-batchscript/assets/147474632/de61c1bb-12eb-45e6-8a7e-8e2277deee12)

# RESULT:
The commands/batch files are executed successfully.

