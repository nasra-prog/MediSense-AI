# MediSense AI — Smart Health Assistant

An AI-powered health assistant that helps users check symptoms, get health tips, handle emergencies, and ask general medical questions.

---

## What It Does

| Feature | Description |
|---|---|
| 🩺 Symptom Checker | Describe symptoms and get a possible assessment |
| 💊 Health Tips | Get lifestyle and wellness advice |
| 🚨 Emergency Guide | Know when to seek urgent medical care |
| 📋 Health Q&A | Get answers to general medical questions |

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python, Flask |
| AI | Claude API by Anthropic |
| Database | SQLite |

---

## Project Structure

```
med/
├── frontend/
│   ├── index.html       — Main UI page
│   ├── style.css        — All styling
│   └── script.js        — Frontend logic
│
├── backend/
│   └── app.py           — Flask API server
│
├── database/
│   ├── schema.sql       — Table definitions
│   └── db.py            — Database functions
│
├── ai/
│   └── ai_logic.py      — Claude AI integration
│
└── docs/
    └── README.md        — This file
```

---

## How To Run

### 1. Install dependencies
```bash
pip install flask flask-cors anthropic
```

### 2. Set your API key
```bash
set ANTHROPIC_API_KEY=your_key_here
```

### 3. Start the backend
```bash
cd backend
python app.py
```

### 4. Open the frontend
Right click `frontend/index.html` in VS Code and click **Open with Live Server**

---

## How It Works

1. User types a message in the browser
2. script.js sends it to Flask backend at localhost:5000
3. app.py saves it to SQLite and calls ai_logic.py
4. ai_logic.py sends it to Claude AI with a medical system prompt
5. Claude replies and it is shown in the chat

---

## Disclaimer

MediSense AI is for informational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified doctor for medical concerns.