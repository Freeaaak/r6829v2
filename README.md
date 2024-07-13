
# r6829 Rootkit
## this is a fork of the r77 and MasterHide rootkits, converted into and all in one ring3-rootkit DLL

  Current working hooks
    NtUserQueryWindow
    NtUserGetForegroundWindow
    NtOpenProcess
    NtQuerySystemInformation
    NtQueryDirectoryFile
    ![image](https://github.com/user-attachments/assets/f6ec3277-4188-4ebf-9d55-eb037c62b0b1)

    
  also has anti regedit, event viewer, and anti winpcap/npcap dlls, if any dll called "packet.dll" or "wpcap.dll" is loaded into any process under hook, it will call exit(0); to kill it.

  contains mild amount of antiskid.
