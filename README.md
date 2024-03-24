# repair windows 11 install

```powershell
DISM.exe /Online /Cleanup-image /Restorehealth
```

The DISM.exe command with the /Online /Cleanup-image /Restorehealth parameters is used to repair and restore the health of the Windows system image. Let’s break down what each part of this command does:

DISM.exe: This stands for Deployment Image Servicing and Management. It’s a built-in Windows utility that allows administrators to prepare, modify, and repair system images.
/Online: Specifies that the operation should be performed on the currently running operating system (online mode) rather than an offline image.
/Cleanup-image: Initiates cleanup operations on the system image. It can remove unnecessary files, components, and packages to reduce the image size.
/Restorehealth: This parameter instructs DISM to restore the health of the system image. It scans for corruption and attempts to repair any issues it finds. If the local image has missing or corrupted files, DISM will attempt to replace them using a known good source (such as the Windows installation media or a recovery image).
Here’s how you can use it:

Open the Command Prompt as an administrator:
Press Windows + X, then select Command Prompt (Admin).
Alternatively, search for Command Prompt, right-click the top result, and choose Run as administrator.
Type the following command and press Enter:
DISM /Online /Cleanup-Image /RestoreHealth
This will start the repair process. DISM will check for corruption and attempt to fix any issues it encounters.
Remember to create a temporary backup before proceeding, just in case. The commands are non-destructive, but it’s always good to have a safety net! 😊
