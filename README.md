💼 Job Portal Application
Overview
The Job Portal Application is a full-stack web platform designed to connect job seekers with employers. The app is divided into two parts:

Frontend: A sleek React-based user interface for interacting with the application.
Backend: A Node.js-powered server that handles data storage, authentication, and APIs.


⚙️ Backend
Overview
The backend of the Job Portal is built using Node.js, Express, and MongoDB. It provides RESTful APIs for managing users, jobs, and authentication, serving as the core for all business logic and data management.

🛠️ Key Technologies
Node.js: Asynchronous JavaScript runtime to handle server operations efficiently.
Express.js: Lightweight framework for building RESTful APIs.
MongoDB: A NoSQL database used for storing job listings, user profiles, and applications.
JWT (JSON Web Tokens): Secures the authentication flow, ensuring protected routes.
Mongoose: MongoDB object modeling for schema definition and database interaction.
📂 Folder Structure:
graphql
backend/
├── controllers/   # Contains logic for user and job actions
├── models/        # Mongoose models for User, Job, etc.
├── routes/        # Defines the API routes
├── middleware/    # Authentication middleware (JWT)
├── server.js      # Main server file
🚀 Getting Started with the Backend
Prerequisites:
Node.js installed on your machine.
A MongoDB database (local or cloud).
Steps:
Install Dependencies

bash
cd backend
npm install
Environment Variables Create a .env file in the backend directory:

env
MONGODB_URI=<Your MongoDB Connection URI>
JWT_SECRET=<Your Secret Key for JWT>
Run the Server

bash
npm start
API Documentation The backend exposes REST APIs for managing jobs, user profiles, and authentication. Refer to the /api routes for further details.
