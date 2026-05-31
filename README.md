# 🎬 Movie Ticket Reservation System

Movie Ticket Reservation System is a backend application developed using **Spring Boot** that manages movies, theaters, shows, users, and ticket bookings through REST APIs. The project implements CRUD operations, database integration, and a layered backend architecture commonly used in real-world applications.

## 🛠️ Tech Stack

- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL
- Lombok

## ✨ Features

- Add, view, update, and delete movies, theaters, shows, users, and tickets
- Search movies using title and genre
- Pagination for retrieving movie data
- Email sending functionality using JavaMailSender
- REST API-based architecture

## 📂 Project Structure

- **Controller** – Handles API requests
- **Service** – Contains business logic
- **Repository** – Manages database operations using JPA
- **Entity** – Represents database tables

## 🎟️ Modules

- **Movie** – Stores movie details such as title, genre, and duration
- **Theater** – Stores theater name and location
- **Show** – Contains movie show details and pricing
- **User** – Manages user information
- **Ticket** – Stores ticket booking and seat details

## ⚙️ How It Works

The application exposes REST endpoints for managing movie ticket booking data. Requests are handled by the controller layer, processed in the service layer, and stored or retrieved from the database using JPA repositories.

## 🚀 Run the Project

1. Clone the repository
2. Configure MySQL database settings in `application.properties`
3. Run the Spring Boot application
4. Access APIs using Postman or Swagger

## 📚 Learning Outcome

This project helps in understanding:

- Spring Boot backend development
- REST API design
- CRUD operations
- Database integration using JPA
- Layered backend architecture
