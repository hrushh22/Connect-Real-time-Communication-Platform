# MERN Stack Chat App

A full-stack real-time chat application built with MongoDB, Express.js, React.js, Node.js, and Socket.io for instant messaging functionality.

## 🚀 Features

- **Real-time Messaging**: Instant message delivery using Socket.io
- **User Authentication**: Secure user registration and login system
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Online Status**: See who's currently online
- **Message History**: Persistent chat history stored in MongoDB
- **Multiple Chat Rooms**: Join different chat rooms or create private conversations
- **Typing Indicators**: See when other users are typing
- **Emoji Support**: Express yourself with emoji reactions
- **File Sharing**: Share images and documents (if implemented)
- **User Profiles**: Customize your profile with avatars and status messages

## 🛠️ Tech Stack

**Frontend:**
- React.js
- Socket.io-client
- CSS3 / Styled Components
- Axios for API calls

**Backend:**
- Node.js
- Express.js
- Socket.io
- MongoDB with Mongoose
- JWT for authentication
- bcryptjs for password hashing

## 📋 Prerequisites

Before running this project, make sure you have the following installed:
- Node.js (v14.0.0 or later)
- npm or yarn
- MongoDB (local installation or MongoDB Atlas)

## ⚡ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/mern-chat-app.git
   cd mern-chat-app
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Environment Variables**
   
   Create a `.env` file in the backend directory and add the following:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/chatapp
   JWT_SECRET=your_jwt_secret_key_here
   NODE_ENV=development
   ```

   For MongoDB Atlas (cloud database):
   ```env
   MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/chatapp
   ```

5. **Start MongoDB**
   - If using local MongoDB: Start your MongoDB service
   - If using MongoDB Atlas: Ensure your connection string is correct in the `.env` file

## 🚀 Running the Application

1. **Start the backend server**
   ```bash
   cd backend
   npm run dev
   ```
   Backend will run on `http://localhost:5000`

2. **Start the frontend application**
   ```bash
   cd frontend
   npm start
   ```
   Frontend will run on `http://localhost:3000`

3. **Visit the application**
   Open your browser and go to `http://localhost:3000`


## 🔧 Available Scripts

**Backend:**
- `npm start` - Start the server in production mode
- `npm run dev` - Start the server with nodemon for development
- `npm run build` - Build the application for production

**Frontend:**
- `npm start` - Start the React development server
- `npm run build` - Build the React app for production
- `npm test` - Run the test suite

## 🌐 API Endpoints

### Authentication
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/auth/me` - Get current user info

### Messages
- `GET /api/messages/:conversationId` - Get messages for a conversation
- `POST /api/messages` - Send a new message

### Users
- `GET /api/users` - Get all users
- `PUT /api/users/profile` - Update user profile

## 🚀 Deployment

### Backend Deployment (Heroku)
1. Install Heroku CLI
2. Login to Heroku: `heroku login`
3. Create Heroku app: `heroku create your-app-name`
4. Set environment variables on Heroku
5. Deploy: `git push heroku main`

### Frontend Deployment (Netlify/Vercel)
1. Build the React app: `npm run build`
2. Deploy the `build` folder to your preferred hosting service
3. Update API endpoints to point to your deployed backend


---

⭐ If you found this project helpful, please give it a star!
