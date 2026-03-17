# 📘 Students-API

**Students-API** is a RESTful backend service built using Go that manages student records. It provides endpoints to create a student, retrieve a student by ID, and list all students. The API includes request validation, structured JSON responses, and uses a lightweight SQLite database for storage.

---

## 🚀 Features

- Create a new student record  
- Fetch a student by ID  
- Retrieve all students  
- Request validation using structured rules  
- JSON-based API responses  
- Lightweight and fast SQLite database  
- Clean configuration and logging setup  

---

## 🛠️ Tech Stack

- **Language:** Go  
- **API / Server:** `net/http` (ServeMux routing)  
- **Database:** SQLite  

### Database Access
- `database/sql`  
- `github.com/mattn/go-sqlite3`  

### Validation
- `github.com/go-playground/validator/v10`  

### Configuration
- `github.com/ilyakaznacheev/cleanenv`  
- `github.com/joho/godotenv`  

### Logging
- `log/slog`  

---

## 📂 API Endpoints

| Method | Endpoint         | Description              |
|--------|----------------|--------------------------|
| POST   | `/students`     | Create a new student     |
| GET    | `/students/{id}`| Get student by ID        |
| GET    | `/students`     | List all students        |

---

## ⚙️ Setup & Run

```bash
# Clone the repository
git clone <your-repo-url>

# Navigate to project directory
cd students-api

# Install dependencies
go mod tidy

# Run the server
go run main.go
