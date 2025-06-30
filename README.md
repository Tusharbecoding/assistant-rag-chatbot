# Assistant RAG ChatBot (Shop assistant)

A Retrieval-Augmented Generation (RAG) powered chatbot that acts as a smart assistant for your shop or product catalog. This application integrates LangChain, Pinecone, and Google Gemini to build a real-world, production-ready AI chatbot that understands user queries based on your own data.

---

## 📌 Features

- 🔍 Contextual question-answering based on shop product data
- 🧠 Embedding generation using Google Gemini
- 📦 Vector storage and retrieval using Pinecone
- 💬 Natural language responses via Large Language Model (LLM)
- 🌐 Streamlit web interface for user interaction

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Tusharbecoding/assistant-rag-chatbot
cd assistant-rag-chatbot
```

### 2. Setup Python Environment

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory:

```env
GOOGLE_API_KEY=your_google_api_key
PINECONE_API_KEY=your_pinecone_api_key
DB_PASSWORD=your_mysql_password
```

### 4. Ingest Data

Run the MySQL ingestion script:

```bash
python data_ingestion.py
```

Then sync data to Pinecone:

```bash
python sync_pinecone.py
```

### 5. Launch Streamlit App

```bash
streamlit run app.py
```

---

## 📊 Technologies Used

- **LangChain** – RAG orchestration
- **Pinecone** – Vector database
- **Google Gemini API** – Embedding and LLM
- **Streamlit** – UI for chatbot
- **MySQL** – Product catalog storage
