# SecureNote 🔐

SecureNote is a simple and secure note‑sharing web app built with the MERN stack.  
It allows users to create encrypted or self‑destructing notes, optionally protected with a password, and share a generated link. Perfect for sensitive or temporary sharing of information.

---

## Screenshots
### Homepage / Create Note
![Create Note Page](screenshots/securenote1.PNG)

### Note Created / Link Generated
![Note Link Page](screenshots/securenote2.PNG)

### Example Note View
![Example Note](screenshots/securenote3.JPG)


## 🚀 Features

- Create a new note with rich text (supports emojis via emoji picker)  
- Option to have the note self‑destruct after reading or after a chosen time  
- Optional password‑based encryption for the note  
- Optional notification email when the note is destroyed  
- Generate a shareable link for the note  
- Clean UI built with Material UI  

---

## 📁 Project Structure

SecureNote/
├── client/ # React frontend
│ ├── src/ # React source code (components, pages, etc.)
│ └── …
├── server/ # Node.js + Express backend
│ ├── index.js # Entry point
│ ├── routes/ # API endpoints (e.g. /api/notes)
│ └── …
├── screenshots/ # Place your screenshots here
├── .gitignore
└── README.md


---

## 🧑‍💻 Tech Stack

- **Frontend:** React, Material UI (MUI), emoji-picker-react  
- **Backend:** Node.js, Express, MongoDB (via Mongoose)  
- **Other:** Form validation via Yup, HTTP requests via axios, routing with react-router-dom  

---

## 📦 Getting Started

### Prerequisites

- Node.js and npm installed  
- MongoDB running locally or a MongoDB Atlas (or similar) URI  

### Setup backend

```bash
cd server
npm install
# configure your .env (e.g. MONGO_URI, PORT etc.)
npm start              # or `node index.js` if not using nodemon

### Setup frontend
```bash
cd client
npm install
npm run dev 

Usage

Open the app in your browser
Fill in note content (plus emojis if desired)
Optionally configure: destroy-after option, password, notification email, link title
Click Create Note
Copy the generated link and share — note will be viewable/permanent or self-destructive as per settings


