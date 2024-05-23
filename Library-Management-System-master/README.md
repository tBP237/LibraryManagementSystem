## Library Management System

### Functionalities:
* Login
* Add book
* Search books based on Book Title
* Search books based on Category
* Search books based on Author
* List all books and their authors
* Issue books to students
* List books issued to students based on their CMS ID 
* List books which are due for return today

### Database Design

Book Table  | -
----------- | ------------------
Book ISBN	| Primary key
Book Title	| Varchar
Category	| Varchar
No of Books	| int

</br>

Author Table	| -
------------ 	| ----------------------	 
Author Name	 	| Varchar
Author Mail Id	| Varchar
Book ISBN		| Foreign KEY, References Book

</br>

Student Table | -
------------- | --------------------
USN			  | Varchar, Primary Key
Name		  | Varchar

</br>

Book ISSUE Table | -
---------------	 | --------------------------------
Issue ID		 | Auto Increment, Primary Key
USN				 | Foreign Key, References Student
Issued Date		 | Date
Return Date		 | Date
Book ISBN		 | Foreign Key, References Book 

</br>

ADMIN Table		| -
--------------- | --------------------
Admin Id		| Varchar, Primary key
Password		| Varchar

</br>
