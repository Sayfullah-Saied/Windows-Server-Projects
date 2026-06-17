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
2- open group policy management and search for Desktop wallpaper, enable it and paste the path of the picture<br>
<img width="555" height="558" alt="5" src="https://github.com/user-attachments/assets/d915150c-b936-4900-98c6-fe538f3b06eb" /><br><br>
<h1>Prevent Access to Control Panel</h1>
Second policy Prevent access to control panel by the following:<br>
1- Search for prohibit access to control panel and PC settings and enable it <br>
<img width="395" height="409" alt="6" src="https://github.com/user-attachments/assets/7181c5bc-d875-4ace-b3a8-add535400de7" /><br>
<h1>Remove Run</h1>
search for Remove run menu from start menu, set it to enable<br>
<img width="572" height="518" alt="7" src="https://github.com/user-attachments/assets/60b84675-7658-4de9-b36b-13d04e746afe" /><br>
<h1>Disable USB</h1>
search for Removable Disks: Deny read and write access<br>
<img width="523" height="542" alt="8" src="https://github.com/user-attachments/assets/f60047db-4a7b-411e-92d8-66ffc7c0381e" /><br>
<h1>Map Network Drive</h1>
add the path of the shared folder, set the letter to Z, enable Reconnect<br>
<img width="580" height="404" alt="9" src="https://github.com/user-attachments/assets/07ddedbb-b824-4959-9325-aa0993153dbd" /><br>
Finally let's link all the policies to the domain:<br>
<img width="158" height="140" alt="10" src="https://github.com/user-attachments/assets/5d54414e-55e2-4f72-8120-c676b69ed9cb" /><br>

<h3>Testing policies</h3>
<p>we will sign in with the user khaled </p>
<img width="476" height="379" alt="11" src="https://github.com/user-attachments/assets/28a614da-55b7-4285-bdef-af23e815a017" /><br>
we see that the background policy has been applied successfully to the user and if we try to open RUN we get the following error<br>
<img width="718" height="527" alt="12" src="https://github.com/user-attachments/assets/78d6ee8f-7dcd-4f0e-9d25-c98540b01173" /><br>
the shared drive also applied successfully<br>
<img width="672" height="420" alt="13" src="https://github.com/user-attachments/assets/72f700a2-b982-4e5e-b830-97ab4d076f80" /><br>
if we try to open control panel we get the followig error<br>
<img width="517" height="510" alt="14" src="https://github.com/user-attachments/assets/1cdbd7e0-d709-40ae-914a-43c92edbbd96" />
<img width="581" height="308" alt="15" src="https://github.com/user-attachments/assets/9728ef70-9d7d-44e2-b770-bb1f019d8ac6" />

