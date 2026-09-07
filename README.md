# 🤖 Telegram RAG Chatbot with Groq — n8n Automation Project

A two-workflow automated AI chatbot system on Telegram that answers questions from business documents stored in Google Drive — with zero manual work.

**Built with:** n8n · Google Drive · Pinecone · Google Gemini · Groq AI · Telegram

---

## 📌 What It Does

When a new file lands in Google Drive, it is automatically chunked, embedded via Google Gemini, and stored in Pinecone. A Telegram bot then lets users ask questions answered in real time by a Groq-powered AI Agent with conversation memory.

---

## 🎯 Problem It Solves

Most businesses manually answer the same document questions every day, have no 24/7 support, and struggle to keep chatbot knowledge up to date. This system:

- ✅ Automatically indexes new Google Drive documents into Pinecone
- ✅ Answers customer questions instantly 24/7 via Telegram
- ✅ Retrieves accurate answers from real business documents (RAG)
- ✅ Maintains conversation memory across messages
- ✅ Requires zero human intervention for standard queries

---

## ⚡ How It Works

**Workflow 1 — Knowledge Ingestion:**
1. Google Drive Trigger detects a new file
2. File is downloaded and text is extracted
3. Text is chunked with Recursive Character Text Splitter
4. Google Gemini converts chunks into vectors
5. Vectors are stored in Pinecone with metadata

**Workflow 2 — Chatbot Query:**
1. Telegram Trigger fires on incoming message
2. AI Agent receives and processes the query via Groq
3. Pinecone Vector Store is queried for relevant chunks
4. Simple Memory maintains conversation context
5. A grounded answer is sent back on Telegram

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| n8n | Workflow automation engine |
| Google Drive | Knowledge base document storage |
| Pinecone | Vector database for semantic search |
| Google Gemini | Text embedding model |
| Groq | Fast LLM for AI responses |
| Simple Memory | Conversation history within sessions |
| Telegram | Customer-facing chat interface |

---

## 🔗 Links

- 📹 [Demo Video](https://drive.google.com/file/d/1gJItQyNcPBt-UgcnBJA9BGe-g51Z1ZTo/view?usp=drive_link)
- 📁 [Workflow JSON](https://drive.google.com/file/d/10B58QpsY9W0RCNnsSXhjPGwA4d7RXxbG/view?usp=drive_link)

---

## 👤 Author

**Omi Mojumdar**  
[LinkedIn](https://www.linkedin.com/in/omi-mojumdar-900923388) · [omimojumdar88@gmail.com](mailto:omimojumdar88@gmail.com)
