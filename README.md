# 🔐 SecureNote

<div align="center">

![Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

**Share secrets securely. Self-destruct on demand. Zero traces left behind.**

A powerful MERN stack application for creating encrypted, self-destructing notes that disappear after being read.

[🎯 Features](#-features) • [🚀 Live Demo](https://mysecurenote.netlify.app/) • [📦 Installation](#-installation) • [💡 Usage](#-usage) • [🛠️ Tech Stack](#️-tech-stack)

### [🌐 **TRY IT LIVE**](https://mysecurenote.netlify.app/) 🌐

---

</div>

## 🎯 Why SecureNote?

Ever needed to share sensitive information like passwords, API keys, or confidential messages without leaving a permanent digital trail? **SecureNote** solves this problem elegantly:

- ✅ **Privacy First** - Notes self-destruct automatically
- ✅ **Zero Knowledge** - Optional password encryption means even we can't read your notes
- ✅ **Time-Controlled** - Set custom expiration times
- ✅ **One-Time Access** - Notes disappear after being read once
- ✅ **Notification System** - Get alerted when notes are destroyed
- ✅ **No Sign-Up Required** - Instant sharing with zero friction

> **🎮 [Try it now](https://mysecurenote.netlify.app/)** - No installation needed!

---

## 📸 Screenshots

### 🏠 Create Your Secure Note
<div align="center">
<img width="1295" alt="Create Note Interface" src="https://github.com/user-attachments/assets/7dcc6642-592f-42d9-8648-e473f43c2d79" />

*Intuitive interface with emoji support, password protection, and flexible expiration options*
</div>

### 🔗 Shareable Link Generated
<div align="center">
<img width="1005" alt="Generated Secure Link" src="https://github.com/user-attachments/assets/7f054651-699c-43bc-a731-7c03ee643d55" />

*Instantly get a shareable link - copy and send via any channel*
</div>

### 📖 Note Viewing Experience
<div align="center">
<img alt="Viewing Secure Note" src="https://github.com/user-attachments/assets/63cc397f-223f-40c9-a8b0-1f7206daa2d6" />

*Clean, distraction-free reading experience*
</div>

### 💥 After Note Destruction
<div align="center">
<img width="1079" alt="Note Destroyed Confirmation" src="https://github.com/user-attachments/assets/2b7ab5a5-a7e5-4f0b-bebf-ca3fcf23950b" />

*Clear confirmation when note has been destroyed - no traces left*
</div>

---

## ✨ Features

### 🔒 **Security Features**
- **End-to-End Encryption** - Password-protected notes are encrypted before storage
- **Self-Destruct Options** - Choose between one-time read or time-based expiration
- **Zero Persistence** - Notes are permanently deleted after conditions are met
- **Secure Link Generation** - Unique, unguessable URLs for each note

### 🎨 **User Experience**
- **Rich Text Support** - Full emoji picker integration for expressive notes
- **Custom Expiration Times** - Set notes to expire in minutes, hours, or days
- **Email Notifications** - Optional alerts when your note is accessed/destroyed
- **Custom URL Slugs** - Create memorable links with custom titles
- **Mobile Responsive** - Works flawlessly on all devices

### 🚀 **Technical Excellence**
- **Modern Stack** - Built with React, Node.js, Express, and MongoDB
- **Material-UI Design** - Beautiful, intuitive interface
- **Form Validation** - Robust validation with Yup
- **RESTful API** - Clean, scalable backend architecture

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technologies |
|-------|-------------|
| **Frontend** | ![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB) ![Material-UI](https://img.shields.io/badge/Material--UI-0081CB?style=flat&logo=material-ui&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white) |
| **Backend** | ![Node.js](https://img.shields.io/badge/Node.js-43853D?style=flat&logo=node.js&logoColor=white) ![Express.js](https://img.shields.io/badge/Express.js-404D59?style=flat&logo=express&logoColor=white) |
| **Database** | ![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=flat&logo=mongodb&logoColor=white) |
| **Deployment** | ![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat&logo=netlify&logoColor=white) ![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=white) |
| **Libraries** | Axios • React Router • Yup • emoji-picker-react |

</div>

---

## 📦 Installation

### Prerequisites

Ensure you have the following installed:
- **Node.js** (v14 or higher)
- **npm** or **yarn**
- **MongoDB** (local or Atlas URI)

### 🔧 Backend Setup

```bash
# Navigate to server directory
cd server

# Install dependencies
npm install

# Create .env file with the following variables:
# MONGO_URI=your_mongodb_connection_string
# PORT=5000
# JWT_SECRET=your_secret_key
# EMAIL_SERVICE=your_email_service (optional)
# EMAIL_USER=your_email (optional)
# EMAIL_PASS=your_email_password (optional)

# Start the server
npm start
# Server will run on http://localhost:5000
```

### 🎨 Frontend Setup

```bash
# Navigate to client directory
cd client

# Install dependencies
npm install

# Start development server
npm run dev
# App will open at http://localhost:5173
```

---

## 💡 Usage

### Creating a Secure Note

1. **Compose Your Message**
   - Visit [mysecurenote.netlify.app](https://mysecurenote.netlify.app/)
   - Type or paste your sensitive content
   - Use the emoji picker (😊) to add personality

2. **Configure Security Settings**
   - **Self-Destruct**: Choose "After reading" or set a custom time
   - **Password Protection**: Add a password for encryption (optional)
   - **Email Notification**: Get notified when note is destroyed (optional)
   - **Custom Link**: Create a memorable URL slug (optional)

3. **Generate & Share**
   - Click **"Create Note"**
   - Copy the generated secure link
   - Share via email, Slack, WhatsApp, or any channel
   - ⚠️ **Important**: Save the link! You won't see it again

4. **Recipient Experience**
   - Recipient opens the link
   - Enters password if required
   - Reads the note
   - Note self-destructs automatically ✅

---

## 🏗️ Project Structure

```
SecureNote/
│
├── client/                    # React frontend
│   ├── src/
│   │   ├── Components/
│   │   │   ├── NoteForm.jsx   # Note creation form
│   │   │   ├── NoteView.jsx   # Note display component
│   │   │   └── EmojiPicker.jsx
│   │   ├── pages/
│   │   │   ├── Home.jsx       # Landing page
│   │   │   ├── CreateNote.jsx
│   │   │   └── ViewNote.jsx
│   │   ├── constants.js       # App constants
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
│
├── server/                    # Node.js + Express backend
│   ├── controllers/
│   │   └── noteController.js  # Note CRUD operations
│   ├── models/
│   │   └── Note.js            # Mongoose schema
│   ├── routes/
│   │   └── noteRoutes.js      # API endpoints
│   ├── middleware/
│   │   └── auth.js            # Authentication middleware
│   ├── utils/
│   │   ├── encryption.js      # Encryption utilities
│   │   └── emailService.js    # Email notifications
│   ├── index.js               # Server entry point
│   └── package.json
│
├── .gitignore
└── README.md
```

---

## 🔐 Security Considerations

- **Encryption**: Notes with passwords are encrypted using industry-standard algorithms
- **Database Security**: Sensitive data is never stored in plain text
- **HTTPS Recommended**: Deploy with SSL/TLS for production use
- **No Logs**: Note content is never logged or cached
- **Automatic Cleanup**: Background jobs remove expired notes regularly

---

## 🚀 Deployment

### Live Application

**Frontend**: Deployed on [Netlify](https://mysecurenote.netlify.app/)  
**Backend**: Deployed on Render (or your hosting platform)  
**Database**: MongoDB Atlas

### Deploy Your Own Instance

**Frontend (Client):**
```bash
# Build the client
npm run build

# Deploy to Netlify
# Connect your GitHub repo to Netlify for automatic deployments
```

**Backend (Server):**
```bash
# Deploy to Render, Railway, or Heroku
# Set environment variables in your hosting platform
# Connect to MongoDB Atlas
```

---

## 🤝 Contributing

Contributions make the open-source community amazing! Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/notes` | Create a new note |
| GET | `/api/notes/:id` | Retrieve a note by ID |
| DELETE | `/api/notes/:id` | Delete a note (automatic) |
| POST | `/api/notes/verify` | Verify password for encrypted note |

---

## 🐛 Troubleshooting

**Issue**: MongoDB connection failed  
**Solution**: Check your `MONGO_URI` in `.env` file

**Issue**: CORS errors  
**Solution**: Ensure backend URL is correctly set in frontend API calls

**Issue**: Email notifications not working  
**Solution**: Verify email service credentials in `.env`

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 👨‍💻 Author

**Tayba Shaikh**

- 💼 **GitHub**: [@Tabbie05](https://github.com/Tabbie05)
- 💼 **LinkedIn**: [Tayba Shaikh](https://www.linkedin.com/in/tayba-shaikh-340448319)
- 🌐 **Live Demo**: [mysecurenote.netlify.app](https://mysecurenote.netlify.app/)
- 📁 **All Projects**: [github.com/Tabbie05](https://github.com/Tabbie05)

---

## 🙏 Acknowledgments

- [Material-UI](https://mui.com/) for the beautiful component library
- [MongoDB](https://www.mongodb.com/) for the powerful database
- [emoji-picker-react](https://github.com/ealush/emoji-picker-react) for emoji support
- [Netlify](https://www.netlify.com/) for seamless frontend deployment
- Inspiration from services like Privnote and One-Time Secret

---

<div align="center">

### ⭐ Star this repo if you find it useful!

**Built with ❤️ for privacy and security by Tayba Shaikh**

[🌐 Live Demo](https://mysecurenote.netlify.app/) • [Report Bug](https://github.com/Tabbie05/SecureNote/issues) • [Request Feature](https://github.com/Tabbie05/SecureNote/issues)

</div>
