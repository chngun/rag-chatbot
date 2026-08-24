# 📚 RAG-based AI Chatbot

Ollama + LangChain ашигласан үнэгүй хичээлийн материалын Q&A чатбот.

## ✨ Features
- 📄 PDF-ээс мэдээлэл татан хэрэглэлт (RAG)
- 🤖 Ollama mistral LLM (үнэгүй, local)
- 🔢 Nomic-embed-text embedding model
- 💾 ChromaDB vector database
- 🎨 Streamlit интерфейс

## 🛠️ Tech Stack
- **Language:** Python 3.10
- **Framework:** LangChain, Streamlit
- **LLM:** Ollama (mistral)
- **Vector DB:** ChromaDB
- **Embedding:** Nomic-embed-text

## 🚀 How to Run (Local)

### Prerequisites
- Python 3.10+
- Ollama installed ([ollama.ai](https://ollama.ai))

### Setup

```bash
# Clone repo
git clone https://github.com/chngun/rag-chatbot.git
cd rag-chatbot

# Create virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

### Run

**Terminal 1 - Start Ollama server:**
```bash
ollama serve
```

**Terminal 2 - Start Streamlit app:**
```bash
cd ~/Documents/rag-project
source venv/bin/activate
streamlit run main.py
```

Open browser: `http://localhost:8501`

## 📝 How It Works

1. **PDF Loading:** PyPDF2 ашиглан PDF-ээс текст унших
2. **Chunking:** RecursiveCharacterTextSplitter (500 tokens)
3. **Embedding:** Nomic-embed-text model ашигладаг
4. **Retrieval:** ChromaDB дээр top-3 chunk авах
5. **Generation:** Mistral LLM хариулт үүсгэнэ

## 📊 Project Structure
## ⚠️ Important Notes

- **Local Development Only:** Ollama сервер таны компьютэр дээр ажиллах ёстой
- **First Run:** Embedding үүсгэхэд 2-3 минут цаг зарцуулж болно
- **Model Size:** Mistral + Nomic models ~5GB нийт

## 🎓 Learning Outcomes

- RAG (Retrieval-Augmented Generation) pipeline сүүлүүлэх
- Vector embeddings ойлгох
- LLM-г local дээр ашиглах
- Streamlit UI хийх

## 🔗 Links

- **GitHub:** [github.com/chngun/rag-chatbot](https://github.com/chngun/rag-chatbot)
- **Ollama:** [ollama.ai](https://ollama.ai)
- **LangChain:** [langchain.com](https://langchain.com)

## 📸 Demo

[Screenshot авч оруулах боломж]

---

**Created by:** Chngun  
**Date:** August 2026
