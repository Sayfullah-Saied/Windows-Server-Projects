<h2 align="center">Remote Management</h2>
<hr>
# I will explain 3 ways to remotly manage windows server:<br>
1-Winrs<br>
2-Remote Desktop connection<br>
3-RSAT<br>
<hr><br>
#First, let's try Winrs which is a shell to execute commands, let't try the hostname command on the server from client pc:<br>
<img width="820" height="515" alt="1" src="https://github.com/user-attachments/assets/1bf915ba-06d7-4c57-b772-69f4ccb73760" />
<hr><br>
# second, we have remote desktop connection let's start by opening it and supply the admin credentials:<br>
<img width="758" height="366" alt="2" src="https://github.com/user-attachments/assets/343e2de9-ba99-47b7-9b20-9178afff6fdf" /><br>
<img width="674" height="699" alt="3" src="https://github.com/user-attachments/assets/a476186b-ec5d-4a9e-a984-8575ec78bc21" /><br>
<b>connected</b><br>
<img width="988" height="696" alt="4" src="https://github.com/user-attachments/assets/d43e3837-5c07-46e3-bd75-09b92a3b3741" /><br>
<hr><br>
# lastly, let's download RSAT server manager on the client machine, go to windows seach --> optional features --> install RSAT server manager:<br>
<img width="647" height="688" alt="5" src="https://github.com/user-attachments/assets/5f2232df-4d92-4b19-b5bc-c73b2099c5fc" /><br><br>
after installing is done right click on it and select run as different user and use the domain admin credentials:<br>
<img width="497" height="622" alt="6" src="https://github.com/user-attachments/assets/13d56994-3c8c-4fde-8f83-14592136e6d2" /><br><br>
add the domain controller and you good to go, you can add roles and features and open powershell and many more from client pc<br>
<img width="593" height="674" alt="7" src="https://github.com/user-attachments/assets/4538442f-1877-4a07-b2aa-daf69c4b8481" />
<img width="561" height="310" alt="8" src="https://github.com/user-attachments/assets/b63df914-585b-4ffc-babc-65585580a441" />
