# Peer_Learning_Document

# Lav's Approach

### Question 1: Design a data model for a simple e-commerce system

1. Instructions:
    1. Identify the entities in an e-commerce system, including products, categories,
       customers, and orders.
    2. Determine the attributes for each entity, such as product name, price, customer
       name, order date, etc.
    3. Identify the relationships between entities, such as a product can belong to multiple
       categories and a customer can place multiple orders.
    4. Determine the primary keys for each entity, such as product ID for products,
       customer ID for customers, etc.
    5. Create an ER diagram to visually represent the data model.
    6. Write a brief description of the data model, including its purpose, entities,
       relationships, and any assumptions or constraints.
       
       
       
### Solution

#### Purpose

The purpose of the this data model is to organize and represent the data for a simple e-commerce system. The data model identifies the key entities, their attributes, and the relationships between them. It provides a framework for storing and managing data related to products, categories, customers, orders, and order items.

This data model helps to ensure that data is structured and stored in a consistent manner, allowing for efficient and accurate processing of orders and other business transactions. It also allows for easy modification and expansion of the system as needed.

#### Entities
              
* Entities:
    * *Products* A product that can be sold on the e-commerce system
    * *Categories* A category that a product can belongs
    * *Customers* A customer who can place orders on the e-commerce system.
    * *Orders* A record of an order placed by a customer that contains information about the products, quantities and total_price

#### Attributes

* Attributes:

    * *Products:* product_id, product_name, product_description, product_price, product_quantity
    * *Categories:* category_id, category_name
    * *Customers:* customer_id, customer_name, customer_email, contact_number, address
    * *Orders:* order_id, order_date, total_amount, order_status

####  Relationships
Products can belong to multiple categories, and each category can have
multiple products. This is a *many-to-many* relationship, which is
represented by a junction table that connects the products and categories
entities.


Each customer can place multiple orders, but each order can only belong
to one customer. This is a *one-to-many* relationship, which is represented
by a foreign key in the orders entity that references the customer entity.


Each order can contain multiple products, and each product can appear in
multiple orders. This is a *many-to-many* relationship, which is represented
by a junction table that connects the orders and products entities.


#### Primary Keys:
*Product ID* is the primary key for the products entity.<br>
*Category ID* is the primary key for the categories entity.<br>
*Customer ID* is the primary key for the customers entity.<br>
*Order ID* is the primary key for the orders entity.<br>


#### Assumptions/Constraints:
*
    * The e-commerce system only sells physical products and does not deal with digital products.
    * Customers can only purchase products that are currently in stock.
    * Each order can have only one status at a time, such as "pending", "shipped", or "delivered".
    * The prices of the products do not change over time, and the prices.
       
### ER Diagram
<img width="1164" alt="Screenshot 2023-03-11 at 12 30 01 PM" src="https://user-images.githubusercontent.com/122512155/224470226-0395a466-9eb9-4433-b660-37da8028ec4d.png">




### Question 2: Design a data model for a student enrollment system

1. Instructions:
    1. Identify the entities in a student enrollment system, including students, courses, and enrollments.
    2. Determine the attributes for each entity, such as student name, course name, enrollment date, etc.
    3. Identify the relationships between entities, such as a student can enroll in multiple courses and a course can have multiple students.
    4. Determine the primary keys for each entity, such as student ID for students, course ID for courses, etc.
    5. Create an ER diagram to visually represent the data model.
    6. Write a brief description of the data model, including its purpose, entities, relationships, and any assumptions or constraints.
       
       
       
### Solution

#### Purpose

The purpose of this data model is to provide a structured representation of a student enrollment system. The model identifies the key entities, attributes, and relationships that are involved in the system, and specifies the primary keys for each entity. This data model can be used as a blueprint to design a database that stores and manages information about students, courses, and enrollments. 

The data model can also help to ensure that the data is consistent, accurate, and easily accessible for various stakeholders, including students, instructors, and administrators. Additionally, the data model can be used to generate reports and insights on student enrollment trends, course popularity, and other metrics that can inform decision-making in an educational institution.

#### Entities
              
