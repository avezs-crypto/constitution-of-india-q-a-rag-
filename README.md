# 📜 Constitution of India – RAG Q&A Chatbot

A **Retrieval-Augmented Generation (RAG)** based chatbot that answers questions about the **Constitution of India** in simple, easy-to-understand language.

The system retrieves relevant constitutional text using vector search and generates accurate answers using a large language model.

---

## 🚀 Features

- 🔍 Semantic search over Constitution of India documents
- 🧠 Retrieval-Augmented Generation (RAG)
- 📚 Source-backed answers (view retrieved sections)
- 💬 Chat-style interface using Streamlit
- ⚡ Fast responses powered by Groq LLaMA 3.3
- 🧩 Modular and extendable architecture

---

## 🏗️ Tech Stack

- **Frontend**: Streamlit  
- **LLM**: LLaMA 3.3 (Groq)  
- **Embeddings**: HuggingFace `all-MiniLM-L6-v2`  
- **Vector Database**: FAISS  
- **Framework**: LangChain  

---

## 📂 Project Structure

.
├── app.py # Streamlit application
├── index.faiss # FAISS vector index
├── index.pkl # FAISS metadata
├── requirements.txt # Python dependencies
├── README.md # Project documentation
├── .env.example # Environment variable template
├── .gitignore


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/constitution-rag-chatbot.git
cd constitution-rag-chatbot
2️⃣ Create a virtual environment (recommended)
bash

python -m venv venv
source venv/bin/activate      # Linux / macOS
venv\Scripts\activate         # Windows
3️⃣ Install dependencies

pip install -r requirements.txt
4️⃣ Set environment variables
Create a .env file or export environment variables:

GROQ_API_KEY=your_groq_api_key
For Streamlit Cloud, add this under Secrets.

▶️ Run the Application
bash

streamlit run app.py
Then open:

arduino

http://localhost:8501
🧠 How the RAG Pipeline Works
User question is converted into embeddings

FAISS retrieves the most relevant constitutional sections

Retrieved context is injected into the LLM prompt

LLM generates a grounded, concise answer

🔐 Environment Variables
Variable	Description
GROQ_API_KEY	API key for Groq LLM

⚠️ Disclaimer
This project is for educational purposes only and does not constitute legal advice.
Always consult a qualified legal professional for official interpretations.

🛣️ Future Enhancements
Article-wise citation (Article numbers)

Multilingual support

Upload custom legal documents

Improved UI and analytics

Answer confidence scoring

🙌 Acknowledgements
Streamlit

LangChain

HuggingFace

FAISS

Groq

⭐ Support
If you find this project useful, please consider giving it a ⭐ on GitHub.
