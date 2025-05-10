
# Growth 🚀

**Growth** is a career counseling platform built using the MERN stack (MongoDB, Express.js, React, Node.js). It connects users with experienced mentors to provide guidance, support, and resources for career development. The platform allows users to find mentors, book sessions, share goals, and track their career progress. Mentors can manage their profiles, provide resources, and engage with mentees.

---

## 🌟 Features

- 👥 **Mentor-User Matching**: Connects users with mentors based on expertise and goals.
- 📅 **Booking & Scheduling**: Allows mentees to book counseling sessions.
- 📝 **Goal Tracking**: Users can set short-term and long-term goals.
- 🗂️ **Resources Sharing**: Mentors can share articles, videos, and learning materials.
- ⭐ **Feedback & Ratings**: Users can provide feedback and rate mentors.
- 🔐 **Authentication**: Secure user and mentor login/registration system.

---

## 🛠️ Tech Stack

- **Frontend**: React + Vite + Tailwind CSS (if used)
- **Backend**: Node.js + Express.js
- **Database**: MongoDB
- **Other**: JWT for authentication, Mongoose for MongoDB interactions

---

## 🚀 Getting Started

Follow these steps to run the project locally.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/growth.git
cd growth
````

### 2️⃣ Set Up the Backend

1. Go to the backend directory:

   ```bash
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the `backend` directory and add the following:

   ```env
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```

4. Start the backend server:

   ```bash
   npm start
   ```

   The backend should now be running at `http://localhost:5000`.

---

### 3️⃣ Set Up the Frontend

1. Open a new terminal window and navigate to the frontend directory:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Run the React app using Vite:

   ```bash
   npm run dev
   ```

   The frontend should now be running at `http://localhost:5173`.

---

## 🖼️ Project Structure

```
growth/
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── .env
│   └── server.js
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── utils/
│   │   └── App.jsx
│   └── vite.config.js
├── README.md
└── package.json
```

---

## 📬 API Endpoints

Some example endpoints:

* `POST /api/auth/register` - Register a new user or mentor
* `POST /api/auth/login` - Login
* `GET /api/mentors` - Get list of mentors
* `POST /api/goals` - Add a new goal
* `GET /api/resources` - Get shared resources

---

## ✅ Requirements

* Node.js >= 16.x
* MongoDB (local or cloud e.g., MongoDB Atlas)

---

## 🙌 Contributing

1. Fork the project.
2. Create your feature branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m 'Add YourFeature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a pull request.

