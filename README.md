```
Name: Swetha S V
Reg no: 212224230285
```
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

![388344173-b2c97dd3-0863-4481-8a62-027ad75b56f0](https://github.com/user-attachments/assets/a41312f2-bc3c-4c95-a0f4-dd28c457d4af)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

    cd %userprofile%\Desktop\MyLab

![388344225-4749e48a-d6c2-465c-b66c-467b535e741c](https://github.com/user-attachments/assets/e6b7cc9a-89c4-4217-8ee0-b2f11cf6e814)

    type nul > MyFile.txt

![388344239-264f09a9-9ab1-4319-8ffb-087580360d88](https://github.com/user-attachments/assets/69825db3-1a14-4fa4-b07b-03d4aff5156b)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT

    dir %userprofile%\Desktop\MyLab

  ![388344276-8a095fc7-fb1e-4b82-9dff-46ed48ac79c9](https://github.com/user-attachments/assets/c7e72f1c-739e-4e48-ba6a-6b24131ee076)

    
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

    mkdir %userprofile%\Desktop\Backup
![388344302-40881217-36a6-4c3b-9a98-084c1d4f06b7](https://github.com/user-attachments/assets/dd56dc73-fae5-4ad2-9ade-37115ea599e5)

    copy MyFile.txt %userprofile%\Desktop\Backup

![388344337-15c04a42-8b5e-4005-a4d6-eefff8a529c2](https://github.com/user-attachments/assets/e668d5a5-4fa1-432c-b6c8-08a8a205fa37)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
    mkdir %userprofile%\Desktop\Documents

![388344361-6db49bc8-0724-45f1-a9f3-ff9ef8d5ffbf](https://github.com/user-attachments/assets/018ef1c2-9638-4c8f-9cf8-51a62c8ee0ee)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.


## COMMAND

    @echo off
    mkdir %userprofile%\Desktop\DocBackup
    copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
    echo Backup completed successfully!

## OUTPUT


![388344382-af5e3830-2b8c-465d-9ccb-b6c15b159502](https://github.com/user-attachments/assets/ea26344c-ba13-4048-87b2-23f66b91e9fc)

## COMMAND

    @echo off
    mkdir %userprofile%\Desktop\DocBackup
    copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
    del %userprofile%\Documents\*.docx
    echo Backup and deletion completed successfully!

## OUTPUT

![388344518-db602c4e-116e-4c0c-84d3-9e750b2d6ebe](https://github.com/user-attachments/assets/a5ff0234-bea9-4697-b4bd-862557474ba0)

# RESULT:
The commands/batch files are executed successfully.

