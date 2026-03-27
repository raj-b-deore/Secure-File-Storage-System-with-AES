# 🔐 SafeVault

### A Secure File Protection & Sharing System

SafeVault is a modern file security platform that enables users to safely upload, encrypt, store, and access files using strong cryptographic techniques. Each file is protected with a unique access key, ensuring only authorized users can retrieve it.

---

## 🚀 Key Highlights

- 🔑 Secure Authentication System – User registration and login with protected sessions  
- 🔒 Advanced Encryption – Files are encrypted using AES-256 algorithm  
- 📥 Controlled Decryption – Files can only be accessed with a valid secret key  
- 📁 Private File Storage – Each user manages their own files securely  
- 🛡️ Key-Based Security – No key = No access  

---

## 📷 Screenshot

<img width="1614" height="930" alt="Image" src="https://github.com/user-attachments/assets/204c0d8f-dc07-4cdd-b50e-6daad226fe09" />

<img width="2411" height="1440" alt="Image" src="https://github.com/user-attachments/assets/0e7d8d89-8420-441b-942d-b0a522c0c71c" />

<img width="1621" height="933" alt="Image" src="https://github.com/user-attachments/assets/f1a2c66c-556a-4743-93cc-888b142b9afc" />

<img width="1597" height="928" alt="Image" src="https://github.com/user-attachments/assets/3006272c-a25b-4ab9-acd8-216567143bb4" />

---

## 🖥️ Application Flow

1. Upload File  
   - User logs in  
   - Uploads file  
   - System generates a unique encryption key  

2. Access File  
   - User enters the secret key  
   - File is decrypted and downloaded  

3. Manage Files  
   - View uploaded files  
   - Download or delete anytime  

---

## ⚙️ Tech Stack

### 🎨 Frontend
- React.js  
- Material UI  
- Axios  
- React Router  
- React Toastify  

### 🧠 Backend
- Node.js  
- Express.js  
- MongoDB  
- Multer (file handling)  
- Crypto module (encryption/decryption)  

---

## 🛠️ Installation Guide

### 📌 Requirements

- Node.js & npm  
- MongoDB (local/cloud)  
- Git  

---

### 📥 Setup Steps

#### 1. Clone Project
```bash
git clone https://github.com/yourusername/safevault.git
cd safevault
```

#### 2. Install Dependencies

**Backend**
```bash
cd backend
npm install
```

**Frontend**
```bash
cd ../frontend
npm install
```

#### 3. Configure Database

```js
mongoose.connect("your_mongodb_connection", {
  useNewUrlParser: true,
  useUnifiedTopology: true
});
```

#### 4. Run Project

**Start Backend**
```bash
cd backend
node server.js
```

**Start Frontend**
```bash
cd frontend
npm start
```

#### 🌐 Open in Browser
```
http://localhost:3000
```

---

## 📂 Folder Structure

### Backend
```
backend/
├── models/
│   ├── FileModel.js
│   └── UserModel.js
├── uploads/
├── server.js
└── package.json
```

### Frontend
```
frontend/
├── src/
│   ├── components/
│   ├── App.js
│   ├── index.js
└── package.json
```

---

## 🔗 API Routes

### 👤 Authentication

| Route   | Method | Description    |
|--------|--------|----------------|
| /signup | POST  | Create account |
| /signin | POST  | Login user     |

---

### 📁 File Handling

| Route            | Method | Description                  |
|------------------|--------|------------------------------|
| /upload-file     | POST   | Encrypt & upload file        |
| /get-file/:id    | POST   | Decrypt & download file      |
| /check-key       | POST   | Validate secret key          |
| /user-files      | GET    | Get user files               |
| /delete-file/:id | DELETE | Remove file                  |

---

## 🔐 Environment Variables

Create a `.env` file inside backend:

```
MONGO_URI=your_mongodb_uri
PORT=5000
```
---

## 📜 License

MIT License

---
