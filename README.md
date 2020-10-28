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

- Query: **SELECT CompanyName, ContactName, Phone, City FROM Customers WHERE Fax is NULL
UNION
SELECT CompanyName, ContactName, Phone, City FROM Suppliers WHERE Fax is NULL;**

Response: **38**

### Q6 - Ahh there you are! My prize ⭐⭐SPARTANTS⭐⭐! MY MARES AND MY STALLIONS! We need to re-target all of our Customers is Paris! Get me information on these clients.

- Query: **SELECT * FROM Customers WHERE City = 'Paris';**
	- Response: **2**

### Q7 - WAIT! Where are you going? (...) These clients are hard to sell too! We need more intel.. Can you find out, from these clients from Paris, whom orders the most by quantity? Who are our top 5 clients?

- Query:
	- Response:

### Q8 - OMG What are you? Some kind of SQL Guardian Angel? THIS IS AMAZING! May God pay you handsomely 😸 because I have no cash on me!.. I do have one more request. I need to know more about these these Paris client. Can you find out which ones their deliveries took longer than 10 days? Display the Business/client name, contact name, all their contact details (don't forget the fax!), as well as the number of deliveries that where overdue! Just add a column named: 'Number overdue orders'! simple, thank you!

- Query:
	- Response:
