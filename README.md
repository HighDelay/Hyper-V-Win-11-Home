# Hyper-V-Win-11-Home
This script allows you to install Hyper-V on either Win 10 or Win 11 Home Edition

To remove Hyper-V you can uncheck the Hyper-V check box in "Windows Features" or use the following powershell command:
```
Disable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V-Hypervisor
```

In case Hyper-V is still running even after you have disabled it via "Windows Features" or the powershell command above, paste the following command in windows terminal or cmd, whichever works for you.
Completely disable Hyper-V and stop them from running again:
```
bcdedit /set hypervisorlaunchtype off
```
Then restart the PC to apply the change

To enable it again run the following command:
```
bcdedit /set hypervisorlaunchtype auto
```
Restart yout PC to apply the change.
