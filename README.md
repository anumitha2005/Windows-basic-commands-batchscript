# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

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

![Screenshot 2024-04-27 034100](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/e30f6b69-f77f-42d7-a54b-04bca04e95c0)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![Screenshot 2024-04-27 034246](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/f79cbd7b-f83a-4c4d-9339-6bae89645550)
![Screenshot 2024-04-27 034259](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/936550fb-2570-42f2-8064-417044e31ba1)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![Screenshot 2024-04-27 034313](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/cfeb1af8-2c29-4216-bd8f-1d51a001d4c4)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![Screenshot 2024-04-27 034507](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/d6fcf539-94ea-49b6-8525-460073a6a526)
![Screenshot 2024-04-27 034519](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/378f017c-d46b-46ba-94aa-d0c856777bb1)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![Screenshot 2024-04-27 034621](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/2679b968-1ed6-4016-8511-51b32671595c)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
``
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
``
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
``
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!

```
``




## OUTPUT

![Screenshot 2024-04-27 034749](https://github.com/anumitha2005/Windows-basic-commands-batchscript/assets/155522855/b45ef9f5-90ea-4fb2-91ad-88e42bc4f17b)




# RESULT:
The commands/batch files are executed successfully.