* Entities:
    * *Student* This entity represents the Students of the enrollment system.
    * *Course* This entity represents the courses of the enrollment system.
    
#### Attributes

* Attributes:

    * *Student:* student ID, name, email address, phone number, address and Date of birth.
    * *Course:*  course ID, course name, credits, start date and end date.


####  Relationships
A student can enroll in multiple courses

A course can have multiple students


#### Primary Keys:
*Student ID* is the primary key for the Student entity.<br>
*Course ID* is the primary key for the coursed entity.<br>


#### Assumptions/Constraints:
*
    * Additionally, this data model does not include any additional attributes associated with the enrollment entity, such as grades or attendance records. 
    * Each enrollment record has an associated enrollment date.
       
### ER Diagram
<img width="1358" alt="Screenshot 2023-03-11 at 12 46 59 PM" src="https://user-images.githubusercontent.com/122512155/224470926-db82fef7-4564-444e-8ac4-590a68d12d16.png">


# Sarthak's Approach

### Question 1: Design a data model for a simple e-commerce system (duration: 1.5-2 hours).

### Instructions:

1. Identify the entities in an e-commerce system, including products, categories, customers, and orders.
1. Determine the attributes for each entity, such as product name, price, customer name, order date, etc.
1. Identify the relationships between entities, such as a product can belong to multiple categories and a customer can place multiple orders.
1. Determine the primary keys for each entity, such as product ID for products, customer ID for customers, etc.
1. Create an ER diagram to visually represent the data model.
1. Write a brief description of the data model, including its purpose, entities, relationships, and any assumptions or constraints.

### Solution:-

#### Description:

This data model represents a simple e-commerce system that sells products to customers. The system contains four entities: products, categories, customers, and orders. Products have attributes such as Product\_id,Product\_name, Description, Price, and Image. Categories have attributes such as Category\_id, Category\_name. Customers have attributes such as Customer\_id,Customer\_name, Email, phone number, and Address. Orders have attributes such as Order\_id, Order date, Total\_price and Quantity.The ER diagram visually represents the relationships between the entities, with arrows indicating the direction of the relationships.

#### Purpose:

The purpose of the below ER model is to provide a data model for a simple e-commerce system. The model describes the various entities, attributes, and relationships that exists within the system.The entities in the model include products,categories,customers and orders

Overall,  the purpose of the ER model is to provide a clear and structured representation of the data that is required to build and operate an e-commerce system. It serves as a blueprint for the design and development of the system, ensuring that all necessary data is captured and stored appropriately.

#### Entities:

- Customers : A customer who can place orders on the e-commerce
  - system.
- Products : A product that can be sold on the e-commerce system
- Categories : A category that a product can belong to
- Orders : A record of an order placed by a customer that contains information about the products, quantities and total\_price

#### Attributes:

- Customers :

Customer\_id, Customer\_name, Email, Address, Phone\_number

- Products :

Product\_id, Product\_name, Price, Description, Image

- Categories :

Category\_id, Category\_name

- Orders :

Order\_id, Order\_date, Quantity, Total\_price

#### Relationships:

- A Product can belong to multiple categories and a category can have multiple products (Many-to-Many).
- A customer can place multiple orders, but an order can only be placed by one customer (One-to-Many)
- An order can contain multiple products and a product can be in multiple



