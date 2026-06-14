# 🎬 AI Video Assistant

An AI-powered Meeting Intelligence and Video Analysis platform that transforms meeting recordings, lectures, and YouTube videos into actionable insights.

The application automatically transcribes audio, generates summaries, extracts action items, identifies key decisions, and enables users to chat with the transcript using Retrieval-Augmented Generation (RAG).

---

## 🚀 Features

* 🎥 Analyze YouTube videos or local media files
* 🎙️ Speech-to-Text transcription using Whisper and Sarvam AI
* 📝 Automatic meeting title generation
* 📋 AI-generated meeting summaries
* ✅ Action item extraction
* 🔑 Key decision extraction
* ❓ Open question identification
* 🧠 RAG-powered chatbot for transcript querying
* 🌐 Interactive Streamlit web interface

---

## 🏗️ System Architecture

```text
Video / YouTube URL
          │
          ▼
    Audio Processing
          │
          ▼
 Speech-to-Text Engine
 (Whisper / Sarvam AI)
          │
          ▼
      Transcript
          │
 ┌────────┼────────┐
 ▼        ▼        ▼
Title   Summary  Extraction
Generation        Engine
                  │
                  ├── Action Items
                  ├── Key Decisions
                  └── Open Questions
          │
          ▼
      RAG Pipeline
          │
          ▼
      ChromaDB
          │
          ▼
   Semantic Search
          │
          ▼
    Mistral LLM
          │
          ▼
      Chatbot
```

---

## 🛠️ Tech Stack

### Frontend

* Streamlit

### Backend

* Python

### AI & LLM

* Mistral AI
* LangChain

### Speech Processing

* OpenAI Whisper
* Sarvam AI

### Vector Database

* ChromaDB

### Embeddings

* HuggingFace Sentence Transformers
* all-MiniLM-L6-v2

### Audio Processing

* FFmpeg
* Pydub
* yt-dlp

---

## 📂 Project Structure

```text
AI-Video-Assistant/
│
├── app.py
├── main.py
├── requirements.txt
├── .env
│
├── core/
│   ├── transcriber.py
│   ├── summarizer.py
│   ├── extractor.py
│   ├── rag_engine.py
│   └── vector_store.py
│
├── utils/
│   └── audio_processor.py
│
├── downloads/
├── chunks/
└── vector_db/
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/AI-Video-Assistant.git
cd AI-Video-Assistant
```

### Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux / Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file:

```env
MISTRAL_API_KEY=your_mistral_api_key

SARVAM_API_KEY=your_sarvam_api_key

WHISPER_MODEL=small

SARVAM_STT_MODEL=saaras:v2.5
```

---

## ▶️ Run Streamlit Application

```bash
streamlit run app.py
```

---

## ▶️ Run CLI Version

```bash
python main.py
```

---

## 💬 Example Questions for RAG Chat

* What are the key decisions made in the meeting?
* Summarize the discussion in 5 bullet points.
* What action items were assigned?
* What deadlines were mentioned?
* Explain the main topic discussed.
* What unresolved questions remain?

---

## 📈 Future Improvements

* Speaker Diarization
* Real-Time Meeting Analysis
* Multi-Language Support
* PDF Report Export
* Cloud Deployment
* Pinecone / Weaviate Integration
* Meeting Calendar Integration

---

## 🎯 Learning Outcomes

This project demonstrates:

* Retrieval-Augmented Generation (RAG)
* Vector Databases
* Semantic Search
* Speech-to-Text Systems
* Prompt Engineering
* LangChain Pipelines
* LLM Application Development
* End-to-End AI Product Development

---

## 👨‍💻 Author

Aryan

Built as a hands-on project to explore Generative AI, LLMs, Speech Intelligence, and Retrieval-Augmented Generation.
