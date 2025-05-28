# 🎨 ArtifexGenie — AI Image Generator

**"Artifex"** (Latin for artist) + **"Genie"** (a magical creative force)  
> **Unleash magical visuals from your imagination!**

ArtifexGenie is a full-stack AI-powered application that lets users generate stunning images from text prompts using OpenAI's DALL·E API, view them in a modern UI, and download or manage them easily.

---

## 📌 Features

- ✨ Generate AI images from text prompts
- 🖼️ Lazy-load images for performance
- 📥 Download images to your device
- 🔎 Search through existing

---

🎨 2. Frontend Setup (React)
bash :
cd client
npm install
npm start
🔧 Frontend Libraries Used
bash:
npm install @emotion/react @emotion/styled @mui/material @mui/icons-material @mui/lab \
axios file-saver react-router-dom styled-components react-lazy-load-image-component

---

📁 Folder Structure (client/src)
client/src/
├── api/
│   └── index.js                   # Axios instance
├── components/
│   ├── Navbar.jsx
│   ├── Button.jsx
│   ├── TextInput.jsx
│   ├── SearchBar.jsx
│   ├── ImageCard.jsx
│   └── GeneratedImageCard.jsx
├── pages/
│   ├── Home.jsx
│   └── CreatePost.jsx
├── utils/
│   └── Theme.js                   # Emotion/MUI theme
├── App.js                         # Routes, layout, theme
└── index.js                       # React DOM entry point


🧠 3. Backend Setup (Node.js + Express)
bash:

cd ../server
npm install
npm install -D nodemon
📁 Folder Structure (server/)
bash:
server/
├── controllers/
│   ├── postController.js          # CRUD + logic
│   └── generateImage.js           # DALL·E API integration
├── models/
│   └── posts.js                   # Mongoose schema
├── routes/
│   └── post.js                    # API endpoints
├── index.js                       # Express entry point
├── error.js                       # Error handler middleware
├── .env                           # Secret keys
├── package.json
└── .gitignore
📄 Add to package.json
json:
"type": "module",
"scripts": {
  "start": "nodemon index.js"
}

🔐 Environment Variables (.env)
env :

PORT=5000
MONGO_URI=your_mongodb_connection_string
OPENAI_API_KEY=your_openai_api_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret

▶ Start the Backend Server
bash:
node index.js


📁 Project Structure

ArtifexGenie/
├── README.md
├── .gitignore
│
├── client/
│   ├── public/
│   └── src/
│       ├── api/
│       ├── components/
│       ├── pages/
│       ├── utils/
│       ├── App.js
│       └── index.js
│
├── server/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── index.js
│   ├── error.js
│   └── .env


💡 Inspiration
ArtifexGenie is inspired by the idea of democratizing creativity. Whether you're a designer, marketer, educator, or student — imagine it, type it, and generate it instantly with the power of AI.

📜 License
This project is licensed under the MIT License.

✨ Slogan
“ArtifexGenie — Your Creative Wish, Instantly Granted.”

