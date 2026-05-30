<h1>DNS Server</h1>
1. DNS Role Installation:<br>
During the Active Directory Domain Services (AD DS) installation, the DNS Server role was automatically added. A primary DNS zone integrated with Active Directory was created to support domain operations and dynamic updates.<br>

2. Creating an Additional Primary Zone:<br>
To simulate a scenario where DNS is hosted on a separate server—or to maintain tighter administrative control—we will create a new standard primary zone.
This zone will be non‑AD‑integrated and configured to disable dynamic updates, ensuring that DNS records cannot be added or modified without administrative approval.<br>

3. Adding Static DNS Records:<br>
We will manually create the required DNS records:<br>

A Record for the Domain Controller (DC)  
Add the DC’s IP address as a static host (A) record.

A Record for the Client Machine  
Add the client device’s IP address as a static host (A) record.

While creating each A record, ensure the “Create associated PTR record” option is selected.
This automatically generates the corresponding reverse lookup (PTR) entries and creates the reverse lookup zone if it does not already exist.<br>

4. Configuring DNS Forwarders:<br>
To improve external name resolution performance and reliability, configure DNS forwarders:
Add Google Public DNS servers:
8.8.8.8
8.8.4.4
These forwarders will handle queries for domains not hosted internally.
