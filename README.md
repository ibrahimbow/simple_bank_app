
Welcome to mymweb 
(Simple bank web Application)


Idea:
Money Transaction: The client can have an account and be able to send the money to another account.

Purpose:
Build web application with java language and implementing the following structures:
- Login
* Not allowed to login if it�s not existed in the database
* After log out cannot comeback without login again
* Not allowed Empty values 

- Register  
* Not allowed for duplicate email and username 
* Not allowed for empty values 
* Generate unique account numbers 
* Generate amount ( This part is only for registration made by user for the first time)

- Welcome client for Transaction
* Able to get the client name on page 
* Able to get the account number of the client on page
* Able to get the amount of the client which is updated automatically in case its changed
* Unable to input characters 
* Able to transfer money from one account to another account smoothly
* Check if the account number is valid otherwise cannot transfer money
* Prevent transfer money if the client has not enough amount 
* Get all the transactions of money list 
* Get all the transactions of the client which are updated automatically 
* Get the account number of Transaction 
* Get the date and time of the transaction
* Get the withdraw and Deposit transaction Type for each operation








- Admin 
* Clients info 
o View all clients information
* Create
o Add new client 
o Not allowed duplicate exists username and email 
o Able to put amount ( Not generated by itself)

* Update
o Get the client info by Searching for Account number 
o Get the information of the client and able to edit it and save it 
* Delete
o Remove the client from database
o This delete will be in all tables in database that related to the client
* Transaction
o View all transactions of all clients
* log info 
o Get the log info for all clients (date) of login in web application

Requirements 
Materials & tools
- Intellij
- Project build with Maven
Language
- Java jdk 11
Database
- MYSQL
- SQL
- JDBC/JPA
Server
- Tomcat 9
Frontend 
- HTML5  
- CSS
- JavaScript/jQuery
- JSP / Servlets
- XML









DATABASE:


ER Diagram












Java Classes : 
Entity - JPA

Entity-Relationship Diagram


MyController class is responsible for all operations 

Custom Exception class



DAO
Dao interface implemented by  Admin Dao class which is responsible for the CRUD of administration 


Service package has two classes which are responsible to generate account numbers and generate amount for the new client who registers by himself for the first time.



Servlet






Intellij � Path java classes































Web Application Contents diagram 






















User Interface

Login
It has alert messages in case the username it�s not exists in database


Signup
It has alert messages in case the duplicate username and password or incorrect email typed

Welcome
Welcome page for the client to transfer money and see the transactions 

This alert show up when the amount is not enough and the account number is not exists and to confirm send the money





Transactions

Admin 
Home page


View Clients information




 Add new Client
It has alert messages in case the duplicate username and password or incorrect email typed

Edit and Delete Client
It has search field for account number after you finished type it. It checks if its exists or not . In case if its exists it gets  the info from database and auto load it in the fields which is be easy to edit it otherwise you get alert message that�s not exists
And it has alert messages in case the duplicate username and password or incorrect email typed
Also show alert message before you delete account to make sure that is confirmed by you.


Transactions
View all transactions for all clients


Logs
View all log for all the clients that they login in web application


14


