# Add Store to Windows 10\11 
## To install, run Windows-Store-AIO.cmd
If the store still will not function, reboot. If still not working, open the command prompt as the administrator and run the following command, then reboot once more.  
```PowerShell -ExecutionPolicy Unrestricted -Command "& {$manifest = (Get-AppxPackage Microsoft.WindowsStore).InstallLocation + '\AppxManifest.xml' ; Add-AppxPackage -DisableDevelopmentMode -Register $manifest}"```    
## Addition troubleshooting    
>Right click start  
Select Run  
Type in: WSReset.exe  
This will clear the cache if needed.  
  
