* P0-BANKING APPLICATION-JAVA CONSOLE-ANDROID

* Project Description
* Banking APP that allows its users to register as customer & employee, login, fund transfer, deposit, withdraw etc, view transactions etc.


Technologies Used

InteliJ IDE

Features
List of features ready and TODOs for future development

User can log in as either employee or customer depending on login
user information is stored in an SQL database and can be accessed via the console

To-do list:

Adding administrator role so that employees can't delete or add other employees

Getting Started
git clone https://github.com/AntyZhu1/Project0.git
(or download and extract the zip)
create an sql database with the name "banklogins"
create 4 tables in banklogins:

customers:
`
+----------------+-------------+------+-----+---------+----------------+
| Field          | Type        | Null | Key | Default | Extra          |
+----------------+-------------+------+-----+---------+----------------+
| cust_id        | int         | NO   | PRI | NULL    | auto_increment |
| cust_username  | varchar(50) | YES  | UNI | NULL    |                |
| cust_password  | varchar(50) | YES  | UNI | NULL    |                |
| cust_firstname | varchar(50) | YES  |     | NULL    |                |
| cust_lastname  | varchar(50) | YES  |     | NULL    |                |
| cust_money     | double      | YES  |     | NULL    |                |
+----------------+-------------+------+-----+---------+----------------+
`

employees:
mysql> desc employees;
`
+---------------+-------------+------+-----+---------+----------------+
| Field         | Type        | Null | Key | Default | Extra          |
+---------------+-------------+------+-----+---------+----------------+
| emp_id        | int         | NO   | PRI | NULL    | auto_increment |
| emp_username  | varchar(50) | YES  | UNI | NULL    |                |
| emp_password  | varchar(50) | YES  | UNI | NULL    |                |
| emp_firstname | varchar(50) | YES  |     | NULL    |                |
| emp_lastname  | varchar(50) | YES  |     | NULL    |                |
+---------------+-------------+------+-----+---------+----------------+
`

peinding (to handle pending accounts for customers)
`
+-------------------+-------------+------+-----+---------+----------------+
| Field             | Type        | Null | Key | Default | Extra          |
+-------------------+-------------+------+-----+---------+----------------+
| pending_id        | int         | NO   | PRI | NULL    | auto_increment |
| pending_username  | varchar(50) | YES  | UNI | NULL    |                |
| pending_password  | varchar(50) | YES  | UNI | NULL    |                |
| pending_firstname | varchar(50) | YES  |     | NULL    |                |
| pending_lastname  | varchar(50) | YES  |     | NULL    |                |
| pending_money     | double      | YES  |     | NULL    |                |
+-------------------+-------------+------+-----+---------+----------------+
`

transfer-funds:
`
+----------------+--------+------+-----+---------+----------------+
| Field          | Type   | Null | Key | Default | Extra          |
+----------------+--------+------+-----+---------+----------------+
| transfer_id    | int    | NO   | PRI | NULL    | auto_increment |
| transfer_to_id | int    | YES  |     | NULL    |                |
| transfer_money | double | YES  |     | NULL    |                |
+----------------+--------+------+-----+---------+----------------+
`


Usage
Once downloaded or set up, simply run main and follow instructions printed into the console.

Contributors
Me

License
This project uses the following license: <license_name>.