|orders|(Many-to-Many|
| - | - |
|||
#### Constraints:

- Entity Integrity Primary Keys:
  - Products : Product\_id
  - Categories : Category\_id
  - Customers : Customer\_id
  - Orders : Order\_id

Intersection Tables:

#### Primary Keys:

- Belongs\_to : Product\_id,Category\_id (Composite Primary Key)
- Contains : Product\_id, Order\_id (Composite Primary Key)
- Referential Integrity Foreign Keys:
- Belongs\_to (Intersection Table) : Defines the relationship between two entities here i.e., Products and Categories

Product\_id (FK) referencing from Product Table and Category\_id(FK) referencing from Categories Table

- Contains (Intersection Table) : Defines the relationship between two entities here i.e., Products and Orders

Product\_id (FK) referencing from Product Table ….              Order\_id (FK) referencing from Orders Table

- As we have One to Many relationship between Customers and Orders So Primary Key of Customers(i.e., Customer\_id) migrates to Orders entity.So,

#### Orders : Customer\_id (FK)

#### Assumptions:-

The Assumptions in this data model are that :-

- Each product can belong to atleast one category
- Each Order must have atleast one product
- Each Customer can have atleast one order

This data model can be used as a basis for the development of an e-commerce system, allowing for the storage and management of products, categories, customers, and orders.

#### ER MODEL:

![1](https://user-images.githubusercontent.com/123646244/226264458-527b712d-8660-4987-b2f4-a9f282a72ff9.jpeg)


### Question 2: Design a data model for a student enrollment system (duration: 1.5-2 hours).

### Instructions:

1. Identify the entities in a student enrollment system, including students, courses, and enrollments.
1. Determine the attributes for each entity, such as student name, course name, enrollment date, etc.
1. Identify the relationships between entities, such as a student can enroll in multiple courses and a course can have multiple students.
4. Determine the primary keys for each entity, such as student ID for students, course ID for courses, etc.
4. Create an ER diagram to visually represent the data model.
4. Write a brief description of the data model, including its purpose, entities, relationships, and any assumptions or constraints.

### Solution:-

#### Description:

This data model represents a student enrollment system where students can enroll in multiple courses and courses can have multiple students. An enrollment is a relationship between a student and a course and includes the enrollment date.The System contains Two Entities i.e., Student and Course.Student consists of an attribute Student\_id,Date of birth(DOB),Gender,Phone\_number,Email,Student\_name which is acting as composite attribute i.e., it can be further categorized to First\_name and last\_name and Address which is also acting as a Composite Attribute i.e., it can be further categorized into State,City,Street and Pincode.The Primary Keys are student\_id and Course\_id

Purpose:

The purpose of the above data model is to represent a student enrollment system. The model is designed to store and manage information related to students, courses, and enrollments. It provides a structure for organizing and storing data related to these entities, including their attributes and relationships. The model can be used to track which courses a student has enrolled in, which students are enrolled in a particular course, enrollment dates .The data model can be used by educational institutions, such as schools or universities, to manage student enrollment and course registration process. It can also be used to generate reports, analyze enrollment trends, and make informed decisions about course offerings and student performance.

#### Entities:

- Student : The entity represents the students who enroll in courses.
- Course : The entity represents the courses that students can enroll in.

#### Attributes:

- Student :

Student\_id, Student\_name(Composite Attribute: can be categorized into ..            First\_name and Last\_name), Email, Address(Composite Attribute: can be ..            categorized into State,City,Street,Pincode), Phone\_number,Gender and ..            DOB

- Course :

Course\_id,Course\_name,Description,End\_date,Instructor\_name,Start\_date, .. Credits

#### Relationships:

- A Student can be enrolled in multiple courses.
- A particular course can have multiple students enrolled
- Here the relationship name is enrollments which is an intersection table defining the relationship between students and course which will contains student\_id and course\_id as foreign key getting referenced from respective table and enrollment\_date as its own attribute which will keep the track of date at which the student is enrolled in a particular course.

#### Constraints:

- Entity Integrity Constraints

#### Primary Keys:

- Student : Student\_id
- Course : Course\_id

#### For Intersection Tables:-

##### Primary Keys:

- Enrollments : Student\_id, Course\_id (Composite Primary Key)
- Referential Integrity Constraints Foreign Keys:
  - Enrollments (Intersection Table) : Defines the relationship between two entities here i.e., Students and Courses

Student\_id (FK) referencing from Student Table and Category\_id(FK) referencing from Categories Table

#### Assumptions:-

The Assumptions in this data model are that :-

- This data model assumes that a student can enroll in multiple courses and a course can have multiple students.
- It also assumes that each enrollment is unique and can be referenced by Course\_id and student\_id acting as a existing as foreign key in Enrollments

intersection table

#### ER MODEL:

![2](https://user-images.githubusercontent.com/123646244/226264500-22641545-b1c4-4b78-97e3-052adbe69a39.jpeg)
