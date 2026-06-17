<h1>Group Policy</h1>
Group Policy is a vast topic, offering numerous options to control and manage user and computer settings.
In this guide, we'll configure several Group Policy Objects (GPOs) to apply these controls within a Windows domain environment.<br><br><hr>

<h3>Open group policy console</h3>
<img width="838" height="674" alt="1" src="https://github.com/user-attachments/assets/1e79dceb-dfa5-4d3c-bf80-89c29e94483a" /><br>
We will setup 2 user policy and 2 computer policy and we will change the background for users in the domain.<br>
The policies we will configure:<br>
<img width="689" height="127" alt="2" src="https://github.com/user-attachments/assets/19fc740b-36e4-4f4c-9a20-1e5e0edea7c5" /><br>
1-Prevent Access to Control Panel<br>
2-Remove Run Command from Start Menu<br>
3-Disable USB Storage Devices<br>
4-Map Network Drive<br><hr>

<h3>Configure and link policies to the domain</h3><hr>
<h1>Background Policy</h1>
Let's first set the background for company users to be the same by the following steps:<br>
1- share the folder that contains the photo across the network<br>
<img width="346" height="284" alt="3" src="https://github.com/user-attachments/assets/1717a4fe-8934-44e9-89a9-5f9a0c2c869e" />
<img width="373" height="436" alt="4" src="https://github.com/user-attachments/assets/fd4a7e95-72fa-4a0c-a84f-73856afb5af6" /><br><br>
2- open group policy management and search for Desktop wallpaper and paste the path of the picture<br>
<img width="555" height="558" alt="5" src="https://github.com/user-attachments/assets/d915150c-b936-4900-98c6-fe538f3b06eb" /><br>

<h3>Testing policies</h3>
