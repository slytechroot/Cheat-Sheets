🔑 Resetting Windows 10 Password Using Kali Linux/Ubuntu  
*Note: This guide is for educational purposes only. Proceed with caution. Do not attempt on your primary system, as it may cause data loss. Always use a legitimate license and practice on a virtual machine.*


### Steps to Reset Windows 10 Password Using Ubuntu

1. Insert a Live USB and Boot into the System  
   Insert a live USB (Kali Linux or Ubuntu) and boot your system to access the root shell.

2. Identify the Windows Partition  
   Use the following command to list all available partitions:
  
   $ lsblk
   
   Locate the Windows partition (typically /dev/sda1).

3. Mount the Windows Partition  
   Create a mount point and mount the Windows partition:
  
   $ sudo mkdir /mnt/windows
   $ sudo mount /dev/sda1 /mnt/windows
   

4. Backup and Replace Utility Files  
   Navigate to the System32 directory where the utility files are located:
  
   $ cd /mnt/windows/Windows/System32
   

   - Backup the utilman.exe file:
    
     sudo cp utilman.exe utilman.exe.bak
     

   - Replace sethc.exe with cmd.exe:
    
     sudo cp cmd.exe sethc.exe
     

5. Unmount the Windows Partition  
   After making the changes, unmount the partition:
  
   sudo umount /mnt/windows
   

6. Reboot the System  
   Reboot the system into Windows:
  
   sudo reboot
   

7. Reset the Windows Password  
   Once the system has rebooted and you reach the login screen, press the Shift key five times to open a command prompt window. In the command prompt, run the following command to reset the password for the user account. (Replace demo with the username and 123456 with the new password):
  
   $ net user demo 123456
   

This method allows you to reset the Windows 10 password using Ubuntu or Kali Linux. Always ensure that you’re following ethical practices and have permission to make changes to the system you’re working on. 

Feel free to reach out if you have any questions or need further assistance! 😊

