
# 🚀 NexusLearn (PRISM)

**NexusLearn** is an AI-powered learning platform that transforms static study material into an interactive experience.
Students can chat with PDFs, generate quizzes, take mock interviews, write notes, and track study progress — all in one place using a Retrieval-Augmented Generation (RAG) pipeline.

---

## ✨ Features

* 📄 Chat with PDFs using AI (RAG)
* 🧠 Automatic quiz generation
* 🎤 AI interview practice
* 📝 Rich text notes with annotations
* 📊 Reading progress tracking
* 📚 Notebook-based document organization
* 🔐 JWT authentication

---

## 🏗 System Architecture

* **Frontend:** React 18 + Vite
* **Backend:** FastAPI (Python)
* **Database:** MongoDB
* **Vector DB:** Pinecone
* **LLM:** Groq (Llama 3)
* **Embeddings:** SentenceTransformers (all-mpnet-base-v2)

---

## 🧠 RAG Pipeline Overview

1. User uploads document
2. Text extracted and chunked
3. Chunks converted to embeddings
4. Stored in Pinecone
5. User query embedded
6. Similar chunks retrieved
7. LLM generates answer using context

---

## 📁 Project Structure

```
nexusLearn
│
├── backend
│   ├── main.py
│   ├── database.py
│   ├── auth.py
│   ├── processors/
│   └── uploads/
│
├── frontend
│   └── src
│       ├── components/
│       ├── contexts/
│       ├── App.jsx
│
└── README.md
```

---

## ⚙️ Setup Instructions

### ✅ Prerequisites

* Node.js 16+
* Python 3.8+
* MongoDB
* Pinecone account
* Groq API key

---

### 🔧 Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```

---

### 🎨 Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🔐 Environment Variables

Create `backend/.env`

```
MONGODB_URL=mongodb://localhost:27017
PINECONE_API_KEY=your_key
GROQ_API_KEY=your_key
SECRET_KEY=your_secret
```

---

## 🤝 Contributing (Team Workflow)

1. Fork or clone repository
2. Create a feature branch

```
git checkout -b feature/your-feature
```

3. Commit changes

```
git add .
git commit -m "added feature"
```

4. Push branch

```
git push origin feature/your-feature
```

5. Create Pull Request → dev branch

---

## 🧑‍💻 Team Roles (Example)

* Backend AI → RAG pipeline
* Frontend → UI & PDF viewer
* Database → MongoDB & Pinecone
* DevOps → Deployment & CI/CD

---

## 📌 Future Improvements

* Mobile app
* Voice interaction
* Adaptive learning
* Collaborative notes
* Offline mode
* Analytics dashboard

---

## 📄 License

This project is licensed under the MIT License.

---

## ⭐ Project Status

Version: **1.0.0**
Status: Active development 🚧
