# Thoughts Backend API
​
## Description
​
Thoughts Backend API is a RESTful API built with Node.js, Express, and MongoDB. It powers a blogging system, allowing users to register, login, create, read, update, and delete blog posts. The API also supports adding and deleting comments on posts and uploading profile pictures and post thumbnails.
​
## Technologies Used
​
* Node.js
* Express
* MongoDB
* Mongoose
* bcrypt
* jsonwebtoken
* dotenv
* cors
* multer
​
## Setup
​
### Prerequisites
​
*** Node**.js (>= 18.x)
*** npm **(>= 9.x)
*** MongoDB**. account and cluster
​
##  **Project Structure**

```
📂 thoughts_be/
├── 📄 .env                # Environment variables
├── 📄 app.js              # Main server file
├── 📂 config/             # Configuration files
│   └── dbConnection.js # MongoDB connection setup
├── 📂 controllers/        # API controllers
│   ├── user.controller.js   # Authentication User logic
│   └── post.controller.js   # Blog post logic
├── 📂 models/             # Mongoose models
│   ├── user.controller.js
│   └── post.model.js
├── 📂 routes/             # API routes
└── 📂 middleware/         # Middleware (fileUploads., authentication)
└── 📂 utils/              # GenerateToken
```


### Installation
​
### **1.  Clone the repository:**
    ```bash
    git clone  https://github.com/amr-ibrahim7/thoughts_be
    cd thoughts_be
    ```
### **2. Install dependencies:**
    ```bash
    npm install
    ```
### **3. Create a `.env` file in the root directory and configure your environment variables:**
    ```bash
    DB_USER=<your_mongodb_user>
    DB_PASS=<your_mongodb_password>
    DB_CLUSTER=<your_mongodb_cluster_url>
    DB_NAME=<your_mongodb_database_name>
    ACCESS_JWT_KEY=<your_access_jwt_key>
    PORT=5000 
    ```
### 4.  Start the development server:
    ```bash
    npm run dev
    ```
###  The server will start at `http://localhost:3000` (or the port specified in your `.env` file).
​
## API Endpoints
## Postman Collection

You can import 
[thoughtsSystem](https://restless-meadow-459784.postman.co/workspace/Team-Workspace~e795dc71-82dd-4b38-897d-9ef8e68c5f41/collection/39966075-94c02203-1dcf-42f0-8a9b-5721443da551?action=share&creator=39966075)
into Postman to easily test all the API endpoints. The endpoints are organized into separate folders for easier navigation: `users`, `posts`, 
​

​
​
## Authentication
​
Most of the protected routes require an access token to be passed in the `Authorization` header as a Bearer token. You will receive this token upon successful registration or login.
​
Example Header:
Thoughts Backend API
Description
Thoughts Backend API is a RESTful API built with Node.js, Express, and MongoDB. It powers a blogging system, allowing users to register, login, create, read, update, and delete blog posts. The API also supports adding and deleting comments on posts and uploading profile pictures and post thumbnails.


