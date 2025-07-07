# 🚀 Habit Quest: The Gamified Habit Tracker

Welcome to Habit Quest, a full-stack web application designed to turn building positive habits into an exciting adventure. Track your daily goals, earn XP, complete challenges, and level up as you conquer your personal quests!

This project is built with a modern MERN-like stack (MongoDB, Express, React, Node.js) and features a clean, scalable architecture.

![Habit Quest App Screenshot](https://via.placeholder.com/800x450.png?text=Add+A+Screenshot+Of+Your+App+Here!)
*(Replace the placeholder above with a real screenshot of your application's dashboard)*

---

## ✨ Features

*   **Habit Creation & Management**: Create custom habits with flexible scheduling options:
    *   Daily
    *   Specific days of the week (e.g., Mon, Wed, Fri)
    *   A set number of times per week (e.g., 3x a week)
    *   Every 'N' days (e.g., every 3 days)
*   **Interactive Daily Dashboard**: View all habits due for the day and mark them as complete with a single click.
*   **Gamification System**:
    *   **XP & Levels**: Earn experience points (XP) for every habit completion and watch yourself level up.
    *   **Streaks**: Build and maintain completion streaks for each habit.
    *   **Challenges & Quests**: Take on a variety of active challenges (e.g., "Maintain a 7-day streak," "Reach Level 10").
    *   **Badges**: Earn unique badges for completing special milestones and challenges.
*   **User Profiles**:
    *   View your overall stats, including level, total XP, and all earned badges.
    *   Upload and update your profile picture.
*   **Secure Authentication**: Secure user registration and login system using JSON Web Tokens (JWT).
*   **Theming**: Switch between a sleek Light and Dark mode.

---

## 🛠️ Tech Stack

This project is a monorepo containing both the frontend and backend code.

### Backend

*   **Framework**: [Node.js](https://nodejs.org/) with [Express.js](https://expressjs.com/)
*   **Database**: [MongoDB](https://www.mongodb.com/) with [Mongoose](https://mongoosejs.com/) for object data modeling.
*   **Authentication**: [JSON Web Tokens (JWT)](https://jwt.io/)
*   **File Uploads**: [Multer](https://github.com/expressjs/multer) for handling profile picture uploads.
*   **Security**: `bcryptjs` for password hashing, `cors` for resource sharing.

### Frontend

*   **Framework**: [React](https://reactjs.org/)
*   **Build Tool**: [Vite](https://vitejs.dev/) for a blazing-fast development experience.
*   **Routing**: [React Router](https://reactrouter.com/) for client-side routing.
*   **State Management**: React Context API for managing global auth and theme state.
*   **API Communication**: [Axios](https://axios-http.com/) with interceptors for streamlined, authenticated API calls.
*   **UI/Styling**:
    *   Plain CSS with modern features (Flexbox, Grid, CSS Variables).
    *   `react-toastify` for notifications.

---

## ⚙️ Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

*   [Node.js](https://nodejs.org/en/download/) (v16 or later recommended)
*   [MongoDB](https://www.mongodb.com/try/download/community) installed and running locally, or a MongoDB Atlas connection string.
*   `npm` (usually comes with Node.js)

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/gamified-habit-tracker.git
    cd gamified-habit-tracker
    ```

2.  **Setup the Backend:**
    *   Navigate to the backend directory:
        ```bash
        cd backend
        ```
    *   Install dependencies:
        ```bash
        npm install
        ```
    *   Create a `.env` file in the `backend` directory and add your configuration:
        ```env
        PORT=5001
        MONGO_URI=your_mongodb_connection_string
        JWT_SECRET=your_super_secret_jwt_key
        ```
    *   (Optional) Seed the database with sample challenges and data. This is highly recommended for first-time setup.
        ```bash
        node seed.js
        ```

3.  **Setup the Frontend:**
    *   Navigate to the frontend directory from the root folder:
        ```bash
        cd frontend
        ```
    *   Install dependencies:
        ```bash
        npm install
        ```
    *   Create a `.env` file in the `frontend` directory to point to your backend API:
        ```env
        VITE_API_URL=http://localhost:5001/api
        ```

### Running the Application

You will need to run the backend and frontend servers in two separate terminal windows.

1.  **Start the Backend Server:**
    *   In the `backend` directory:
        ```bash
        npm start
        ```
    *   The API should now be running on `http://localhost:5001`.

2.  **Start the Frontend Development Server:**
    *   In the `frontend` directory:
        ```bash
        npm run dev
        ```
    *   The React application should now be running and accessible at `http://localhost:5173` (or another port specified by Vite).

---
