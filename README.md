# Online Learning Platform

This is a full-stack web application that allows users to register, log in, create and enroll in courses, add lessons, and track their learning progress.

## Features

- **User Registration & Authentication:** Secure registration and login using JWT tokens.
- **Course Management:** Create, view, and list courses with multiple lessons.
- **Lesson Management:** Add lessons (title and content) to each course.
- **Enrollment:** Users can enroll in courses and see their enrolled courses.
- **Progress Tracking:** Mark lessons as complete and track progress.
- **Responsive UI:** Clean and modern interface with custom CSS.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript (vanilla)
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (via Mongoose)
- **Authentication:** JWT (JSON Web Tokens)

## Folder Structure

```
course/
│
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── server.js
│
├── css/
│   └── styles.css
│
├── js/
│   ├── auth.js
│   ├── dashboard.js
│   ├── create-course.js
│   └── course.js
│
├── create-course.html
├── dashboard.html
├── course.html
├── login.html
├── register.html
└── index.html
```

## Getting Started

### Prerequisites

- Node.js and npm installed
- MongoDB running locally

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. **Install backend dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Set up environment variables:**
   - Create a `.env` file in the `backend` folder with:
     ```
     MONGO_URI=mongodb://localhost:27017/onlinelearning
     JWT_SECRET=your_jwt_secret
     PORT=5000
     ```

4. **Start the backend server:**
   ```bash
   node server.js
   ```
   or (for auto-reload)
   ```bash
   npx nodemon server.js
   ```

5. **Open the frontend:**
   - Open `index.html` or `dashboard.html` in your browser, or visit `http://localhost:5000/dashboard.html` if served by Express.

## Usage

- Register a new user or log in.
- Create a new course and add lessons.
- Enroll in available courses.
- Mark lessons as complete to track your progress.

## Troubleshooting

- Ensure MongoDB is running locally.
- Check the browser console and backend terminal for errors.
- If lessons do not appear, make sure you are adding them before submitting the course.

## License

This project is for educational purposes.
