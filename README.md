# 🚀 Realtime Chat Application

Welcome to the Realtime Chat Application! This project is a modern, full-stack web application that allows users to communicate with each other in real time. Built with a robust backend and a dynamic frontend, it provides a seamless and engaging chat experience.

## ✨ Features

- **Realtime Messaging:** Instantly send and receive messages with the power of WebSockets.
- **User Authentication:** Secure user registration and login using JSON Web Tokens (JWT).
- **Private and Group Chats:** Create private conversations or join group chats to communicate with multiple users.
- **User Presence:** See which users are currently online and available to chat.
- **Message History:** Never lose a conversation! All messages are stored and can be retrieved later.
- **Typing Indicators:** See when others are typing for a more natural conversation flow.
- **Responsive Design:** A clean, intuitive, and mobile-friendly user interface.
- **Profile Management:** Users can update their profiles and avatars.

## 🛠️ Technologies Used

### Backend

- **Node.js & Express.js:** A powerful and flexible framework for building the server-side logic.
- **MongoDB:** A NoSQL database for storing user data, messages, and chat information.
- **Mongoose:** An elegant MongoDB object modeling tool for Node.js.
- **Socket.IO:** The engine for real-time, bidirectional, event-based communication.
- **JWT (JSON Web Tokens):** For secure and stateless user authentication.
- **Bcrypt:** Hashing passwords to ensure security.

### Frontend

- **React:** A declarative and component-based JavaScript library for building user interfaces.
- **React Router:** For handling client-side routing.
- **Axios:** A promise-based HTTP client for making API requests.
- **Socket.IO Client:** The client-side library for connecting to the Socket.IO server.
- **Tailwind CSS:** A utility-first CSS framework for rapid and custom UI development.

## 💻 Getting Started

### Prerequisites

- Node.js installed on your machine.
- MongoDB installed and running or a cloud-based MongoDB Atlas account.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```

2.  **Install backend dependencies:**
    ```bash
    cd backend
    npm install
    ```

3.  **Install frontend dependencies:**
    ```bash
    cd ../frontend
    npm install
    ```

### Configuration

1.  **Backend:**
    - Create a `.env` file in the `backend` directory.
    - Add your environment variables:
      ```env
      PORT=5000
      MONGO_URI=your_mongodb_connection_string
      JWT_SECRET=a_very_secret_key
      ```

2.  **Frontend:**
    - The frontend is configured to connect to the backend at `http://localhost:5000` by default. If you change the backend port, update the `src/config.js` or similar file.

### Running the Application

1.  **Start the backend server:**
    ```bash
    cd backend
    npm start
    ```

2.  **Start the frontend development server:**
    ```bash
    cd ../frontend
    npm start
    ```

The application should now be running! Open your browser and navigate to `http://localhost:3000` to see it in action.

## 📄 API Endpoints

| Method | Endpoint                    | Description                           |
| :----- | :-------------------------- | :------------------------------------ |
| `POST` | `/api/auth/register`        | Register a new user                   |
| `POST` | `/api/auth/login`           | Authenticate and log in a user        |
| `GET`  | `/api/users/search?query=`  | Search for users                      |
| `GET`  | `/api/chats`                | Get all chats for the authenticated user |
| `POST` | `/api/chats`                | Create a new chat                     |
| `GET`  | `/api/messages/:chatId`     | Get all messages for a specific chat  |
| `POST` | `/api/messages`             | Send a new message                    |

## 🤝 Contribution

Contributions are welcome! If you have a bug to report, a feature to suggest, or a pull request to submit, please feel free to do so.

1.  Fork the repository.
2.  Create a new branch: `git checkout -b feature/your-feature-name`.
3.  Make your changes and commit them: `git commit -m 'feat: Add new feature'`.
4.  Push to the branch: `git push origin feature/your-feature-name`.
5.  Create a pull request.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by Anurag Mishra
