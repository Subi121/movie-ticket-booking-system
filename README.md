# 🎬 Movie Ticket Reservation System

Movie Ticket Reservation System is a backend application developed using **Spring Boot** that manages movies, theaters, shows, users, and ticket bookings through REST APIs. The project implements CRUD operations, database integration, and a layered backend architecture commonly used in real-world applications.

# 🎬 Movie Ticket Reservation System

![Java](https://img.shields.io/badge/Java-17-orange)
![Spring Boot](https://img.shields.io/badge/SpringBoot-Backend-brightgreen)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue)
![REST API](https://img.shields.io/badge/API-REST-yellow)
![License](https://img.shields.io/badge/license-MIT-green)

A backend REST API application built with **Spring Boot** that manages movies, theaters, shows, users, and ticket bookings.

---

## 🛠️ Tech Stack

* Java 17 · Spring Boot · Spring Data JPA · Hibernate · MySQL · Lombok · JavaMailSender · Maven

---

## ✨ Features

* Full CRUD for Movies, Theaters, Shows, Users, and Tickets
* Advanced search: `StartsWith`, `EndsWith`, `Contains`, `AND`, `OR`, `IN`
* Pagination using `PageRequest`
* Email sending via `JavaMailSender`
* Clean layered architecture: Controller → Service → Repository → Database

---

## 📂 Project Structure

```
src/main/java/com/example/project/
├── Controller    → REST API request handling
├── Service       → Business logic
├── Repository    → JPA database operations
├── Entity        → Database entity classes
```

---

## 🔗 API Endpoints

### Core CRUD

| Module  | GET | POST | PUT | DELETE |
|---|---|---|---|---|
| Movies   | `/gett2`    | `/postt2`    | `/putt2/{id}`    | `/deletet2/{id}`  |
| Theaters | `/gett1`    | `/postt1`    | `/putt1/{id}`    | `/deletet1/{id}`  |
| Shows    | `/gett4`    | `/postt4`    | `/putt4/{id}`    | `/deletet4/{id}`  |
| Users    | `/gett3`    | `/postt3`    | `/putt3/{id}`    | `/deletet3/{id}`  |
| Tickets  | `/gett5`    | `/postt5`    | `/put5/{id}`     | `/deletet5/{id}`  |

### Search & Utility

| Endpoint | Description |
|---|---|
| `/startspro?title=` | Starts with |
| `/endspro?title=` | Ends with |
| `/containspro?title=` | Contains |
| `/and?title=&genre=` | AND condition |
| `/or?title=&genre=` | OR condition |
| `/in?title=v1,v2` | IN query |
| `/Page?page=0&size=5` | Pagination |
| `/sendmail` | Send email (`receiver`, `subject`, `body`) |

---

## ⚙️ Setup

```bash
git clone https://github.com/your-username/movie-ticket-reservation-system.git
cd movie-ticket-reservation-system
```

Configure `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/movie_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

```bash
mvn spring-boot:run
```

Test with **Postman** or **Swagger UI**.

---

## 🚀 Future Improvements

* JWT Authentication & Role-Based Access Control
* Online Payment Integration
* Swagger/OpenAPI Documentation
* Docker Deployment
* Input Validation & Global Exception Handling
* Seat Availability Tracking

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
