Student Management System API (Python + Flask)

A simple and scalable REST API built using Python and Flask to manage student records.  
This backend application supports CRUD operations, MySQL database integration, and follows a clean modular structure suitable for backend developer internship roles.

------------------------------------------
FEATURES
------------------------------------------
- Add new students  
- Update student details  
- Delete student records  
- Fetch all students  
- MySQL database integration  
- Modular Flask project structure  
- API tested using Postman  
- Easily extendable (courses, attendance, departments, etc.)

------------------------------------------
TECH STACK
------------------------------------------
Language: Python  
Framework: Flask  
Database: MySQL  
Tools: Postman, Git, JSON  
Libraries: mysql-connector-python, PyJWT (optional)

------------------------------------------
FOLDER STRUCTURE
------------------------------------------
Student-Management-API/  
│-- app.py  
│-- database.py  
│-- requirements.txt  
│-- README.md  
│-- models/  
│     student.py  
│-- routes/  
│     student_routes.py  
└── utils/  
      auth.py (optional)

------------------------------------------
INSTALLATION AND SETUP
------------------------------------------

1. Clone the repository:
git clone https://github.com/YourUsername/Student-Management-API.git
cd Student-Management-API

2. Install dependencies:
pip install -r requirements.txt

3. Create MySQL database:
CREATE DATABASE student_db;

4. Run the project:
python app.py

API runs at:
http://127.0.0.1:5000

------------------------------------------
API ENDPOINTS
------------------------------------------

1. Add Student  
Method: POST  
Endpoint: /students/add  
Request Body:
{
  "name": "Nani",
  "department": "CSE",
  "email": "nani@example.com",
  "age": 21
}

2. Get All Students  
Method: GET  
Endpoint: /students/all

3. Update Student  
Method: PUT  
Endpoint: /students/update/<id>  
Request Body:
{
  "name": "New Name",
  "department": "CSE",
  "email": "new@example.com",
  "age": 22
}

4. Delete Student  
Method: DELETE  
Endpoint: /students/delete/<id>

------------------------------------------
TESTING USING POSTMAN
------------------------------------------
Use Postman to test all API endpoints:
- POST to add a student  
- GET to fetch all students  
- PUT to update  
- DELETE to remove  

------------------------------------------
FUTURE ENHANCEMENTS
------------------------------------------
- JWT authentication  
- Student attendance module  
- Course management  
- Role-based access  
- Pagination and search filters  

------------------------------------------
AUTHOR
------------------------------------------
Nani Garnipudi  
GitHub: https://github.com/GarnipudiNani
