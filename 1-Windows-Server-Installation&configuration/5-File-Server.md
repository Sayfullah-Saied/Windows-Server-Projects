<h2>File Server configuration</h2>
<hr>
NOTE:
<h4>In a production environment, it is generally recommended to install the file server on a separate machine. However, since this is a lab environment with limited RAM resources, the file server will be configured on the domain controller. The File Server role has already been installed alongside Active Directory Domain Services.</h4>
<hr>
1# We will create three Organizational Units (OUs): HR, Sales, and IT. Within each OU, a dedicated security group will be created to simplify user management and permission assignment.<br>
<img width="391" height="521" alt="1" src="https://github.com/user-attachments/assets/66d6cc58-d264-45f3-9203-180f5a9d474a" />
<img width="380" height="502" alt="2" src="https://github.com/user-attachments/assets/6f1d3202-41be-47ee-851e-ee7ca62c647e" />
<hr><br>
2#On the domain controller, we will create three folders for each group. Each group will only have access to its own folder and will not be able to access or modify other group folders.<br>
<img width="458" height="371" alt="3" src="https://github.com/user-attachments/assets/d5add893-a6c8-4d31-9f7a-e22aae1687c6" /><br><br>
Right-click the folder and select Properties → Sharing → Advanced Sharing → Permissions. Then add the group that belongs to that folder and remove any unnecessary permissions or groups.(do this for all folders)<br>
<img width="454" height="487" alt="11" src="https://github.com/user-attachments/assets/388ecdcd-b249-4002-bc85-cbbc350aefad" />
<hr><br>
3# From the client machine let’s sign in with Khaled from the Sales Group <br>
<img width="413" height="473" alt="4" src="https://github.com/user-attachments/assets/7eaaacff-192a-4abf-9203-75899ad3ce5c" /><br><br>
go to share folders hit Windows+r and write "\\DC1"
<img width="875" height="676" alt="8" src="https://github.com/user-attachments/assets/f7d6d5ce-43b9-4550-ac48-74c649e8f458" /><br><br>
If we open the Sales-Data folder, it will open successfully. However, if we try to access the IT or HR folders, we will receive an Access Denied message.<br>
<img width="752" height="506" alt="6" src="https://github.com/user-attachments/assets/79cb0918-c681-4084-b639-c35b0f757984" />
<img width="848" height="674" alt="10" src="https://github.com/user-attachments/assets/954afc1d-aea0-4a88-9ed7-a9b4672c9172" />
