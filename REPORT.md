Project Description 
Library management system: 
This project presents the design and implementation of a Library Management System database. The purpose of the system is to store and manage information related to books, authors, members, borrowing transactions, and staff. The system ensures that library operations such as book registration, member enrollment, borrowing, and returns are handled efficiently.
The project includes the creation of an Entity-Relationship (ER) Diagram, database schema using Data Definition Language (DDL), Data Manipulation Language (DML) operations, and SQL queries to retrieve meaningful information. Assumptions made in the system include:
1.	Each book belongs to one author.
2.	Members can borrow multiple books.
3.	A staff member processes borrowing and return transactions.
4.	All data will be stored in a cloud database platform for collaboration.



ER DIAGRAM DESIGN
 6 simple tables and relationships:
Entities & Attributes
1.	Book
o	BookID  (PK)
o	Title
o	AuthorID (FK)
o	Category
o	Published Year
o	Copies Available
2.	Author
o	AuthorID (PK)
o	FullName
o	Country
3.	Member
o	Member ID (PK)
o	Full Name
o	Email
o	Phone
o	Join Date
4.	Staff
o	StaffID (PK)
o	FullName
o	Position
5.	Borrow
o	BorrowID (PK)
o	MemberID (FK)
o	BookID (FK)
o	StaffID (FK)
o	BorrowDate
o	DueDate
6.	Return
o	ReturnID (PK)
o	BorrowID (FK)
o	ReturnDate
o	ConditionReturned
________________________________________


ERD RELATIONSHIPS
•	Author 1 — M Book
•	Member 1 — M Borrow
•	Book 1 — M Borrow
•	Staff 1 — M Borrow
•	Borrow 1 — 1 Return


ERD Diagram (images/ERD Database.png) 
