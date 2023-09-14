Restaurant Database SQL Project
Introduction
This SQL project revolves around the creation and management of a restaurant database. In this project, I have designed a relational database system with tables for employees, menu items, reservations, and orders. 
I populated it with mock data by ChatGPT, where each reservation requires an associated employee, and clients can order multiple food items for a single reservation; subsequently, I uploaded the database to ChatGPT and requested the generation of exercises at three different difficulty levels.

Database Structure
The database consists of the following tables:

1. Employees
employee_id (Primary Key): Unique identifier for each employee.
name: First name of the employee.
surname: Last name of the employee.
phone_number: Contact phone number of the employee.
date_of_birth: Date of birth of the employee.
employment_type: Type of employment (e.g., full-time, part-time).

3. Menu Items
item_id (Primary Key): Unique identifier for each menu item.
dish_name: Name of the menu item.
vegetarian: Indicates whether the item is suitable for vegetarians (Boolean).
vegan: Indicates whether the item is suitable for vegans (Boolean).
price: Price of the menu item (decimal).

5. Reservations
reservation_id (Primary Key): Unique identifier for each reservation.
table_number: Table number where the reservation is made.
number_of_people: Number of people in the reservation.
reservation_datetime: Date and time of the reservation.
employee_id (Foreign Key): Employee responsible for the reservation.

7. Orders
order_id (Primary Key): Unique identifier for each order.
reservation_id (Foreign Key): Reservation associated with the order.
item_id (Foreign Key): Menu item included in the order.
