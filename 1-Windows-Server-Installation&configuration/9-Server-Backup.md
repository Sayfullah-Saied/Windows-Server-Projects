<h1>Server Backup</h1>
NOTE:
Server backup is one of the most important aspects of system administration because it helps ensure business continuity and prevents service disruption in the event of data loss or system failure. There are many backup solutions and backup strategies available, each designed to meet different organizational requirements. In this project, we will back up a hard drive to demonstrate the basic concept and process of server backup.
<br><hr>
1. We have an E: drive that contains three folders. This is the drive that will be backed up.<br>
<img width="504" height="542" alt="1" src="https://github.com/user-attachments/assets/90e59e70-0f74-4758-8d47-117efbcb5f4f" />
<br><br>
- Open the Add Roles and Features Wizard, navigate to the Features page, and install the Windows Server Backup feature.<br>
<img width="379" height="427" alt="2" src="https://github.com/user-attachments/assets/e3d20f84-a916-464f-af5c-d95ad068e09d" />

<br><br>
- from tools choose windows server backup and select backup once<br>
<img width="823" height="637" alt="3" src="https://github.com/user-attachments/assets/276ba65a-2ea8-4357-951c-976b403059a0" />

<br><br>
- in out case we will choose custom to backup a hard drive only<br>
<img width="466" height="472" alt="4" src="https://github.com/user-attachments/assets/4b9aef92-df5f-48ff-8925-c2d2e4ef53d2" />
<br><br>
- choose the E drive<br>
<img width="359" height="356" alt="5" src="https://github.com/user-attachments/assets/c9ede994-276b-4565-a4f1-b753f9be4f2d" />
<br><br><hr>
2. let's delete the contents of the E drive now <br>
<img width="748" height="566" alt="6" src="https://github.com/user-attachments/assets/7aa1f4ba-725f-4a4e-99c0-b9b058acbb4d" />
<br><br>
- again from windows server backup choose recover and select the backup date and time and recover the hard drive<br>
<img width="659" height="459" alt="7" src="https://github.com/user-attachments/assets/8f5c1cb9-9f0d-4ea8-bc34-11a3ead414e1" />
<br><br>
- Data successfully recovered <br>
<img width="658" height="488" alt="8" src="https://github.com/user-attachments/assets/86abd6d1-1470-4e5a-b817-4b16bae8dea7" />
