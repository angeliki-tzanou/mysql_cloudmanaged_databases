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

- After doing so and accessing my SQL workbench console I went ahead to File and created a new query tab in which I typed my code to create my database as follows, while also ensuring that everything ran properly from the action output terminal on the bottom:
  <img width="900" alt="Screenshot 2023-10-01 at 7 50 59 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/9e9c57de-103a-44f9-a94f-ee66cf4e2f90">

- Then proceeded with adding a new query tab where I pasted the code that was used for this instance, ran it and ensured that the tables were created successfully:
<img width="1000" alt="Screenshot 2023-10-01 at 8 05 33 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/9ee55975-e7b7-48a2-a290-0ff392f84e2d">

- After the tables were created, I clicked on the Database tab and selected the Reverse Engineer (or command R for Mac users) to create my ERD diagram
- In the pop-up window continued through all the steps while selecting my database and my ERD diagram was generated as shown below:
<img width="1000" alt="erd 1" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/bfb425da-51a1-4b0f-b2b5-90155ac45ca5">

- On the bottom when clicking the "Foreign Key" tab you also have the option to edit the relationship between the tables depicted nad change their cardinality from 1 to many, to 1 to 1 as shown above.
- Thats how the EER diagram can be generated.

## My SQL setup on GCP:
- Following a similar process with above, I logged into my GCP account and clicked to enter my main console
- From there I selected from the dropdown to create a new project
- Then under the hamburger icon selected SQL and created a new server
- During the setup process, ensured that stayed within the budget of a low-cost plan and like above had the server open publicly and allowed all to enter through the addition of the 0.0.0.0/0 IP address.
- When satisfied with the options that were picked and clicked on to create the server it took around 13 mins for it to finalize its creation.
- When created, I was redirected to the overview of my server that looked like the pictures shown below:
![Image 10-1-23 at 9 00 PM](https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/7c633c57-3250-49b3-8364-9352cd308ac5)

- Then, proceeded by going into my SQL workbench and creating another connection linking it into my GCP account by filling in the following:
  - Replaced my hostname with my public IP address showing up on the dashboard
  - Ensured the port ```3306``` remained at its default
  - Clicked once again on the "Store in Keychain" option to enter the password used when initially creating the GCP server
<img width="1000" alt="Screenshot 2023-10-01 at 9 03 59 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/e4110a86-5e71-4dec-a753-3ac081dcfcd6">

- After filling in the necessary information as shown above, I tested the connection to ensure that it has connected successfully:
<img width="444" alt="Screenshot 2023-10-01 at 9 06 29 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/e5665213-e25b-4433-9359-5d7ce6059d6a">

- Then after doing so, I clicked on the connection that I had just created on my dashboard and entered my workbench console.
- There I repeated the same steps as for the Azure one above
  - By creating a new query and a new database following the same commands as the ones above
  - With the only difference of the code entered which in this case was the one below:
  ![Image 10-1-23 at 9 10 PM](https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/a194766d-8f88-494a-8ff2-2d79965ef247)
- Then as previously described clicked on the "Database" tab and selected Reverse Engineer where I generated my ERD diagram:
  ![Image 10-1-23 at 9 13 PM](https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/c4030761-d2db-4ade-8148-79eaecca11af)

- Then I was able to go into my Google Shell console and access the SQL monitor by using the command ```mysql --host <IP address> --user <username> --password```
- After doing so it asked to enter the password, which is the same one used when setting up the GCP server.
<img width="900" alt="Screenshot 2023-10-01 at 2 20 58 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/100c230e-bfa2-40d6-8f6a-28f2a4218877">

- Then I was able to depict the contents of the database by doing the following:
<img width="700" alt="Screenshot 2023-10-01 at 2 21 32 PM" src="https://github.com/angeliki-tzanou/mysql_cloudmanaged_databases/assets/141374140/1ee4c89a-e289-45d8-89da-75312e32079f">
