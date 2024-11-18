# Challenge 1 - Restore a SQL Server Backup and Query the Data

## Background story

Woodgrove Retail has running an online retail website for several years and we have access to some archived data. Woodgrove This retailer  is a Internet-based mail order business (B2C business) thats located in Germany and also located in a rural area including storage space (which can be adapted if necessary and with some lead time). There is a small, motivated team, which can be supplemented by auxiliary staff if required.

### Known challenges of the company:

* Significant decline in sales and profits last year
* A high number of returns - partly due to defective and/or delayed items, partly due to "return kings" among customers, and also some suppliers.



## Data diagram

Here is a description of the data

![sqldiagram](images/sqldiagram.png)

* **Orders table**: Contains the previous orders and if there were any returns, discounts, delays impacting the sale
* **Supplier table**: Contains the location of the Supplier
* **Customer table**: Contains the customer demographic information
* **Article table**: Contains information about

## Technical details

The team needs to analyze the data in SQL and figure out the best way to use the provided View (or create your own view)and try and figure out how to solve the known challenges facing the company.
In the Azure Portal you can find the connection information for the database. Utilize [SQL Server Managerment Studio](https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16) to query the data. 



## Success criteria

Connect to the SQL Server instance. After connecting look into the tables & views and try and come up with a query that helps explain why there are so many returns on some items. The team must be able to explain the thought process behind the decisions to the team's coach and provide insights into those decisions. 

## Resources


- https://learn.microsoft.com/en-us/azure/azure-sql/database/connect-query-ssms?view=azuresql


