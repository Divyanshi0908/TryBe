# 🚀 Trybe

> TRYBE = TRY + VIBE  
> A smarter shopping experience — seamless, engaging, and AI-powered.

---

## 🎯 Problem Statement

Theme 2: The GenZ Way of Shopping  

Current issues with traditional shopping platforms:  
- 🔒 Ultimate GlamClan features are buried, making them hard to discover.  
- 🎁 Rewards are hidden, reducing accessibility and user engagement.  
- 🧠 Fashion GPT (vibe-based search) is not integrated with normal search.  
- 🔎 Lack of vibe-based search functionality in discovery sections like GlamStream.  

---

## 💡 Opportunity

Why Trybe is a Game-Changer  
- Easier access = higher engagement + better experiences.  
- Boosts visibility, trust, and social connections.  
- Perfectly aligns with GenZ’s preference for authenticity, social sharing, and discovery.  
- Positions Trybe (and partners like Myntra) as a trendsetter in fashion-tech innovation.  

📊 Proven Success Inspiration:  
- YouTube Shorts → Watch time ↑ 135% by moving to homepage.  
- Instagram Reels → 3× engagement after homepage placement.  

---

## ✅ Proposed Solution

TRYBE = TRY + VIBE

### 🔹 Features Enhanced & Added
- 🏆 Always-visible rewards on the homepage → Boosts engagement.  
- 🔍 Integrated mood/vibe-based search → Simplifies discovery.  
- 🎥 Video reviews with links & interactions → Social + influencer-driven content.  
- ⬆ Easy video uploads with captions → Fresh, user-driven engagement.  
- 🏷 Added vibe & category filters in GlamStream → Smarter, contextual recommendations.  

---

## 🛠 Tech Stack

Frontend  
- React 18  
- TailwindCSS  
- Vite  
- React Router, Swiper, React Player  

Backend  
- Node.js + Express  
- MongoDB + Mongoose  
- Cloudinary (video uploads)  
- Axios, Bcrypt  
- Express File Upload  

PyBackend (AI Service)  
- FastAPI  
- Uvicorn  
- Sentence Transformers (all-MiniLM-L6-v2)  

---

## 📂 Project Structure

Trybe/
├── Backend/ # Node.js + Express backend
│ ├── controllers/ # API controllers
│ ├── routes/ # API routes
│ ├── Schema/ # Mongoose schemas
│ ├── DatasetCreation/ # Seed & embeddings
│ └── Utils/ # Utility functions
│
├── Frontend/ # React + Tailwind frontend
│ ├── src/ # UI components
│ ├── index.html
│ └── package.json
│
├── pybackend/ # FastAPI service for embeddings
│ ├── app.py
│ └── requirements.txt



---

## ⚡ Getting Started

### 1️⃣ Clone Repository
bash
git clone https://github.com/your-username/trybe.git
cd trybe


### 2️⃣ Setup Backend (Node.js API)
bash
cd Backend
npm install


--Create a .env file in Backend/ with:
env
MONGO_URI=your_mongodb_connection
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret


--Run server:
bash
npm start

### Server runs at http://localhost:5000

### 3️⃣ Setup Frontend (React + Vite)
bash
cd Frontend
npm install
npm run dev

### Frontend runs at http://localhost:5173

### 4️⃣ Setup PyBackend (FastAPI Service)
bash
cd pybackend
pip install -r requirements.txt
uvicorn app:app --host 0.0.0.0 --port 8000

### Embedding API available at http://localhost:8000/embed

## 📡 API Endpoints
| Method | Endpoint                          | Description                       |
| ------ | --------------------------------- | --------------------------------- |
| POST   | /api/register                   | Register new user                 |
| POST   | /api/login                      | Login user                        |
| GET    | /api/fetch-Image                | Get all product images            |
| GET    | /api/vibe-search?text=...       | Search products by text embedding |
| GET    | /api/vibe-search-video?text=... | Search videos by vibe             |
| GET    | /api/fetch-title                | Get all product titles            |
| POST   | /api/upload-video/:id           | Upload video review for a product |
| GET    | /api/tag-search?tags=tag1,tag2  | Get videos by tags                |
| GET    | /api/video/:id                  | Get user + posts                  |


## 🖼 Architecture & Screenshots

### 🏗 Architecture


### UI Previews

## 🚀 Future Enhancements
- 🔑 JWT Authentication & Authorization
- 📱 In-App Product Sharing with friends
- 🎉 Festive Contests & Trend Challenges
- 🗳 User Polls & Feedback → Personalized recommendations
- ⭐ Product rating system
- 🤖 Recommendation engine (based on user activity)
