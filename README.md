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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```

mkdir %userprofile%\Desktop\MyLab

```
<img width="710" alt="image" src="https://github.com/user-attachments/assets/6a452a3f-4742-42b5-b4fc-f88c3a6eaddc" />



## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

```
cd %userprofile%\Desktop\MyLab

```
<img width="651" alt="image" src="https://github.com/user-attachments/assets/7a808a8a-758a-40f9-9512-74820a735c72" />

```

 type nul > MyFile.txt

```
<img width="700" alt="image" src="https://github.com/user-attachments/assets/54d4a9ad-4c5d-4c4c-a1ac-8e8337004307" />



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
dir %userprofile%\Desktop\MyLab

```
<img width="811" alt="image" src="https://github.com/user-attachments/assets/ffcb283d-b7ae-4e65-a706-19e16f140ec5" />


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup

```
<img width="799" alt="image" src="https://github.com/user-attachments/assets/0db3d4c3-5c97-4e23-9e29-1241ab686037" />



```

copy MyFile.txt %userprofile%\Desktop\Backup

```
<img width="811" alt="image" src="https://github.com/user-attachments/assets/a393b486-d311-4e1e-9fe4-9304aa1b666f" />


## COMMAND AND OUTPUT

move MyLab Documents

```
mkdir %userprofile%\Desktop\Documents

```
<img width="828" alt="image" src="https://github.com/user-attachments/assets/660dcfcf-0a14-4620-b4fc-8c219e0ba50f" />


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

## Command:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

```






## OUTPUT
<img width="828" alt="image" src="https://github.com/user-attachments/assets/75924fea-e48a-4f15-bfac-1808b164c887" />

## command:

```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!

```

## Output:

<img width="828" alt="image" src="https://github.com/user-attachments/assets/27102831-801a-4ddc-aef8-578b2f78b608" />





# RESULT:
The commands/batch files are executed successfully.

