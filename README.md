# 🛠️ RESTful API with Express & Mongoose

This project is a simple RESTful API built using **Node.js**, **Express**, and **Mongoose**. It allows basic CRUD operations on a `User` collection.

---

## 📁 Folder Structure

```
project/
├── config/
│   ├── db.js
│   └── .env (you will have to create yours of course :) )
├── models/
│   └── User.js
├── server.js
├── .gitignore
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/ryadbahi/11-REST-API.git
cd 11-REST-API
```

### 2. Install dependencies
```bash
npm install
```

### 3. Add environment variables

Create a `.env` file inside the `config/` folder:

```env
MONGO_URI=your_mongodb_connection_string
PORT=5000
```

### 4. Start the server
```bash
node server.js
```

Server will run at:  
```
http://localhost:5000
```

---

## 🧪 API Endpoints

### 📥 POST - Add a New User

- **URL:** `/users`
- **Method:** `POST`
- **Headers:** `Content-Type: application/json`
- **Body Example:**
```json
{
  "name": "Ryad",
  "email": "ryad@example.com",
  "age": 25
}
```

![post](https://github.com/user-attachments/assets/a5111770-089a-4dd8-99f2-4d32ce4aa85b)


---

### 📤 GET - Get All Users

- **URL:** `/users`
- **Method:** `GET`

![get](https://github.com/user-attachments/assets/c86af441-40b2-4647-903d-0c385755949e)


---

### 🔁 PUT - Update User by ID

- **URL:** `/users/:id`
- **Method:** `PUT`
- **Headers:** `Content-Type: application/json`
- **Body Example:**
```json
{
  "age": 27
}
```

![put](https://github.com/user-attachments/assets/f963c8bb-307c-4257-9dc0-1df06e9600f9)


---

### ❌ DELETE - Remove User by ID

- **URL:** `/users/:id`
- **Method:** `DELETE`

![delete](https://github.com/user-attachments/assets/00e19916-bc71-48b5-9606-531f890c3c97)


---

## 📦 Tech Stack

- Node.js
- Express
- MongoDB Atlas
- Mongoose
- dotenv
