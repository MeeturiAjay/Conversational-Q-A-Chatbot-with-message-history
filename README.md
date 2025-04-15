# Conversational Q&A Chatbot with Message History

A smart, context-aware conversational chatbot built using LangChain, Groq, and HuggingFace that answers questions based on a PDF document. It maintains chat history to provide context-aware answers.

---

## 🧠 Features

- 🔎 PDF-based Q&A: Upload a PDF and ask questions from its content.
- 🧩 LLM Powered: Uses LLaMA-4 via Groq for powerful language understanding.
- 📚 Vector Search: Utilizes ChromaDB with HuggingFace embeddings for semantic search.
- 💬 Chat History Aware: Remembers past questions to provide more accurate responses.
- ⚡ Fast & Efficient: Light and easy to run locally.

---

## 🛠️ Tech Stack

- **LangChain** - For chaining LLMs with retrievers
- **Groq API** - To access Meta LLaMA-4 model
- **HuggingFace Embeddings** - For vectorizing document chunks
- **ChromaDB** - As the vector store
- **PyPDFLoader** - To extract text from PDFs
- **Python** - Core scripting language
- **VS Code** - Recommended editor

---


## 🚀 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/MeeturiAjay/Conversational-Q-A-Chatbot-with-message-history.git
cd Conversational-Q-A-Chatbot-with-message-history
```

### 2. Create & Activate a Virtual Environment
```
python -m venv .venv
source .venv/bin/activate         # Linux/macOS
.venv\Scripts\activate            # Windows

```

### 3. Install Dependencies
```
pip install -r requirements.txt
```

### 4. Set API Keys
Create a .env file in the root folder and add your API keys:
```
GROQ_API_KEY=your_groq_api_key
HUGGINGFACE_API_KEY=your_huggingface_api_key
```

### 5. Run the Project
```
python main.py
```

---

## 🧠 How It Works

- PDF is loaded and split into chunks.
- Chunks are embedded using HuggingFace and stored in ChromaDB.
- User questions are passed to the retriever.
- Retriever fetches relevant chunks based on the query.
- Groq’s LLaMA-4 model answers using the retrieved context and chat history.

---

## 🙋‍♂️ Author
### Meeturi Ajay Kumar
Connect with me on 
- ![LinkedIn](https://www.linkedin.com/in/meeturi-ajay-kumar-a02743248/)
- meeturiajaykumar.23@gmail.com