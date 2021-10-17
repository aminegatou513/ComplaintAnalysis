
Please note that the ipbix file is connected live to the analyse service database, unfortunately Microsoft PowerBI doesn't support the switch from live connection to Import mode so to view the file and open it yourself, follow these steps.

1- Attach the database files provided in .rar files to your SSMS

2- Open the solution file of Analyse service projet on Visual Studio ( You should have installed SQL Server Data Tools & Analyse Service Extensions from the Visual Studio Market Place  )

3-Change the server name to localhost or to your database server.

4-Deploy the cube 

<<<<<<

If at the Cube deployement you get this error : ' OLE DB or ODBC error : Login Failed for user 'NT Service\MSSQLServerOLAPService:28000'
Then follow these steps : 

OPEN SQL SERVER CONFIGURATION MANAGER : 

![image](https://user-images.githubusercontent.com/68833853/120118265-7e628c00-c189-11eb-9227-f39ea57cb690.png)

Select SQL SERVER SERVICES -> RIGHT CLICK SQL SERVER ANALYSIS SERVICES -> PROPRIETIES

ON THE LOG ON TAB CHOOSE THE BUILT IN ACCOUNT AND CHOOSE LOCAL SYSTEM 

![image](https://user-images.githubusercontent.com/68833853/120118312-d00b1680-c189-11eb-90ea-57b170e268c3.png)

APPLY & RESTART THE SERVICE THEN YOU CAN REDOPLOY THE CUBE 


>>>>>>>

5- Open the PowerBi File !



Best Regards! 
Amine Gatou & Lifi ElMostafa
2020/2021

Bellow are some screenshots from the ibpix file!

Home Page 

![1](https://user-images.githubusercontent.com/68833853/120108894-07b09900-c15f-11eb-81c8-73509bdaf202.png)

About Us & Project 

![2](https://user-images.githubusercontent.com/68833853/120108909-14cd8800-c15f-11eb-8349-ef3a91c2c76c.png)

Complains Analysis 
By General measures
![3](https://user-images.githubusercontent.com/68833853/120108919-24e56780-c15f-11eb-9e94-3f09ccde9a5a.png)
![4](https://user-images.githubusercontent.com/68833853/120108920-257dfe00-c15f-11eb-9529-9a25e3d0d891.png)
![5](https://user-images.githubusercontent.com/68833853/120108921-26169480-c15f-11eb-8c3e-84f1508f678a.png)


By Customers dimension 

![6](https://user-images.githubusercontent.com/68833853/120108925-2ca50c00-c15f-11eb-8d09-67908506f7f5.png)


By Brokers dimension


![7](https://user-images.githubusercontent.com/68833853/120108930-33cc1a00-c15f-11eb-99b2-107d61ee784b.png)


