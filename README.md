
# r6829 Version 2 Rootkit
## this is a fork of the r77 and MasterHide rootkits, converted into and all in one ring3-rootkit DLL

  Current working hooks
    NtUserQueryWindow
    NtUserGetForegroundWindow
    NtOpenProcess
    NtQuerySystemInformation
    NtQueryDirectoryFile
    and some more techniques included in source but stay unlisted for security purposes.
    ![image](https://github.com/user-attachments/assets/f6ec3277-4188-4ebf-9d55-eb037c62b0b1)
![Screenshot 2024-07-13 095825_2](https://github.com/user-attachments/assets/2685bbc1-baa3-4580-8e0f-848d43b1c2f8)

    
  also has anti regedit, event viewer, and anti winpcap/npcap dlls, if any dll called "packet.dll" or "wpcap.dll" is loaded into any process under hook, it will call exit(0); to kill it.

  contains mild amount of antiskid.
