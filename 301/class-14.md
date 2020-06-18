# DataBase Normalization
[DB Normalization](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)

[Definition of a DataBAse Table](https://www.essentialsql.com/what-is-a-database-table/)

DB normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included. Take a spreadsheet containing the information as an example, where the data contains salespeople and customers serving several purposes:

- Identify salespeople in your organization
- List all customers your company calls upon to sell a product
- Identify which salespeople call on specific customers.

By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.
## Reasons for Database Normalization
There are three main reasons to normalize a database.  
- The first is to minimize duplicate data
- The second is to minimize or avoid data modification issues.
- The third is to simplify queries. 

## Data Duplication and Modification Anomalies
Notice that for each SalesPerson we have listed both the SalesOffice and OfficeNumber. There are duplicate salesperson data. Duplicated information presents two problems:

- It increases storage and decrease performance.
- It becomes more difficult to maintain data changes.

There are three modification anomalies that can occur:

- Insert Anomaly
- Update Anomaly
- Deletion Anomaly

## Search and Sort Issues
The last reason we'll consider is making it easier to search and sort your data.

## Definition of Database Normalization
There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively.

