# Bus Management System

## Project Overview
The Bus Management System is an advanced software solution designed to streamline and automate operations involved in managing bus services. It covers aspects such as route planning, passenger bookings, and payment processing, providing a comprehensive platform for bus operators to efficiently manage their services and enhance the overall passenger experience.

## Key Features
- **Route Management**: Create, update, and manage bus routes, including starting points, destinations, stops, and service frequency.
- **Schedule Management**: Efficiently manage bus schedules, assign buses to specific schedules, and adjust as needed.
- **Booking Management**: Allow passengers to book seats, make payments, receive confirmations, and manage bookings.
- **Passenger Management**: Track passenger information and provide personalized services.
- **Bus Management**: Manage bus details, seating capacity, assignments, and maintenance schedules.
- **Payment Management**: Secure payment processing and management of payment records.

## System Architecture
The system is divided into three tiers:
- **Client Tier**: Web, mobile, and desktop applications for user interfaces.
- **Application Tier**: Web and application servers handling APIs, business logic, and processing.
- **Data Tier**: MySQL database server for managing data related to passengers, bookings, routes, buses, and payments.

## Database Structure
- **Passengers**: Stores passenger details.
- **Drivers**: Stores driver details and credentials.
- **Bookings**: Manages booking details, connecting passengers, routes, and buses.
- **Routes**: Stores route information, including origin, destination, and distance.
- **Buses**: Contains bus details like capacity and type.
- **Payments**: Manages payment details, linked to bookings.

## SQL Queries and Procedures
The project includes several SQL queries and procedures, such as:
1. List active buses with their capacity and type.
2. Calculate the total fare collected for each bus.
3. Retrieve booking details along with related passenger and route information.

**Example SQL Query:**
```sql
SELECT bus_number, capacity, type
FROM Buses
WHERE status = 'Active';
