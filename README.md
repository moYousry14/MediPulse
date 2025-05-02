# MediPulse 1.0

MediPulse is an AI-powered medical assistant chatbot built with Flask, LangChain, and Groq's LLaMA 3 model.  
It provides preliminary health guidance in both **English** and **Arabic**, ensuring safe, concise, and ethical medical responses.

---

## 🌐 Live Interaction

MediPulse offers an API-driven interface that supports:

- **Structured medical intake** (age, smoker, conditions)
- **Dynamic language handling** (Arabic or English)
- **Context-aware follow-up**
- **Safe and ethical symptom analysis**
- **Over-the-counter suggestions with disclaimers**

---

## ⚙️ Tech Stack

- **Python** (Flask)
- **LangChain**
- **Groq API (LLaMA 3 70B)**
- **Flask-Session**
- **Postman-compatible REST API**
- **Frontend**: Basic HTML/CSS/JS (chatbox UI)

---

## 🔌 API Endpoints

### `POST /api/start`
- Initializes a new session.
- Returns the first question in both languages.

### `POST /api/chat`
- Accepts user replies.
- Responds with either the next question or a medical assessment based on user inputs and Groq response.

---

## 📁 Project Structure

MediMulse/
├── medipulseGROQ.py # Main Flask backend
├── requirements.txt # Python dependencies
├── Procfile # For deployment (e.g., Railway)
├── templates/
│ └── index.html # Web UI template
├── static/
│ ├── style.css # Chat UI styling
│ └── script.js # Frontend JS (user interaction)
