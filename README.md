# SecureNote 🔐

SecureNote is a simple and secure note‑sharing web app built with the MERN stack.  
It allows users to create encrypted or self‑destructing notes, optionally protected with a password, and share a generated link. Perfect for sensitive or temporary sharing of information.

---

## Screenshots
### Homepage / Create Note
![Create Note Page]
<img width="1295" height="629" alt="securenote1" src="https://github.com/user-attachments/assets/7dcc6642-592f-42d9-8648-e473f43c2d79" />



### Note Created / Link Generated
![Note Link Page]
<img width="1005" height="408" alt="securenote2" src="https://github.com/user-attachments/assets/7f054651-699c-43bc-a731-7c03ee643d55" />


### Example Note View
![Example Note]
![securenote3](https://github.com/user-attachments/assets/63cc397f-223f-40c9-a8b0-1f7206daa2d6)


### After Note View
[[Example After View]]
<img width="1079" height="526" alt="image" src="https://github.com/user-attachments/assets/2b7ab5a5-a7e5-4f0b-bebf-ca3fcf23950b" />


## 🚀 Features

- Create a new note with rich text (supports emojis via emoji picker)  
- Option to have the note self‑destruct after reading or after a chosen time  
- Optional password‑based encryption for the note  
- Optional notification email when the note is destroyed  
- Generate a shareable link for the note  
- Clean UI built with Material UI  

---

## 📦 File Structure

SecureNote/
```bash
├── client/               # React frontend
│   ├── src/              # Source code
│   │   ├── Components/   # React components (NoteForm, etc.)
│   │   ├── pages/        # App pages
│   │   ├── constants.js  # Constants for expiration, text info, etc.
│   │   └── App.jsx       # Main React app
│   └── package.json
├── server/               # Node.js + Express backend
│   ├── index.js          # Entry point
│   ├── routes/           # API routes (e.g., /api/notes)
│   ├── controllers/      # Controllers for note handling
│   ├── models/           # Mongoose models
│   └── package.json
├── screenshots/          # Screenshots of the app (PNG/JPG)
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

### usage:
  description: "How to Use SecureNote"
  steps:
    - "Open the app in your browser (default http://localhost:5173/)."
    - "Enter your note content (supports emojis via the emoji picker)."
    - "Optionally set:"
    - "  - Self-destruct option: After reading or a chosen time."
    - "  - Password: Encrypt the note with a password."
    - "  - Notification email: Receive email when note is destroyed."
    - "  - Link title: Custom URL for your note."
    - "Click Create Note."
    - "Copy the generated link and share."
    - "The recipient can view the note, and it will auto-destroy according to your settings."





