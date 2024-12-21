
# 🚀 FastAPI Student Management API

A simple API to manage student records built with **FastAPI**.

## 🌟 Features
- **Retrieve a student** by ID or name
- **Create a new student**
- **Update an existing student**
- **Delete a student**

## 📖 Endpoints

### 1. Root Endpoint
- **URL:** `/`
- **Method:** `GET`
- **Description:** Welcome message.

### 2. Get Student by ID
- **URL:** `/get-student/{student_id}`
- **Method:** `GET`
- **Description:** Retrieve a student by their ID.
- **Path Parameter:**
  - `student_id` (int): ID of the student. Must be greater than 0.

### 3. Get Student by Name
- **URL:** `/get-student-by-name/{student_id}`
- **Method:** `GET`
- **Description:** Retrieve a student by their name.
- **Query Parameters:**
  - `name` (optional, str): Name of the student.
  - `test` (int): Test value.

### 4. Create a Student
- **URL:** `/create-student/{student_id}`
- **Method:** `POST`
- **Description:** Create a new student.
- **Path Parameter:**
  - `student_id` (int): ID of the student.
- **Request Body:**
  ```json
  {
    "name": "string",
    "age": int,
    "year": "string"
  }
  ```

### 5. Update a Student
- **URL:** `/update-student/{student_id}`
- **Method:** `PUT`
- **Description:** Update an existing student's details.
- **Path Parameter:**
  - `student_id` (int): ID of the student.
- **Request Body:**
  ```json
  {
    "name": "string (optional)",
    "age": int (optional),
    "year": "string (optional)"
  }
  ```

### 6. Delete a Student
- **URL:** `/delete-student/{student_id}`
- **Method:** `DELETE`
- **Description:** Delete a student by their ID.
- **Path Parameter:**
  - `student_id` (int): ID of the student.

## 🔧 Setup and Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name/fastapi-student-api.git
   ```

2. Navigate to the project directory:
   ```bash
   cd fastapi-student-api
   ```

3. Install dependencies:
   ```bash
   pip install fastapi uvicorn pydantic
   ```

4. Run the server:
   ```bash
   uvicorn main:app --reload
   ```

5. Open your browser and navigate to:
   - Swagger UI: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) 📚
   - ReDoc: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc) 📘

## 📂 Folder Structure
```
📦fastapi-student-api
 ┣ 📜main.py         # The main FastAPI application
 ┗ 📜README.md       # Project documentation
```

## 💬 Feedback
If you have any feedback or suggestions, feel free to open an issue or reach out!

---

Made with ❤️ by [Md. Sakibur Rahman]
