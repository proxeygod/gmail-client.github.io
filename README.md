# 📧 Full-Stack Gmail IMAP Client

A modern, **full-stack Gmail client** that allows users to securely connect to their Gmail account, view, search, and paginate through their emails.  
This project leverages a **React frontend**, a **Node.js backend**, and a **MySQL database** to provide a fast, responsive, and persistent email viewing experience.

---

## 📸 Screenshots

| Signin Page | Inbox Page |
|--------------------|------------------|
| ![Life Calendar](https://filedn.eu/lKBQ3k74oxYj0kgKuxh2wfS/Gmail%20Client/signin%20page.png) | ![Add new Counter](https://filedn.eu/lKBQ3k74oxYj0kgKuxh2wfS/Gmail%20Client/inbox.png) |

---

## ✨ Features
- 🔐 **Secure Google OAuth 2.0 Authentication** – Log in safely with your Google account without sharing your password.  
- 📥 **IMAP Email Fetching** – Connects directly to Gmail's IMAP server to sync email metadata.  
- 💾 **Persistent Database Storage** – Stores email metadata in MySQL for lightning-fast access and history.  
- 🔍 **Dynamic Search** – Instantly search synced emails by sender or subject.  
- 📄 **Pagination** – Navigate your inbox with "Next" and "Previous" controls.  
- 💻 **Modern & Responsive UI** – Clean, mobile-friendly interface built with React + Tailwind CSS.  
- 🛡️ **Centralized Error Handling** – Robust backend error middleware for stability.  

---

## 🛠️ Tech Stack
- **Frontend:** React, Tailwind CSS  
- **Backend:** Node.js, Express.js  
- **Database:** MySQL  
- **Authentication:** Google OAuth 2.0  
- **Email Sync:** IMAP  

---

## 🚀 Getting Started

Follow these steps to set up the project locally:

### ✅ Prerequisites
- Node.js (**v18+**)
- npm
- Running MySQL server

### ⚙️ Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/SuwanSankaja/gmail-client.git
   cd gmail-client
   ```

2. **Setup Backend**
   ```bash
   cd backend
   npm install
   ```

3. **Setup Frontend**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Configure Environment Variables**  
   In the `/backend` directory, create a `.env` file with:

   ```env
   # Server Port
   PORT=5000

   # Database Credentials
   DB_HOST=localhost
   DB_USERNAME=your_db_user
   DB_PASSWORD=your_db_password
   DB_DATABASE=gmail_client_db

   # Google OAuth2 Credentials
   GOOGLE_CLIENT_ID=your_client_id_from_google
   GOOGLE_CLIENT_SECRET=your_client_secret_from_google

   # Session Secret
   SESSION_SECRET=a_long_random_string_for_session_encryption
   ```

5. **Setup the Database**
   ```bash
   # Ensure MySQL server is running
   # Create a new database (e.g., gmail_client_db)

   npm run db:migrate
   ```

6. **Run the Application**
   ```bash
   # Start Backend
   cd backend
   node index.js

   # Start Frontend (in another terminal)
   cd frontend
   npm start
   ```

7. Open [http://localhost:3000](http://localhost:3000) 🎉

---

## 💡 Contributing
Contributions are welcome! Feel free to fork this repo, submit issues, or open pull requests.  

---

