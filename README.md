# 🍽️ YourHungry AI

YourHungry AI is an AI-powered culinary assistant that generates recipes, dish images, nearby restaurants, and remembers your chat sessions. Built with React, Express, MongoDB, and OpenAI.

---

## 🔧 Tech Stack

- **Frontend**: React, React Router, custom CSS (glassmorphism)
- **Backend**: Express.js + MongoDB Atlas
- **Authentication**: Email/password, Google OAuth, GitHub OAuth
- **Image API**: Unsplash
- **Location + Restaurants**: Google Places API
- **Email OTP**: Resend API
- **AI Model**: OpenAI `gpt-3.5-turbo`

---

## ✨ Features

- 🧠 Chatbot that answers culinary queries
- 📸 AI-generated food images via Unsplash
- 📍 Nearby restaurants via Google Maps
- 💬 Persistent chat history with edit/delete support
- 🔒 Secure login (OAuth + JWT)
- 📧 Password reset with OTP

---

## 🗂️ Project Structure

```
/client     # React frontend
/server     # Express backend
```

---

## 🚀 Local Setup

### 1. Clone the Repository

```bash
git clone https://github.com/mrohan2203/yourhungryai.git
cd yourhungryai
```

### 2. Backend Setup

```bash
cd server
npm install
```

Create `.env` in `server/`:

```
PORT=5001
MONGODB_URI=your_mongo_uri
JWT_SECRET=your_jwt_secret
RESEND_API_KEY=your_resend_api_key
RESEND_EMAIL_FROM=your_verified_email
REACT_APP_GOOGLE_CLIENT_ID=your_google_id
REACT_APP_GOOGLE_CLIENT_SECRET=your_google_secret
REACT_APP_GITHUB_CLIENT_ID=your_github_id
REACT_APP_GITHUB_CLIENT_SECRET=your_github_secret
GOOGLE_PLACES_API_KEY=your_google_maps_key
```

Start backend:

```bash
node server.js
```

### 3. Frontend Setup

```bash
cd ../client
npm install
```

Create `.env` in `client/`:

```
REACT_APP_API_URL=http://localhost:5001
REACT_APP_OPENAI_API_KEY=your_openai_key
REACT_APP_UNSPLASH_ACCESS_KEY=your_unsplash_key
```

Run frontend:

```bash
npm start
```

---

## 🌐 Deployment

- **Frontend**: Vercel (`yourhungry.net`)
- **Backend**: Render (`api.yourhungry.net`)
- Ensure `.env` is set correctly on both.

---

## ✅ To-Do

- [ ] Calories per dish
- [x] Restaurant links in new tab
- [x] Responsive styling
- [ ] Add voice support
- [ ] Admin dashboard

---
