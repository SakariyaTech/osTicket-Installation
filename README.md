# osTicket (Help Desk) Installation and Configuration

### Description
This project walks through the manual deployment of osTicket, an open-source help desk system. To get it running, I built out the backend infrastructure on a Windows 10 virtual machine using IIS for the web server, PHP to handle the application logic, and MySQL to host the database.

### Environments and Technologies Used
*   Microsoft Azure (Virtual Machines, Networking)
*   Internet Information Services (IIS)
*   PHP
*   MySQL 

### Operating Systems Used
*   Windows 10

### High-Level Deployment Steps

**Step 1: Web Server Foundation (IIS & PHP)**
*   First, I enabled the Internet Information Services (IIS) feature in Windows and configured CGI. From there, I installed PHP and set up a Handler Mapping in IIS so the web server could properly process the PHP files required by the ticketing system.

<img width="1256" height="355" alt="project1" src="https://github.com/user-attachments/assets/1f72eecd-55af-485c-bd14-2d5008961dd2" />
<img width="1047" height="444" alt="project3" src="https://github.com/user-attachments/assets/90c64c6d-ee88-4ed5-ace7-1fb23b62f18f" />

**Step 2: Database Initialization**
*   Next, I installed MySQL and configured it as the backend database. Using MySQL Workbench and the command line, I provisioned a dedicated database specifically for osTicket to store all the system's users, incoming tickets, and configurations.

<img width="676" height="971" alt="project2" src="https://github.com/user-attachments/assets/41f4d9fe-2d8c-4b12-b243-b76fd975b93a" />

**Step 3: Core Application Deployment**
*   Once the server and database were prepped, I downloaded the osTicket application files, extracted the folders, and moved them directly into the `C:\inetpub\wwwroot\osticket` directory so IIS could serve the application to the web.

<img width="1100" height="614" alt="project4" src="https://github.com/user-attachments/assets/6db47c55-adc0-4339-b3f4-f670f6ef0005" />

**Step 4: System Launch**
*   Finally, I ran the built-in web installer in the browser, linked the PHP application to the MySQL database, and brought the system online. I verified the launch by successfully accessing both the End-User Support Center and the backend Staff Control Panel.

<img width="877" height="800" alt="project 5" src="https://github.com/user-attachments/assets/040da407-26a5-4a72-9048-c2054ec10901" />
<img width="968" height="589" alt="project5" src="https://github.com/user-attachments/assets/a1b335bf-97b9-4c3f-8fcb-13c20ec74c24" />
