```markdown
# 🧠 Memory Chatbot

Build an **AI Agent with Memory** using LangChain / LangGraph.  
This project shows how to create chatbots that **remember past conversations, summarize efficiently, and persist context across sessions**.

---

## ✨ Features
- Persistent conversation memory  
- Summarization to reduce token usage  
- Vector DB / local storage support  
- Hands-on LangChain & LangGraph code examples  
- Real-world use cases (booking, expense claims, workflow automation)

---

## 📂 Project Structure
```

.
├── memory\_chatbot.ipynb   # Main notebook
├── requirements.txt       # Dependencies
├── .env.example           # Environment variables
├── data/                  # Memory persistence
└── README.md

````

---

## ⚡ Quickstart

### 1. Clone the repo
```bash
git clone <your-repo-url>
cd <your-repo-folder>
````

### 2. Create a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate      # macOS/Linux
.venv\Scripts\activate         # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment

Copy `.env.example` → `.env` and update:

```ini
OPENAI_API_KEY=sk-xxxx
VECTORSTORE=chroma
CHROMA_PERSIST_DIR=./data/chroma
```

### 5. Run the notebook

```bash
jupyter lab
```

Open `memory_chatbot.ipynb` and run cells step by step.

---

## 🔑 How It Works

1. Stores **short-term + long-term memory**
2. Uses **summarization** to compress old chats
3. Persists memory via vector DB or local JSON
4. Retrieves key facts at each new session

---

## 🐳 Run with Docker (optional)

```bash
docker build -t memory-chatbot .
docker run -p 8888:8888 --env-file .env memory-chatbot
```

---

## 🤝 Contributing

1. Fork the repo
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit changes
4. Open a PR 🎉

---

## 📜 License

MIT — use it freely.
Maintained by **Saran GenAI Labs**.

```

---

✅ This will render cleanly on GitHub with proper headings, lists, and code blocks.  

Do you also want me to **generate the `requirements.txt`** automatically from your notebook (`memory_chatbot.ipynb`) so the repo is fully plug-and-play?
```
