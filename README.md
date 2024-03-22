# How to migrate database data from SQL Server 2000@Windows Server 2003 to AWS RDS SQL Server 2019

## Here is my notes on doing data migration from SQL Server 2000 to SQL Server 2019

Please note: 
- I am connecting using SQL Server Management Studio 19.3
- The machine that run the above is Windows Server 2022 Datacenter
- You must confirm that you can connect to your on-premise DB and RDS.
- In case you meet any errors, you can choose certain tables to migrate first instead of running it all.

Hope that helps.

1. Use SQL Server Import and Export Wizard: Choose SQL server Native Client 10.0
2. Enter the source (SQL Srv 2k).  Server name is DB IP, and username password.
![image](https://github.com/alucard001/migrate-from-2k3-to-rds-sql-server-2019/assets/1968244/2a3ece30-fb62-4c1a-9e99-13ce8f715c35)

1. Enter the destination   
![image](https://github.com/alucard001/migrate-from-2k3-to-rds-sql-server-2019/assets/1968244/a65ca0ae-1de8-4443-bf9d-0721b453ec7d)

1. Select: Copy data from one or more tables or views.
![image](https://github.com/alucard001/migrate-from-2k3-to-rds-sql-server-2019/assets/1968244/8317ac7f-6399-40b2-9300-879cbc9dc3ec)

1. Select which table(s) you would like to migrate
![image](https://github.com/alucard001/migrate-from-2k3-to-rds-sql-server-2019/assets/1968244/e851b49a-12eb-4f5e-b23d-ac01a27fb434)

1. Map the column
![image](https://github.com/alucard001/migrate-from-2k3-to-rds-sql-server-2019/assets/1968244/d4792f3a-5f03-45b3-a655-28e8798ea371)

1. Select "Run immediately"
![image](https://github.com/alucard001/migrate-from-2k3-to-rds-sql-server-2019/assets/1968244/8f2636d4-7e35-4dd0-8148-2b54ce5572be)

1. The process will start
![image](https://github.com/alucard001/migrate-from-2k3-to-rds-sql-server-2019/assets/1968244/f7fa17b1-c6fc-4f3f-b475-cfddbd7c5a31)
