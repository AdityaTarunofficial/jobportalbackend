# ⚙️ Backend

### Overview
The **backend** of the Job Portal is built using **Node.js**, **Express**, and **MongoDB**. It provides RESTful APIs for managing users, jobs, and authentication, serving as the core for all business logic and data management.

### 🛠️ Key Technologies
- **Node.js**: Asynchronous JavaScript runtime to handle server operations efficiently.
- **Express.js**: Lightweight framework to build robust APIs.
- **MongoDB**: NoSQL database for flexible data storage.
- **Mongoose**: ODM for MongoDB to structure and manage data.
- **JWT (JSON Web Token)**: For user authentication and authorization.
- **Bcrypt.js**: For securely hashing passwords.

### Features
- **Authentication & Authorization**: 
  - User registration and login using JWT tokens.
  - Password hashing for security with Bcrypt.js.

- **Job Management**:
  - CRUD operations for job listings (Create, Read, Update, Delete).
  - Endpoint for users to apply for jobs.
  
- **Profile Management**: 
  - APIs to get and update user profiles.

- **Applied Jobs Tracking**: 
  - Users can fetch the jobs they've applied to.
  - Ability to reject job applications.

### Endpoints

#### User Routes:
- `POST /api/users/register` - Register a new user.
- `POST /api/users/login` - Log in a user.
- `POST /api/users/logout` - Log out the current user.
  
#### Job Routes:
- `GET /api/jobs` - Fetch all jobs.
- `POST /api/jobs` - Create a new job (Admin).
- `PUT /api/jobs/:id` - Update an existing job (Admin).
- `DELETE /api/jobs/:id` - Delete a job (Admin).
- `POST /api/jobs/:id/apply` - Apply for a job.
- `POST /api/jobs/:id/reject` - Reject an applied job.

### Installation & Setup

1. **Clone the backend repository:**
   ```bash
   git clone https://github.com/yourusername/job-portal-backend.git
   cd job-portal-backend
