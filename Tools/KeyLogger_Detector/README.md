Keylogger Detection Tool – README & User Guide

This security tool addresses the growing threat of unauthorized keystroke monitoring by:

• Detecting known keylogger processes in memory
• Identifying suspicious process names and behaviors
• Providing visibility into running system processes
• Offering basic process management capabilities

The tool helps users identify potential security risks while maintaining strict ethical guidelines for defensive cybersecurity use only.

FEATURES

1. Detects known keylogger process names using pattern matching.
2. Lists all currently running programs and processes.
3. Shows live system health stats like CPU and RAM usage.
4. Clean, responsive graphical interface built with Tkinter.
5. Gives user the option to terminate detected keylogger processes.
6. Includes animated scanning window and progress bar for better UX.


SETUP INSTRUCTIONS

Requirements:
- Windows 7/10/11
- Python 3.6 or later
- Administrator privileges (for full functionality)

Installation Steps:
1. Install Python from python.org
2. Open Command Prompt as administrator
3. Install required package:
   pip install psutil
4. Download the keylogger_detector.py file
5. Run the application:
   python keylogger_detector.py

Note: This tool should only be used on systems you own or have permission to scan.

HOW IT WORKS
- The app checks the list of currently running programs using psutil.
- It compares each process name against a dictionary of known keylogger-related keywords such as:
    "keylogger", "logger", "spy", "ahk.exe", "hook", etc.
- If any of these are found in the name of a running process, the tool assumes it might be suspicious.
- It shows a result window listing the possible threats.
- You can then choose to end those processes from within the app.
 


SCREENSHOTS

•	Main Interface

Clean home screen with scanning options



![ss1](https://github.com/user-attachments/assets/3caf4854-1e85-4b52-aac1-e4c87add5210)


•	Detection Progress

Real-time progress bar during detection



![ss2](https://github.com/user-attachments/assets/432d7701-9b53-44a9-9742-796e2ea7c8fa)



•	Results Window

Detailed view of detected keyloggers with termination option

![ss3](https://github.com/user-attachments/assets/7d81f98d-6023-476f-849d-2353b781b0bb)
![ss4](https://github.com/user-attachments/assets/a1729949-1996-4377-8b37-d3d1059bf77d)

	              
•	Process Viewer

Complete list of running processes

![ss5](https://github.com/user-attachments/assets/b59fdda9-1a7b-4191-b625-50fa21ec441a)


•	System Health Info

![ss6](https://github.com/user-attachments/assets/83b2d513-1bd8-410f-bd49-1f4300c51df5)


LIMITATIONS
- This tool only scans based on names, not behavior or file content.
- It may give false positives if safe programs have names similar to keyloggers.
- It cannot detect advanced or hidden keyloggers that mask their process name.
- It is not a substitute for antivirus or professional threat detection tools.

