# 🧑‍💼 Employee Management Web Application

A full-stack web application that allows administrators to securely manage employee records with Create, Read, Update, and Delete (CRUD) operations. Includes user authentication, data validation, and secure storage using Node.js, Express, MongoDB, and JWT.

---

## 🚀 Features

- 🔐 **Authentication** (Login/Register with JWT)
- 🧾 **CRUD operations** on employee data
- ✔️ **Form validation** using `express-validator`
- 🔒 **Password hashing** using bcrypt
- 🧠 Clean modular code structure (MVC pattern)
- 🌐 RESTful API endpoints
- 💡 Frontend with simple HTML + Vanilla JS (no framework required)

---

## 🛠️ Tech Stack

| Layer      | Technology           |
|------------|----------------------|
| Frontend   | HTML, CSS, JavaScript |
| Backend    | Node.js, Express.js   |
| Database   | MongoDB               |
| Auth       | JWT + bcrypt          |
| Validation | express-validator     |

---

## 📁 Project Structure

```
employee-crud-app/
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middlewares/
│   └── server.js
├── frontend/
│   ├── index.html
│   └── app.js
├── .env.example
└── README.md
```

---

## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/employee-crud-app.git
cd employee-crud-app
```

### 2. Install Backend Dependencies

```bash
cd backend
npm install
```

### 3. Create `.env` File

Create a `.env` file inside the `backend` folder with the following:

```
MONGO_URI=your_mongodb_connection_uri
JWT_SECRET=your_super_secret_key
```

> You can use MongoDB Atlas (https://www.mongodb.com/cloud/atlas) to get a free cloud DB.

### 4. Start Backend Server

```bash
node server.js
```

Server runs at `http://localhost:5000`

### 5. Open Frontend

Use any live server extension or directly open the `frontend/index.html` file in your browser.

---

## 🧪 API Endpoints

| Method | Endpoint             | Description              |
|--------|----------------------|--------------------------|
| POST   | `/api/auth/register` | Register a new admin     |
| POST   | `/api/auth/login`    | Login and receive token  |
| GET    | `/api/employees`     | Get all employees        |
| POST   | `/api/employees`     | Add a new employee       |
| PUT    | `/api/employees/:id` | Update employee details  |
| DELETE | `/api/employees/:id` | Delete an employee       |

> All `/employees` routes are protected and require Bearer token in headers.

---

## 🛡️ Security Notes

- Passwords are hashed using `bcrypt` before storing in DB.
- JWT is used to protect employee routes.
- Sensitive fields like `.env` are ignored using `.gitignore`.

---

## 📸 Preview

![Screenshot](https://via.placeholder.com/800x400?text=Employee+CRUD+App+Preview)

---

## 🤝 Author

Made with ❤️ by **Adarsh Raj**  
[LinkedIn](https://www.linkedin.com/in/adarshraj-dev) | [GitHub](https://github.com/YOUR_USERNAME)

---

## 📃 License

This project is licensed under the [MIT License](LICENSE).
