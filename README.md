# IIT-NIT-IIIT-Analysis-Dashboard

IIT-NIT-IIIT Analysis Dashboard dashboard analyzes opening and closing ranks across different institutes,seat quota and programs offered by IITs, NITs, and IIITs.

---

## Features

- Interactive dashboard for analyzing JoSAA opening and closing ranks of 2025.
- Analyze seat quotas, including General (Gender-Neutral) and Female-only quotas.
- Identify the highest and lowest opening/closing ranks for each program.
- Dynamic filtering by institute type, institute name, program, quota, gender, and academic year
- Relational database designed using MySQL with normalized tables.
- Integrated MySQL database directly with Power BI for real-time analysis.
- Interactive charts, KPIs, slicers, and drill-down reports.
- Easy comparison of admission competitiveness across institutes and branches.
- Uses official JoSAA counselling data, ensuring reliable and accurate insights.

---
## Dashboard KPIs

🏛️ Total Institutes :

1. IITs: 23
2. NITs: 32
3. IIITs: 26

🎓 Total Programs Offered :

1. IITs: 131
2. NITs: 86
3. IIITs: 50

👥 Seat Quota Analysis

1. General (Gender-Neutral) quota
2. Female-only quota

📊 Rank Analysis :

1. Maximum Opening Rank by program
2. Maximum Closing Rank by program
3. Program-wise and institute-wise comparisons

---
## Skills Demonstrated

- SQL Queries
- Database Design
- Data Modeling
- ETL Process
- Power BI
- Data Visualization
- Dashboard Design
- Relational Database Management

---
## Integrating MySQL with Power Bi 

##### Steps :
1. Install MySQL connecotor
   [https://dev.mysql.com/downloads/connector/net/]
2. Open MySQL server command line and create a new MySQL user name
   '''sql
   CREATE USER 'your_user_name'@'localhost' IDENTIFIED WITH mysql_native_password BY
 'Password';
3. Open cmd and type this to change the user name of the MySQL :
   '''sql
   mysql -u your_user_name -p
4. Change the database to use
5. Open MySQL server command line again :
   1. Grant permission to the Power BI to use the database in MySQL
      '''sql
      grant all privileges on database_name to 'powerbi_user'@'localhost';
      flush privileges;  # to reload the granted permission
   2. Then grant permission for the tables in the databse to give acces to Power BI
   3. Use flush privileges to reload the granted permission
6. Open Power BI :
   1. Power BI desktop → File 
   2. Options and settings 
   3. Select MySQL → Clear permissions 
   4. Close Power BI completely
   5. Reopen the  Power BI 
   6. Open the Power BI file where you have to add the database
   7. Go to get data → more
   8. MySQL database 
   9. Server : give the server name
   10. After this it opens this page
       (HERE : use DATABASE  not Windows which in left side of the MySQL database)
!(Screenshot (421).png.png)
   11. After this connection select the table you have to load
  
[!Note]
If error occurs like “ WE COUD’NT AUTHENTICATE….” while connecting : DO the permission granting step in MySQL and also select DATABASE instead of Windows


---
## Demo

https://github.com/user-attachments/assets/f6555f87-da1e-4ee9-a8e7-d5b75d2bdabf






