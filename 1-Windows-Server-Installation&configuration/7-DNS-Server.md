<h1>DNS Server</h1>
1. DNS Role Installation:<br>
During the Active Directory Domain Services (AD DS) installation, the DNS Server role was automatically added. A primary DNS zone integrated with Active Directory was created to support domain operations and dynamic updates.<br>
<img width="871" height="668" alt="1" src="https://github.com/user-attachments/assets/91d274af-21e8-45f0-a8c1-2e1bde9c1e1e" /><br><br><hr>
2. Creating an Additional Primary Zone:<br>
To simulate a scenario where DNS is hosted on a separate server—or to maintain tighter administrative control—we will create a new standard primary zone.
This zone will be non‑AD‑integrated and configured to disable dynamic updates, ensuring that DNS records cannot be added or modified without administrative approval.<br>
<img width="616" height="425" alt="2" src="https://github.com/user-attachments/assets/8fca65cf-b706-4860-855d-1e88acea3cc4" /><br><br><hr>
3. Adding Static DNS Records:<br>
We will manually create the required DNS records:<br>
A Record for the Domain Controller (DC) <br> 
Add the DC’s IP address as a static host (A) record.<br>
<img width="372" height="342" alt="3" src="https://github.com/user-attachments/assets/e506a948-91f8-4976-b5b8-82dcacc31d25" /><br>
A Record for the Client Machine<br>
Add the client device’s IP address as a static host (A) record.<br>
<img width="340" height="347" alt="4" src="https://github.com/user-attachments/assets/4533191a-a8d4-4585-b86a-720958034950" /><br>
While creating each A record, ensure the “Create associated PTR record” option is selected.<br>
This automatically generates the corresponding reverse lookup (PTR) entries and creates the reverse lookup zone if it does not already exist.<br><br><hr>
4. Configuring DNS Forwarders:<br>
To improve external name resolution performance and reliability, configure DNS forwarders:<br>
Add Google Public DNS servers:<br>
8.8.8.8<br>
8.8.4.4<br>
<img width="587" height="517" alt="5" src="https://github.com/user-attachments/assets/234e8783-8ef9-4848-ae82-61a48f6993e8" /><br>
These forwarders will handle queries for domains not hosted internally.
