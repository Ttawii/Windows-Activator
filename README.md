# Windows 10 Activation Script

This project provides a script to activate Windows 10 using KMS (Key Management Service) and the `slmgr.vbs` utility. The script sets the product keys for different versions of Windows 10 and attempts activation through several KMS servers.

## Steps:

### 1. **Create the Script File:**
- Open **Notepad** (or any text editor of your choice).
- Copy the script code provided below into Notepad.
- This script will help you activate Windows by attempting to connect to different KMS servers and applying a set of keys.

### 2. **Script Code:**
```batch
@echo off
title Windows 10 ALL version activator&cls&echo ************************************&echo Supported products:&echo - Windows 10 Home&echo - Windows 10 Professional&echo - Windows 10 Enterprise, Enterprise LTSB&echo - Windows 10 Education&echo.&echo.&echo ************************************ &echo Windows 10 activation...
cscript //nologo c:\windows\system32\slmgr.vbs /ipk TX9XD-98N7V-6WMQ6-BX7FG-H8Q99 >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk 3KHY7-WNT83-DGQKR-F7HPR-844BM >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk 7HNRX-D7KGG-3K4RQ-4WPJ4-YTDFH >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk PVMJN-6DFY6-9CCP6-7BKTT-D3WVR >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk W269N-WFGWX-YVC9B-4J6C9-T83GX >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk MH37W-N47XK-V7XM9-C7227-GCQG9 >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk NW6C2-QMPVW-D7KKK-3GKT6-VCFB2 >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk 2WH4N-8QGBV-H22JP-CT43Q-MDWWJ >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk NPPR9-FWDCX-D2C8J-H872K-2YT43 >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4 >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk WNMTR-4C88C-JK8YV-HQ7T2-76DF9 >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ipk 2F77B-TNFGY-69QQF-B8YKP-D69TJ >nul
echo ************************************ &echo.&echo.&set i=1
:server
if %i%==1 set KMS_Sev=kms.shuax.com
if %i%==2 set KMS_Sev=NextLevel.uk.to
if %i%==3 set KMS_Sev=GuangPeng.uk.to
if %i%==4 set KMS_Sev=AlwaysSmile.uk.to
if %i%==5 set KMS_Sev=kms.chinancce.com 
if %i%==6 exit
cscript //nologo c:\windows\system32\slmgr.vbs /skms %KMS_Sev% >nul
cscript //nologo c:\windows\system32\slmgr.vbs /ato | find /i "successfully" && (echo.& echo ************************************ & echo. & choice /n /c YN /m "Do you want to restart your PC now [Y,N]?" & if errorlevel 2 exit) || (echo The connection to the server failed! Trying to connect to another one... & echo Please wait... & echo. & echo. & set /a i+=1 & goto server)
shutdown.exe /r /t 00
```
### 3. **Save the File:**
- After pasting the code, save the file with the `.txt` extension. For example, name the file `activate_windows.txt`.

### 4. **Convert the `.txt` to `.bat`:**
- Change the file extension from `.txt` to `.bat`. For example, rename the file to `activate_windows.bat`.
- To do this, simply right-click the file, select **Rename**, and change the extension to `.bat`.

### 5. **Run as Administrator:**
- Right-click on the `activate_windows.bat` file.
- Select **Run as Administrator** to allow the script to execute with the required permissions.

### 6. **What Does This Script Do?**
- The script starts by setting the product keys for different Windows 10 versions.
- Then, it attempts to activate Windows by connecting to various KMS servers.
- If the first KMS server fails, it will attempt others until successful or it runs out of servers.
- Once a successful activation is detected, it will prompt the user to restart the system to apply the changes.

### 7. **Important Notes:**
- **Warning**: Using this script can violate Microsoft's licensing agreements and is generally not recommended for legal, authorized use. It is meant for educational purposes or testing in specific environments.
- Make sure you are aware of the legal implications before running such scripts.

## Conclusion

This script provides a way to activate Windows 10 using KMS servers and product keys. However, please note that activating Windows in this way may violate Microsoft's licensing agreements. This project is intended solely for educational purposes and testing in controlled environments. Always ensure that you comply with legal and ethical standards when using such tools.

If you have any questions or need further assistance, feel free to reach out or open an issue in this repository.

Thank you for checking out this project!

<a href="https://www.instagram.com/t2tt/" style="color: white; text-decoration: none;">
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/95/Instagram_logo_2022.svg" alt="Instagram" width="30" />
</a>
