# PremierZone – Premier League Player Analytics Dashboard

PremierZone is a full-stack football analytics platform built to manage, visualize, and analyze Premier League player statistics.

The application integrates a Spring Boot backend with a React frontend to provide real-time player data access, dynamic filtering, and smooth API-driven communication.

The frontend automatically connects to the backend APIs running on port `8080`, enabling seamless data retrieval and interaction.

---

## Project Overview

PremierZone is designed as a centralized dashboard for exploring player performance statistics across the Premier League season.

It supports:

- Player statistics visualization
- Team-based filtering
- Position-based filtering
- Nation-based filtering
- Name-based search
- Real-time backend API integration
- PostgreSQL data persistence
- Full CRUD operations

The project demonstrates strong full-stack development skills including backend API development, database integration, frontend development, and clean REST architecture.

---

## Tech Stack

### Backend
- Java
- Spring Boot
- Spring Web
- Spring Data JPA
- Hibernate
- REST APIs

### Frontend
- ReactJS
- JavaScript
- HTML
- CSS

### Database
- PostgreSQL
- SQL Queries

### Tools
- Maven
- IntelliJ IDEA
- Postman
- Git
- GitHub

---

## Features

### Backend Features
- RESTful API architecture
- CORS configuration for frontend-backend communication
- CRUD operations for player records
- Dynamic filtering APIs
- Service layer architecture
- Repository pattern using JPA
- Transaction management

### Frontend Features
- Clean football analytics dashboard UI
- Search by player name
- Filter by team
- Filter by nation
- Filter by player position
- Refresh and clear filters
- Real-time API integration
- Automatic backend connection on application startup

### Database Features
- Player statistics stored in PostgreSQL
- Efficient querying using Spring Data JPA
- Real-time updates through API calls

---

## Project Structure

```text
PremierZone
│
├── backend
│   ├── controller
│   ├── service
│   ├── repository
│   ├── entity
│   └── config
│
├── frontend
│   ├── components
│   ├── pages
│   ├── services
│   └── styles
│
└── database
```

---

## Backend API Endpoints

### Get All Players
```http
GET /api/v1/player
```

### Filter By Team
```http
GET /api/v1/player?team=Arsenal
```

### Search By Name
```http
GET /api/v1/player?name=Haaland
```

### Filter By Position
```http
GET /api/v1/player?position=FW
```

### Filter By Nation
```http
GET /api/v1/player?nation=England
```

### Add New Player
```http
POST /api/v1/player
```

### Update Player
```http
PUT /api/v1/player
```

### Delete Player
```http
DELETE /api/v1/player/{playerName}
```

---

## Player Statistics Included

The application tracks multiple performance metrics including:

- Name
- Team
- Nation
- Position
- Age
- Matches Played
- Starts
- Minutes Played
- Goals
- Assists
- Penalties Scored
- Yellow Cards
- Red Cards
- Expected Goals (xG)
- Expected Assists (xAG)

---

## Database Entity

The `Player` entity maps player statistics into the `player_statistic` table.

Main fields include:

- `id`
- `player_name`
- `team_name`
- `nation`
- `position`
- `age`
- `goals`
- `assists`
- `xg`
- `xag`

---

## How to Run the Project

### Backend

Move to backend project folder:

```bash
cd backend
```

Run Spring Boot application:

```bash
mvn spring-boot:run
```

Backend runs on:

```text
http://localhost:8080
```

---

### Frontend

Move to frontend folder:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Run frontend:

```bash
npm start
```

Frontend automatically connects to backend APIs on port `8080`.

---

## CORS Support

The backend includes global CORS configuration to allow smooth communication with the React frontend.

```java
.allowedOrigins("*")
.allowedMethods("*")
.allowedHeaders("*")
```

---

## Key Learning Outcomes

This project helped strengthen knowledge in:

- Full-stack application development
- REST API design
- React frontend integration
- Database modeling
- Spring Boot architecture
- JPA and Hibernate
- SQL querying
- Data filtering logic
- Clean code practices

---

## Future Enhancements

- Match outcome prediction using Machine Learning
- Player performance comparison charts
- Team ranking system
- Authentication and authorization
- Deployment using Docker and cloud services
- Live football API integration

---

## Author

**Phanindra Mekala**  
