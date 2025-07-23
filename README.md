# IRCTC Train Booking System

A Java-based backend system for train ticket booking and management, similar to IRCTC. Built using Gradle and Java 8.

## Features

- **User Management**
  - Sign up with username and password (secure password hashing)
  - User authentication/login
  - View booking history

- **Train Operations**
  - Search trains between source and destination
  - Real-time seat availability checking
  - Seat booking with row and column selection
  - Booking cancellation

- **Data Persistence**
  - JSON-based local storage for users and trains
  - Jackson for JSON serialization/deserialization

## Tech Stack

- Java 8
- Gradle 8.14.3
- Dependencies:
  - Jackson Databind 2.15.2
  - JBCrypt 0.4
  - Lombok 1.18.32
  - JUnit for testing

## Project Structure
app/
└── src/
    └── main/
        └── java/
            └── ticket/
                └── booking/
                    ├── entities/
                    │   ├── Train.java
                    │   ├── Ticket.java
                    │   └── User.java
                    ├── service/
                    │   ├── TrainService.java
                    │   └── UserBookingService.java
                    ├── util/
                    │   └── UserServiceUtil.java
                    └── localDb/
                        ├── trains.json
                        └── users.json


## Setup & Running

1. Clone the repository
2. Ensure Java 8 and Gradle are installed
3. Build the project:
   ```bash
   ./gradlew build
