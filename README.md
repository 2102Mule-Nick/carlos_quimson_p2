# American Flights API

The American Flights API is a system API for operations on the american table in the flights database. It supports the following operations: get all flights, get a flight with a specific ID, add a flight, delete a flight, partially update a flight, and replace a flight.

## Technologies Used
1. Mulesoft
2. Anypoint Platform
3. Anypoint Studio
4. REST
5. PostgreSQL
6. AWS RDS

## Features
1. Get all flights from an AWS RDS databae
2. Get a single flight via flight ID
3. Add a flight to the AWS RDS database
4. Delete a flight
5. Partially update a flight by updating its price and empty seats capacity
6. Replacing a flight

### To-do list
- Refactor to follow best practices 
- Implement MUnit for testing

## Getting Started
#### Copy the repo via executing the command: 
  `git clone https://github.com/PorkodiVenkatesh/PROJECT-NAME#project-name`
  
#### Database Setup
The database that the application works with requires the table to have the following columns:
- id - integer/serial
- code - text
- price - float
- departuredate - text
- origin - text
- destination - text
- emptyseats - int
- planetype - text
- totalseats - int

#### Usage
The application must be opened in Anypoint Studio and run. 

Use Advanced Rest Client to see how the application works. A sample input data is included below.

```
{
    "id": 4,
    "code": "ffee0192",
    "price": 300,
    "origin": "MUA",
    "destination": "LAX",
    "departureDate": "2016-01-19",
    "emptySeats": 0,
    "plane": {
      "totalSeats": 300,
      "type": "Boeing 777"
    }
  }
```
