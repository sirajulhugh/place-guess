# 🌍 World Explorer  
*A Geography Guessing Game*  

🔍 Guess your location using **Google Street View** and test your geography skills!  

[![Netlify Status](https://api.netlify.com/api/v1/badges/YOUR-DEPLOY-ID/deploy-status)]([https://app.netlify.com/sites/YOUR-SITE-NAME/deploys](https://world-explorer2504.netlify.app/))  

---

## 🚀 Features  
- **Street View Exploration**: Get dropped into a random global location  
- **Map Guessing**: Pinpoint your guess on an interactive world map  
- **AI-Powered Hints**: Get clues via **Google Gemini** AI  
- **Scoring System**: Earn points based on accuracy  
- **Secure API Keys**: Serverless backend protects sensitive keys  

---

## 🛠️ Tech Stack  
| **Category**       | **Technology**                     |  
|--------------------|-----------------------------------|  
| **Frontend**       | HTML5, CSS3, JavaScript           |  
| **Maps API**       | Google Maps & Street View         |  
| **AI Hints**       | Google Gemini API                 |  
| **Backend**        | Netlify Functions (Node.js)       |  
| **Hosting**        | Netlify                           |  

---

## 📂 Project Structure  

├── index.html # Main HTML entry point
├── game-test.js # Core game logic
├── config.js # Geographic search zones
├── style.css # Styling
├── netlify/ # Serverless functions
│ ├── functions/
│ │ ├── get-key.js # Fetches Google Maps key
│ │ ├── get-gemini-key.js # Fetches Gemini key
│ │ └── get-gemini-hint.js # Proxies Gemini API requests
└── apiKey.js # Local API keys (ignored by Git)


---

## 🛠️ Setup  

### 1. Local Development  
in bash
git clone https://github.com/sirajulhugh/place-guess.git  
cd world-explorer  
Set Up API Keys
Create apiKey.js in the root directory:


const GOOGLE_API_KEY = "your-google-maps-key";  
const GEMINI_API_KEY = "your-gemini-key";  

2. Netlify Deployment
Push your repo to GitHub/GitLab

Deploy to Netlify and set these environment variables:

GOOGLE_API_KEY

GEMINI_API_KEY

🔒 API Key Security
Production: Keys fetched via Netlify Functions (never exposed client-side)

Local: Uses apiKey.js (never commit this file!)

🎮 How to Play
Click "Start Game" to enter a random Street View location

Use the map to guess your location

Need help? Click "Get Hint" (with a time penalty!)

Submit your guess and see your score!

🌟 Future Ideas
Add a leaderboard (Firebase/Supabase)

Implement multiplayer mode

Optimize AI hints with caching

📜 License
MIT © SIRAHULHUGH

