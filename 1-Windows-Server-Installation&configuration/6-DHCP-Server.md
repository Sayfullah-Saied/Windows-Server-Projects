<h1>DHCP Server Configuration</h1>

<b>NOTE:</b><p>DHCP configuration involves far more than what we will cover on this page. There are server and scope options, backup and restore features, and failover servers. For now, we will explain how to configure an IP address pool and allow users to obtain IP addresses automatically.</p>
<hr><br>
1. Open Add Roles and Features and install the DHCP Server role.<br><br>
<img width="850" height="674" alt="1" src="https://github.com/user-attachments/assets/c29a7267-f614-4ba7-8775-e39577f59c11" /><br><br><br><br>
- Configure a static IP address on the DHCP server before setting up DHCP services.<br><br>
<img width="473" height="489" alt="2" src="https://github.com/user-attachments/assets/44d761e0-1cbc-41b8-975f-eb38f18fa902" /><br><br><br><br>
2. open dhcp server console and select add new scope.<br><br>
<img width="420" height="448" alt="3" src="https://github.com/user-attachments/assets/dfe44229-f5e1-4cc3-a653-05c5036899a4" /><br><br><br><br>
- write the range of iPs from start to end <br><br>
<img width="439" height="526" alt="4" src="https://github.com/user-attachments/assets/b4c36ecb-902a-4b4c-aaf2-edd0770bdf12" /><br><br><br><br>
- write your excluded IPs we will exclude here from 192.168.44.1 - 192.168.44.20<br><br>
<img width="426" height="550" alt="5" src="https://github.com/user-attachments/assets/c506b3d6-9dac-4bc7-8cce-bf4c5e62958c" /><br><br><br><br>
- leave the lease duration at default <br><br>
<img width="476" height="536" alt="6" src="https://github.com/user-attachments/assets/5966eb22-fd54-4b23-884c-b82517a241e0" /><br><br><br><br>
- set the scope options Gateway and DNS<br><br>
<img width="414" height="484" alt="7" src="https://github.com/user-attachments/assets/76d97c6c-4f22-45f9-8cdd-ffa3aefdd9fa" />
<img width="419" height="398" alt="8" src="https://github.com/user-attachments/assets/34c08a2a-124c-4725-9c0f-60d635728378" /><br><br><br><br>
3. Now, let’s open the client machine and run the ipconfig /all command. The device has obtained an IP address from the configured pool, and the DHCP options are correctly applied. Finally, if we open the DHCP console and navigate to Address Leases, we can see the IP address assigned to the client host.<br><br>
<img width="621" height="325" alt="9" src="https://github.com/user-attachments/assets/b086d285-665d-4099-afc7-9da40fb78620" />
<img width="597" height="392" alt="10" src="https://github.com/user-attachments/assets/2fafb683-46ea-4758-ab48-daa3a481dc08" />
