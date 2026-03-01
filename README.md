# 🎙️ Interview Voice Bot

A voice-powered personal assistant for job interviews.

## Quick Setup (5 minutes)

### 1. Get Free Gemini API Key
- Go to: https://aistudio.google.com/app/apikey
- Click "Create API Key" → Copy it

### 2. Edit Your Profile
Open `app.py` and fill in YOUR_PROFILE section with:
- Your name, skills, experience, education, projects

### 3. Run Locally
```bash
pip install -r requirements.txt
export GEMINI_API_KEY="your_key_here"     # Mac/Linux
# set GEMINI_API_KEY=your_key_here        # Windows
python app.py
```
Open: http://localhost:5000

---

## 🚀 Deploy Free on Render.com (10 min)

1. Push this folder to a GitHub repo
2. Go to https://render.com → New → Web Service
3. Connect your GitHub repo
4. Settings:
   - **Build Command:** `pip install -r requirements.txt`
   - **Start Command:** `gunicorn app:app --bind 0.0.0.0:$PORT`
5. Add environment variable: `GEMINI_API_KEY` = your key
6. Click Deploy → Get your URL! 🎉

---

## Features
- 🎤 Voice input (Web Speech API, no cost)
- 🔊 Voice output (browser TTS, no cost)
- 💬 Text fallback input
- 🧠 Gemini AI responses (free tier)
- 💾 Conversation memory within session
- 🎨 Beautiful dark UI
