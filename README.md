# Sql_project

The background of the company:

Universal Furniture Outlet (UFO) sells quality furniture for home and office use.  Its sales representatives use the attached form to take orders.  Customer account numbers on the form are unique.  Customers have only one billing address.  This address is filled out when a new customer account is created or when there is a change of address of an existing customer.  The delivery address is the place where the furniture are to be delivered.  It is filled in the order form if the customer decides to use the delivery service of UFO.  All furniture in one order are delivered to the same address.  UFO offers free delivery service for orders with a total value exceeding $1,000.  For smaller orders it charges a nominal fee of $50.  The customer is not charged the delivery fee if he/she declines to use UFO’s delivery service for orders less than $1,000.      
UFO owns several trucks for delivering customer orders.  Trucks have a vehicle number, license plate number, license expiration date, and inspection expiration date.  Each truck is assigned to a driver, who is an employee of UFO.  Every evening the operations manager plans the next day’s delivery.  Orders are broken into delivery units called shipments so that each shipment may fit into one truck.  A large order that cannot fit into a single truck may be broken into multiple shipments, whereas a small order may be delivered as a single shipment.  Shipments are assigned to trucks that are available for next day’s delivery service.  A truck may carry more than one shipment.  All items included in a shipment are delivered by one truck. Each type of furniture, such as computer desk, executive chair, etc., is identified by an item code.  The price of each furniture type and the quantity in stock are also tracked.
UFO employs several employees.  Each employee has a social security number, name, address, and phone.  A driver, a type of employee, has a driver’s licence number and license expiration date, in addition to other employee information.  Sales reps are also a  type of employee.  All employees are salaried.  Sales reps earn commissions in addition to salaries.    
UFO wants to create an information system to manage its operatons.  UFO’s management team has hired you as consultants for this project.

Requirements
Part I :
Identify the entities in the UFO application.  List each entity with a short definition. Create a relationship matrix to identify relationships among these entities.  Write business rules to describe the relationships among these entities.  Each pair of business rules will have the following format:
Each A is {sometimes | always} related to {one | one or more} B's.
Each  B is {sometimes | always} related to {one | one or more} A's.
Describe supertype-subtypes relationships as: A is a kind of B.
		            		 B can be an A.
You don’t need to create an E-R diagram for this part.


PART II :

a.	Revised Part I. 								

b.	Create two E-R diagrams for the information system using Crow’s foot notation.  One diagram should show all entities and relationships including many-to-many relationships.  The second diagram will include all the entities in the first diagram.  In addition, it will have bridge entities that replace many-to-many relationships.  Do not list attributes on the ERDs.  								

c.  Create a relational schema for your database in fourth normal form.  Describe your schema using the following format.  Note that primary keys are in uppercase and underlined; foreign keys are also underlined but are in lowercase.  You may follow a suitable convention to identify an attribute that is both a primary key and a foreign key.  Clearly indicate the convention that you follow for such attributes.  			

RELATION_NAME (PRIMARY_KEY_ATTRIBUTE(S), non-key attribute(s)).

For example, a relation STUDENT with primary key STUDENT_ID, and attributes name, address, and phone and foreign key major would be:

STUDENT (STUDENT_ID, StudentName, Address, Phone, Major).

d.  Create a data dictionary for your database using the format described in Table 3.6 in Coronel & Morris (pp. 88, 13th Ed.).    Make reasonable assumptions about data types and sizes for different attributes.  You must specify the schema name (the userid of the account in which the tables are created ) in the data dictionary.  

e.	Create Tables in Oracle to implement the UFO database.  This must be done in your UTA Oracle account so that I can verify your implementation. Enter about 5-8 rows in each table.  To document this part in your report, use the Describe command to list the schema of each table followed by the Select command to list its content.  Grant Select to Mahapatra on all tables.						

f.  Execute the following queries using SQL: 							
1.	List all customer names, addresses, and phone numbers. 
2.	Pick an order, and get all information about that order included in the order form.  You don’t need to compute the totals and the delivery fee.  This may be split into two queries, one for the header and the other for the order lines.  
3.	What is the phone number of the salesrep who took order in the query above? 
4.	Pick a driver and list all customers whose orders have been delivered by him/her.
5.	What is the total value (quantity time unit price) of all items in stock that have unit prices exceeding $25?
