# Technical Interview - Hotel Room Pricing System Challenge

##  Objective: 
Develop a web application that allows users to view hotel room prices based on selected dates.

##  Requirements:

### Hotel Data Structure:
Each **hotel** should have:
- Hotel Name
- Location (City)
- Image URL (optional)

### Room Data Structure:
Each hotel can have **multiple types of rooms**:
- Room Type (e.g., single, double, suite)
- Number of Rooms of that type

### Price Data Structure:
Each room type should have a dynamic pricing model based on the stay date:
- Date of stay
- Price for that specific room type on that date

## Database Setup:
Set up tables for **hotels**, **room types**, and their respective **prices**.
The database admin should support basic CRUD operations for hotels, room types, and their prices.

## Backend:

- An API to fetch **list of hotels**
  - Parameters: none
  - Return: A list of hotels and each of the hotels details
         
- An API to fetch a specific **hotel details**.
  - Parameters: int HotelId
  - Return: All details from the hotel
         
- An API to fetch available room types and their prices **based on a chosen date**, for a specific hotel.
  - Parameters: HotelID, CheckIn Date, CheckOut Date, Number of Rooms
  - Return: Details of the Hotel, List of available Room Types with each os the days price for the room type

## Frontend:
- A simple landing page displaying a list of hotels.
- An option to select a date using a date picker beside each hotel.
- When a date is chosen, display the available room types and their prices for the selected date.
 
##  Guidelines:

- Use PHP, preferable **Laravel** or other Framework
- Prioritize data integrity, especially when dealing with the number of available rooms and their prices.
- Ensure the application is free from basic vulnerabilities like SQL injection.
- Allowed to use any packages that make the work easier
- Allowed to use AI to write the code, but you need to inform that you uses AI
    
##  Evaluation of the exercice

- 35% : Implement the Database and API 
- 10% : Implement a basic CRUD Admin (no need to build fron scratch, might use any external packages)
- 10% : Implement the Frontend
- 20% : Use of code writing best practices, use SOLID principles where possible [Reference](https://www.digitalocean.com/community/conceptual-articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design)
- 10% : Write unit test
- 10% : Documentation
- 5% : Use of docker to setup the project

##  Deliverables:

- Source code of the application, **share the github repository** via email
- A brief documentation explaining your design choices and any assumptions made, including database design diagrams
