User Management API (Node.js + Express + MongoDB)

Description:
This is a simple REST API built using Node.js, Express, and MongoDB (Mongoose).
It allows users to perform basic CRUD operations such as register, view, update, and delete users.

Features:

Register new users

Get all users

Update user by username

Delete user by username

Uses environment variables with dotenv

Tech Stack:

Node.js

Express.js

MongoDB

Mongoose

dotenv

Project Structure:

backend/
│
├── node_modules/
├── .env
├── index.js
├── package.json
└── README.txt

Installation Steps:

Clone the repository:
git clone <your-repository-url>

Navigate into the project folder:
cd backend

Install dependencies:
npm install

Environment Variables:

Create a .env file in the root folder and add:

PORT=5000
MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/testdb

Replace:

username with your MongoDB Atlas username

password with your MongoDB Atlas password

cluster.mongodb.net with your cluster URL

Run the Server:

node index.js

If successful, you will see:
MongoDB connected
Server is running on port 5000

API Endpoints:

Register User
Method: POST
URL: http://localhost:5000/register

Body (JSON):
{
"username": "ansh",
"email": "ansh@gmail.com
",
"password": "123456"
}

Get All Users
Method: GET
URL: http://localhost:5000/users

Update User
Method: PUT
URL: http://localhost:5000/users/:username

Body (JSON):
{
"email": "newmail@gmail.com
",
"password": "newpassword"
}

Delete User
Method: DELETE
URL: http://localhost:5000/users/:username

Testing Tools:

Postman

Thunder Client (VS Code Extension)

Future Improvements:

Password hashing using bcrypt

Login API

JWT Authentication

Input validation

Better error handling
