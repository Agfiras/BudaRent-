# RentCar - Car Rental Application

RentCar is a full-stack web application for car rental services, featuring a modern Angular frontend and a Node.js/Express backend with MongoDB database.

## Features

- **User Authentication System**
  - JWT-based authentication
  - User registration with email verification
  - Password reset functionality
  - Role-based access control (user/admin)
  - User activity tracking

- **Car Management**
  - Comprehensive car listings with detailed information
  - Advanced filtering options (category, price, seats, transmission, fuel type)
  - Search functionality
  - Sorting options (price, year)
  - Pagination for car listings
  - Car image uploads and management

- **Booking System**
  - Car reservation with date selection
  - Booking management (view, cancel)
  - Additional services selection
  - Payment status tracking

- **User Profile Management**
  - Profile viewing and editing
  - Password changing
  - Booking history

- **Admin Dashboard**
  - Vehicle management (add, edit, delete)
  - User management
  - Booking oversight

- **Reviews and Ratings**
  - Car review system
  - Rating calculation

- **Additional Features**
  - API Documentation with Swagger
  - Responsive design
  - Interactive maps for car locations
  - Email notifications

## Technology Stack

### Frontend
- **Framework**: Angular 19.2.x
- **UI Components**: Angular Material 19.2.x
- **Maps**: Google Maps integration
- **Icons**: Font Awesome 6.7.x
- **Notifications**: ngx-toastr 19.0.0
- **HTTP Client**: Angular HttpClient
- **Routing**: Angular Router
- **State Management**: RxJS 7.8.1

### Backend
- **Runtime**: Node.js
- **Framework**: Express 5.1.0
- **Database**: MongoDB 8.13.x (Mongoose ODM)
- **Authentication**: JWT (jsonwebtoken 9.0.2)
- **Password Encryption**: bcryptjs 3.0.2
- **Validation**: express-validator 7.2.1
- **File Upload**: multer 1.4.5
- **Email Service**: nodemailer 6.10.1
- **API Documentation**: Swagger (swagger-jsdoc 6.2.8, swagger-ui-express 5.0.1)
- **Environment Variables**: dotenv 16.5.0

## Installation and Setup

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (v5 or higher)
- Angular CLI (v19.2.x)

### Backend Setup
1. Navigate to the backend directory:
   ```
   cd rentcar-backend
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Create a `.env` file in the root directory with the following variables:
   ```
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/rentcar
   JWT_SECRET=your_jwt_secret
   JWT_EXPIRES_IN=7d
   
   # Email configuration
   SMTP_HOST=your_smtp_host
   SMTP_PORT=your_smtp_port
   SMTP_USER=your_smtp_username
   SMTP_PASS=your_smtp_password
   SMTP_FROM=noreply@rentcar.com
   
   # URLs
   API_URL=http://localhost:5000
   FRONTEND_URL=http://localhost:4200
   ```

4. Start the backend server:
   ```
   node server.js
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```
   cd project-bolt-sb1-eui7ezxp/project
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the development server:
   ```
   npm start
   ```

4. Access the application at `http://localhost:4200`

## API Documentation
The API documentation is available at `http://localhost:5000/api-docs` when the backend server is running.

## Folder Structure

### Backend
- `config/` - Configuration files
- `controllers/` - Request handlers
- `middleware/` - Custom middleware functions
- `models/` - Database models
- `routes/` - API routes
- `uploads/` - Uploaded files storage
- `utils/` - Utility functions

### Frontend
- `src/app/core/` - Core functionality (services, guards, models)
- `src/app/features/` - Feature modules (cars, auth, admin, user)
- `src/app/shared/` - Shared components and utilities
- `src/assets/` - Static assets
