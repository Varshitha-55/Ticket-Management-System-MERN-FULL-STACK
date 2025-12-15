# Support Desk

Ticket management system with MERN stack

• MERN stack project for create and manage tickets.

• Features: JWT based login system. User can perform CRUD operations on tickets.

• Features: Redux-toolkit for state management, Responsive UI.


**Support Desk** is a full-stack **MERN (MongoDB, Express, React, Node.js)** ticket management system that allows users to create and manage support tickets with authentication, CRUD operations, and responsive UI.


## 📌 Features

✅ User authentication using **JWT tokens**
✅ Create, read, update, delete **tickets**
✅ **Redux Toolkit** for state management
✅ Responsive UI built with **React.js**
✅ Backend APIs with **Node.js + Express.js**
✅ MongoDB for data storage
✅ Clean folder structure for frontend & backend separation ([GitHub][1])

---

## 🧠 Project Flow

flowchart TD
    A[User] -->|Login / Register| B[React Frontend]
    B -->|Auth Request| C[Express API]
    C -->|Generate JWT| D[MongoDB]
    B -->|CRUD Tickets| C
    C --> D
    C -->|Send Response| B


1. **User interacts** with the React frontend.
2. Frontend calls **backend APIs** for login/signup.
3. Backend verifies credentials, issues **JWT** tokens.
4. Authenticated users interact with ticket APIs (CRUD).
5. Data is stored in **MongoDB**.

---

## 📁 Repository Structure

```
supportdesk/
├── backend/                     # Node + Express backend
│   ├── controllers/            # Business logic
│   ├── models/                 # Mongoose schemas
│   ├── routes/                 # API endpoints
│   ├── middleware/             # Auth middleware
│   └── server.js               # App entrypoint
├── frontend/                   # React application
│   ├── src/
│   │   ├── components/         # UI components
│   │   ├── pages/              # Route pages
│   │   ├── redux/              # Redux slices & store
│   │   ├── services/           # API functions
│   │   └── App.js
│   ├── public/
│   └── package.json
├── .env                        # Environment variables
├── .gitignore
├── README.md
└── package.json
```

---

## 🛠 Tech Stack

| Layer      | Technology              |
| ---------- | ----------------------- |
| Frontend   | React.js, Redux Toolkit |
| Backend    | Node.js, Express.js     |
| Database   | MongoDB                 |
| Auth       | JWT Tokens              |
| Deployment | GitHub Pages (frontend) |
| State Mgmt | Redux Toolkit           |

---
### 🚀 Getting Started

### Prerequisites

Install the following:

* Node.js (v14+)
* npm / yarn
* MongoDB (Atlas or local)


### Backend Setup

1. Go to the backend folder:

```bash
cd backend
```

2. Install dependencies:

```bash
npm install
```

3. Create `.env` file (example):

```
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
```

4. Start backend:

```bash
npm start
```

---

### Frontend Setup

1. Go to frontend folder:

```bash
cd frontend
```

2. Install dependencies:

```bash
npm install
```

3. Run the app:

```bash
npm start
```

Your app should now be running at `http://localhost:3000`

---

## 🧪 Usage

1. Register a new user
2. Login using email/password
3. Create a support ticket
4. View and manage tickets
5. Update or delete your tickets

---

## 🎯 Future Enhancements

✔ Add role-based access (admin vs user)
✔ Add ticket comments & attachments
✔ Add email notifications
✔ Improve UI with better UX/confetti ✨

---

## 📫 Contact

Created by
Namburu.Sri Varshitha

[2]: https://pranavmappoli.github.io/supportdesk/?utm_source=chatgpt.com "Support Desk - Pranav M"
[3]: https://github.com/pranavmappoli?utm_source=chatgpt.com "Pranav M pranavmappoli"
