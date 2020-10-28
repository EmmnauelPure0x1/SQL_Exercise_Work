# SQL_Exercise_Work

### Q1 - How many orders in NWDB?

- Query: **SELECT COUNT(*) FROM Orders;**
	- Response: **830**

### Q2 - How many order that the Ship City is Rio de Janeiro?

- Query: **SELECT COUNT(*) FROM Orders WHERE ShipCity = 'Rio de Janeiro';**
	- Response: **34**

### Q3 - Select all orders that the Ship City is Rio de Janeiro or Reims?

- Query: **SELECT COUNT(*) FROM Orders WHERE ShipCity = 'Rio de Janeiro' OR ShipCity = 'Reims';**
	- Response: **39**

### Q4 - Select all of the entries where the Company name has a z or a Z in the table of Customers

- Query: **SELECT * FROM Customers WHERE CompanyName LIKE '%[Zz]%';** 
	- Response: **6**

### Q5 - We need to update all of our FAX information! This Day and age it is a must! 😅😅😅 Find me the Name of All of the companies that we do not have their FAX numbers! I would also like to know with whom I need to speak with, their contact numbers and what city they are base in.

Query: ``` **SELECT CompanyName, ContactName, Phone, City FROM Customers WHERE Fax is NULL
UNION
SELECT CompanyName, ContactName, Phone, City FROM Suppliers WHERE Fax is NULL;** ``` 

Response: **38**
