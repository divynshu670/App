🎬 Movie Review Platform

A full-stack web application where users can browse movies, read/write reviews, give star ratings, and manage their personal watchlist.
This project is built as part of a Full Stack Developer assignment, using React for the frontend and Node.js + Express + MongoDB for the backend.

🚀 Features

Responsive UI (mobile + desktop)

Browse featured and trending movies

Search and filter by genre, year, and rating

Movie detail pages with cast, trailers, and reviews

Star rating and text review submission

User profile with review history

Add/remove movies from personal watchlist

User authentication (register/login)

Average ratings stored and displayed

Error handling and loading states throughout

🏗 Tech Stack

Frontend: React, React Router, Redux/React Context
Backend: Node.js, Express
Database: MongoDB (can also support MySQL)
Authentication: JSON Web Token
Optional API: TMDB for fetching posters and metadata

⚙️ Setup Instructions
Clone Repository
git clone https://github.com/your-username/movie-review-platform.git
cd movie-review-platform

⚡ Backend Setup
cd server
npm install


Create .env file in server/:

PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret

npm run dev

⚛️ Frontend Setup
cd client
npm install


Create .env file in client/:

REACT_APP_API_URL=http://localhost:5000

npm start

🗃 Database Schema

Movies

title, genre, releaseYear, director, cast, synopsis, posterUrl, averageRating


Users

username, email, password(hashed), profilePicture, joinDate


Reviews

userId, movieId, rating(1-5), reviewText, timestamp


Watchlist

userId, movieId, dateAdded

📡 API Endpoints
Method	Endpoint	Description
GET	/movies	Get all movies (with pagination/filter)
GET	/movies/:id	Get specific movie with reviews
POST	/movies	Add new movie (admin only)
GET	/movies/:id/reviews	Get reviews for a movie
POST	/movies/:id/reviews	Submit a new review
GET	/users/:id	Get user profile and review history
PUT	/users/:id	Update user profile
GET	/users/:id/watchlist	Get user watchlist
POST	/users/:id/watchlist	Add to watchlist
DELETE	/users/:id/watchlist/:movieId	Remove from watchlist
📌 Notes

Input validation on frontend + backend

Error boundaries implemented in React

JWT-based secure authentication

All sensitive config in .env

Rate limiting (optional) with express-rate-limit

Responsive layout for all major screen sizes

🌐 Optional (If Implemented)

Movie recommendation system

Social features (follow users, see their reviews)

Admin dashboard

Real-time notifications

Live Demo: https://your-live-demo.com

📄 License

MIT License — Submitted as part of a Full Stack Developer assignment.
