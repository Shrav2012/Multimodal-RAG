
# 🌾 Multimodal RAG Assistant

This project is a lightweight web-based **Retrieval-Augmented Generation (RAG)** assistant built with **FastAPI**, **LangChain**, and **HuggingFace Transformers**. Users can upload PDFs and ask questions, and the app answers using content from the uploaded documents.

---

## 🚀 Features

- 🧠 RAG-powered QA with LangChain + HuggingFace
- 📄 Upload PDF documents for ingestion
- 🔍 Ask natural language questions and get AI-generated answers
- 💾 FAISS vector store for document retrieval
- 🔐 Basic token-based authentication
- 🌐 Simple static frontend (HTML + Tailwind CSS)
- 🌩️ One-click deployment using Render

---

## 🧪 Demo Credentials

You can use these hardcoded demo credentials:

```txt
Username: testuser
Password: testpass
```

---

## 📁 Project Structure

```
Multimodal-RAG/
├── app/                  # FastAPI backend logic
├── static/               # Frontend: index.html + app.js
├── requirements.txt      # Python dependencies
├── render.yaml           # Render Blueprint deployment config
```

---

## 🖥️ Local Development

```bash
# Create and activate virtual environment
python -m venv venv
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Initialize the database
python app/init_db.py

# Run the app locally
uvicorn app.main:app --reload
```

Then open `static/index.html` in a browser.

---

## 🌍 Deployment on Render

- Push this repo to GitHub
- Go to [https://render.com](https://render.com)
- Click **New + → Blueprint**
- Connect this GitHub repo
- Render will auto-detect `render.yaml` and deploy both backend and frontend

After deployment, **edit `static/app.js`** and replace:

```js
const backendURL = "http://localhost:8000";
```

With your deployed backend URL from Render.

---

## 📦 Dependencies

- fastapi
- uvicorn
- langchain
- langchain-community
- langchain-huggingface
- transformers
- faiss-cpu
- PyPDF2
- sentence-transformers
- python-jose

---

## 📃 License

MIT License
```

---

✅ Let me know if you'd like a live badge, your name at the bottom, or a screenshot section added too!
