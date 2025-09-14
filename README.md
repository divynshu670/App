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

npm run dev

⚛️ Frontend Setup
cd client
npm install


Create .env file in client


npm start

All sensitive config in .env

Rate limiting (optional) with express-rate-limit

Responsive layout for all major screen sizes

