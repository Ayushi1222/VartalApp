# VartalApp 💬

VartalApp is a modern, real-time chat application built with the MERN stack and Socket.io, enabling instant messaging and seamless engagement through live conversations and notifications.

## 🚀 Features

- **Real-time Messaging**: Instant message delivery using Socket.io
- **Live Notifications**: Get notified immediately when new messages arrive
- **User Authentication**: Secure login and registration system
- **Responsive Design**: Optimized for both desktop and mobile devices
- **Online Status**: See who's currently online
- **Message History**: Persistent chat history stored in MongoDB
- **User Profiles**: Customizable user profiles with avatars
- **Typing Indicators**: See when someone is typing
- **Direct Messaging**: One-on-one conversations between users

## 🛠️ Tech Stack

### Frontend
- **React.js** - User interface library
- **Socket.io Client** - Real-time communication
- **CSS3/SCSS** - Styling and responsive design
- **Axios** - HTTP client for API requests

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **Socket.io** - Real-time bidirectional communication
- **JWT** - JSON Web Tokens for authentication

### Database
- **MongoDB** - NoSQL database for storing user data and messages
- **Mongoose** - MongoDB object modeling

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/) (local installation or MongoDB Atlas)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Ayushi1222/VartalApp.git
   cd VartalApp
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

4. **Set up environment variables**
   
   Create a `.env` file in the backend directory with the following variables:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/vartalapp
   JWT_SECRET=your_jwt_secret_key
   NODE_ENV=development
   ```

5. **Start MongoDB**
   Make sure your MongoDB service is running locally or provide a MongoDB Atlas connection string.

## 🚀 Running the Application

### Development Mode

1. **Start the backend server**
   ```bash
   cd backend
   npm run dev
   ```
   The backend server will run on `http://localhost:5000`

2. **Start the frontend development server**
   ```bash
   cd frontend
   npm start
   ```
   The frontend will run on `http://localhost:3000`

### Production Mode

1. **Build the frontend**
   ```bash
   cd frontend
   npm run build
   ```

2. **Start the production server**
   ```bash
   cd backend
   npm start
   ```

## 📁 Project Structure

```
VartalApp/
├── backend/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── socket/
│   ├── utils/
│   ├── server.js
│   └── package.json
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── utils/
│   │   └── App.js
│   └── package.json
└── README.md
```

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Messages
- `GET /api/messages/:userId` - Get conversation with a specific user
- `POST /api/messages` - Send a new message

### Users
- `GET /api/users` - Get all users
- `PUT /api/users/profile` - Update user profile

## 🌐 Socket Events

### Client to Server
- `join_chat` - Join personal chat
- `send_message` - Send a message
- `typing` - User is typing
- `stop_typing` - User stopped typing

### Server to Client
- `receive_message` - Receive a new message
- `user_online` - User came online
- `user_offline` - User went offline
- `typing_indicator` - Show typing indicator
- `online_users` - List of online users

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👩‍💻 Author

**Ayushi Katroliya** - [Ayushi1222](https://github.com/Ayushi1222)

## 🙏 Acknowledgments

- Socket.io documentation and community
- MERN stack tutorials and resources
- All contributors and testers

## 📞 Support

If you have any questions or need help, please open an issue on GitHub or contact the maintainer.

---

**Happy Chatting! 🎉**
