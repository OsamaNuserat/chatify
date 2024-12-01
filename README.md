
# **Chatify**  

A real-time chat application built with NestJS, leveraging WebSocket for fast and reliable communication. This app is designed for seamless integration into larger platforms, supporting role-based interactions and scalable deployment.

---

## **Features**

- 💬 **Real-Time Messaging**: Instant communication with WebSocket integration.
- 🔒 **Secure Authentication**: Role-based access control (e.g., users, coaches).
- 📚 **Modular Design**: Scalable, maintainable, and extensible architecture.
- 🛠️ **Built with NestJS**: Robust framework with TypeScript support.
- ⚡ **Scalable WebSocket Clustering**: Supports high concurrency and distributed systems.
- 🌍 **Localization Ready**: Designed to accommodate global audiences.
  
---

## **Getting Started**

### **Prerequisites**

- Node.js >= 16.x
- npm or yarn
- A database (PostgreSQL, MongoDB, etc., depending on configuration)
- Redis (if enabling clustering)

### **Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/chatify.git
   cd chatify
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and configure the following:
   ```env
   DATABASE_URL=your_database_url
   JWT_SECRET=your_jwt_secret
   PORT=3000
   REDIS_URL=your_redis_url (if clustering)
   ```

4. Run database migrations (if applicable):
   ```bash
   npm run migration:run
   ```

5. Start the application:
   ```bash
   npm run start:dev
   ```

---

## **Usage**

### **Endpoints**
| Method | Endpoint          | Description                  |
|--------|-------------------|------------------------------|
| `POST` | `/auth/login`     | Log in and obtain tokens.    |
| `GET`  | `/chat/messages`  | Fetch chat history.          |
| `POST` | `/chat/message`   | Send a message.              |

### **WebSocket Events**
- **`message`**: Sends/receives chat messages.
- **`typing`**: Indicates user is typing.
- **`status`**: Updates user's online/offline status.

---

## **Development**

### **Folder Structure**
```
src/
├── auth/              # Authentication and roles
├── chat/              # WebSocket and messaging logic
├── common/            # Shared utilities and modules
├── database/          # Database configuration
├── gateway/           # WebSocket gateway
├── user/              # User-related logic and endpoints
└── main.ts            # Application entry point
```

### **Scripts**
- Start in development mode:
  ```bash
  npm run start:dev
  ```
- Run tests:
  ```bash
  npm test
  ```

---

## **Future Enhancements**

- 🔄 **Message Reactions**: Add emojis or reactions to messages.
- 🖼️ **File Sharing**: Support for media uploads.
- 🚀 **Push Notifications**: Notify users of new messages.
- 🔔 **Unread Counts**: Track and display unread messages.

---

## **Contributing**

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Added feature-name"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Create a Pull Request.

---

## **License**

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## **Contact**

For queries, feel free to reach out:

- **Author**: Osama Nuserat  
- **Email**: [osamanuserat3@gmail.com](mailto:osamanuserat3@gmail.com)  
- **GitHub**: [https://github.com/osamanuserat](https://github.com/osamanuserat)  
- **LinkedIn**: [https://linkedin.com/in/osamanuserat](https://linkedin.com/in/osamanuserat)  

---