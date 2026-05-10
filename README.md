# Student Management System API

REST API built with Node.js, Express, and MongoDB.

## Setup

Create a `.env` file:
```
MONGO_URI=(YOUR_MONGODB-URL-HERE)
PORT=3000s
```
//Download Zip from here open in cmd
```bash
npm install
npm start
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/students | Add new student |
| GET | /api/students | Get all students (filter: ?department=CS&page=1&limit=10) |
| GET | /api/students/search?name=ali | Search by name |
| GET | /api/students/:id | Get student by ID |
| PUT | /api/students/:id | Full update |
| PATCH | /api/students/:id | Partial update |
| DELETE | /api/students/:id | Delete student |
| PATCH | /api/students/:id/deactivate | Deactivate student |

## Sample Request Body (POST)

```json
{
  "rollNumber": "23F-0560",
  "name": "Husnian Sattar",
  "email": "husnainsattar54@gmail.com",
  "department": "Computer Science",
  "cgpa": 3.78,
  "enrollmentYear": 2023
}
```
