## My SQL Setup on Azure:
- First I used the account that I had previously created on Azure
- Then I created a new resource group on the Azure platform and created an SQL server
- There I made sure to have it open to the public and since no information was used that would compromise any PHI the IP address was set to all by typing ```0.0.0.0/0```
- Then selected the appropriate settings for the budget that is provided, set up my server, and went ahead and created it.
- Opened my My SQL Workbench and created another instance under the SQL Connections
<img width="800" alt="Screenshot 2023-10-01 at 2 29 19 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/a7e90db2-80a1-4637-91b6-e81a7801efbb">

- In that pop-up window, I named my connection as ```Azure-ang504-4``` and _**filled in the rest as shown below**_ under the ```Parameters``` tab
  - Ensured that the username matched the name of my SQL database.
  - Copied my Azure server name and pasted in the space asking for the hostname, also ensured that the port number has remained at the default ```3306``` which matches the default port set on my Azure SQL server
  - Lastly clicked on ```store in keychain``` and provided the password that was typed in when creating the database on Azure
 <img width="600" alt="Screenshot 2023-10-01 at 7 28 00 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/c82687d0-6b6f-48d2-9f9a-fc3ee8a29d4e">

  - Clicked on ```Test Connection``` and the connection was made successfully.
<img width="333" alt="Screenshot 2023-10-01 at 7 28 27 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/bd0d99b1-2366-41b8-9c66-894a00bd25b3">

- After doing so and accessing my SQL workbench console I went ahead to File and created a new query tab in which I typed my code to create my database <img width="700" alt="Screenshot 2023-10-01 at 7 50 59 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/5336cb97-d059-43de-a3a7-c32594d8dd99">
as follows
