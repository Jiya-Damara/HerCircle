# 🌸 HerCircle

HerCircle is a secure, inclusive social support web application designed to empower women. Built using the MERN stack, it provides a safe, stigma-free platform where users can share experiences, seek advice, and access AI-powered guidance.

---

## 🎯 Project Goals

- **Safe Space:** Foster a supportive environment for women to discuss sensitive topics like reproductive health and mental wellness without fear of judgment.
- **Privacy First:** Enable anonymous interactions so users can control what they share.
- **AI-Powered Support:** Provide instant, reliable guidance through an integrated AI chatbot.
- **Community Engagement:** Encourage meaningful discussions through posts, likes, comments, and topic-based feeds.

---

## ✨ Key Features

- 🔐 **Secure Authentication**
  - User sign-up and login using JWT
  - Password hashing with bcrypt

- 🕵️‍♀️ **Anonymous Posting**
  - Toggle to hide identity on posts

- 🏷️ **Topic-Based Feed**
  - Categories like PCOS, Menstrual Health, Mental Health, Nutrition, Fitness, etc.

- 💬 **Community Interaction**
  - Like, comment, and engage with posts

- 🤖 **AI Chatbot (Gemini)**
  - Private AI assistant for guidance
  - Chat history saved per user

- 📱 **Responsive UI**
  - Clean and modern interface using React.js
  - Works across mobile and desktop

---

## 🛠️ Tech Stack

### Frontend
- React.js

### Backend
- Node.js
- Express.js
- JSON Web Tokens (JWT)
- Bcrypt.js

### Database
- MongoDB
- Mongoose ODM

### AI Integration
- Google Gemini API

---

## 📐 System Design Overview

The application follows a **Client-Server Architecture**:

1. **Client (Frontend)**
   - Handles UI rendering, routing, and state management
   - Manages user sessions and feed updates

2. **API Layer (Backend)**
   - Handles authentication and authorization (JWT)
   - Processes CRUD operations for posts and comments
   - Acts as a secure proxy for Gemini API

3. **Data Layer (Database)**
   - Stores users, posts, comments, and chat history
   - Uses relational references (User → Posts → Comments)

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- MongoDB (local or Atlas)
- Google Gemini API Key

---

### 📦 Installation

#### 1. Clone the repository

```bash
git clone https://github.com/yourusername/HerCircle.git
cd HerCircle


#### 2. Setup Backend

```bash
cd backend
npm install
```

Create a `.env` file in the backend directory:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
GEMINI_API_KEY=your_gemini_api_key
```

Run the backend server:

```bash
npm run dev
```

#### 3. Setup Frontend

```bash
cd ../frontend
npm install
npm start
```

## 📡 Core API Endpoints

### 🔐 Auth
- POST `/api/auth/register` → Register new user
- POST `/api/auth/login` → Login & receive JWT

### 📝 Posts
- GET `/api/posts` → Fetch posts (with topic filters)
- POST `/api/posts` → Create post (supports anonymous flag)

### 🤖 Chatbot
- POST `/api/chat` → Send prompt to Gemini
- GET `/api/chat/history` → Fetch chat history

## 📱 UI Preview
(Will add after project completion)

## 📅 Timeline & Milestones

- [x] 23rd March: Project name updated with repository link in the sheet
- [x] 26th March: Requirement and Design document uploaded to GitHub repository
- [x] 26th March: Completed README.md with project description, goals, specifications, and design
- [ ] 🎯 9th April (Final Deadline): Project to be completed with all deliverables checked into GitHub repository


## 💡 Future Enhancements

- User profile customization
- Bookmark / saved posts
- Voice-based AI interaction
- Moderation & reporting system
- Notifications system

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.

## 📄 License

This project is licensed under the MIT License.

## 💖 Acknowledgement

HerCircle is built with the vision of creating a safe digital space for women to express, heal, and grow together.