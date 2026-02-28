# Social-Media-App

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![React](https://img.shields.io/badge/React-18.2.0-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-Backend-green.svg)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-brightgreen.svg)
![Socket.IO](https://img.shields.io/badge/Socket.IO-RealTime-lightgrey.svg)

**Social-Media-App** is a robust and dynamic social network platform designed to foster connections, share ideas, and engage communities. It provides a comprehensive suite of features that enable users to create personalized profiles, publish diverse content (text, images, media), interact with peers in real-time, and stay updated through instant notifications—all within a secure and scalable environment.

---

## 🚀 Key Features

- **User Authentication & Profiles:** Secure registration and login using JWT. Users can manage their customized profiles.
- **Content Sharing & Feed:** Publish posts (including image/media support) and scroll through a dynamic feed of content from the community.
- **Real-Time Chat:** Exchange direct messages in real-time, powered by Socket.io for instantaneous communication.
- **Stories System:** Share temporary updates and moments with your network.
- **Instant Notifications:** Receive real-time alerts for interactions, messages, and overall activity.
- **Responsive UI:** A beautifully designed frontend utilizing Material UI (MUI) and Bootstrap for a seamless experience across all devices.

---

## 🛠️ Tech Stack

### Frontend (Client)
- **Framework:** React.js (v18)
- **Styling & UI Components:** Material UI (MUI), Bootstrap, raw CSS
- **Routing:** React Router DOM (v6)
- **State Management & Data Fetching:** Context API, Axios
- **Real-Time Integration:** Socket.io-client
- **Extra Integrations:** Firebase (potential usage for external services/auth/storage)

### Backend (Server)
- **Environment & Framework:** Node.js, Express.js
- **Database & ODM:** MongoDB, Mongoose
- **Authentication & Security:** JWT (JSON Web Tokens), Bcrypt (password hashing), Helmet, CORS
- **Real-Time Engine:** Socket.io
- **File Handling:** Multer, GridFS Stream, Multer-GridFS-Storage

---

## 📂 Project Structure

```text
Social-Media-App/
├── Social App Code/
│   ├── client/              # React Frontend Application
│   │   ├── public/          # Static files
│   │   └── src/             # Source code
│   │       ├── components/  # Reusable UI components
│   │       ├── pages/       # Distinct Page views (Home, Profile, Chat, Landing)
│   │       ├── context/     # Global state context
│   │       ├── RouteProtectors/ # Secured routing logic
│   │       ├── images/      # Application assets
│   │       └── styles/      # Application styling
│   └── server/              # Node.js + Express Backend Application
│       ├── controllers/     # Business logic and request handlers
│       ├── models/          # MongoDB/Mongoose Schemas (Users, Posts, Chats, Stories)
│       ├── routes/          # API route definitions
│       ├── middleware/      # Express middlewares (Auth, File uploads)
│       ├── index.js         # Entry point for backend server
│       └── SocketHandler.js # Centralized real-time socket events management
└── README.md                # This file
```

---

## 💻 Getting Started

### Prerequisites

Ensure you have the following installed on your local machine:
- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [MongoDB](https://www.mongodb.com/) (Local or Atlas URI)

### Installation

1. **Clone the repository:**

   ```bash
   git clone <your-repository-url>
   cd Social-Media-App
   ```

2. **Setup the Backend:**

   Navigate to the server directory and install dependencies:
   ```bash
   cd "Social App Code/server"
   npm install
   ```

   *Create a `.env` file in the server directory based on expected environment variables (e.g., `PORT`, `MONGO_URI`, `JWT_SECRET`).*

   Start the backend server:
   ```bash
   npm start
   ```

3. **Setup the Frontend:**

   Open a new terminal, navigate to the client directory, and install dependencies:
   ```bash
   cd "Social App Code/client"
   npm install
   ```
   Start the React application:
   ```bash
   npm start
   ```

4. **View the Application:**
   Open your browser and navigate to `http://localhost:3000` (or the port specified by React). The backend API will typically run on `http://localhost:5000` (or as configured).

---

## 📄 License

This project is licensed under the MIT License.
