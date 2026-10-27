# 📄 RAG Document Chatbot

An AI-powered chatbot that answers questions from uploaded PDF documents using Retrieval-Augmented Generation (RAG).

## 🚀 Features

- Upload PDF documents and ask questions about their content.
- Extract and split PDF text into chunks.
- Generate text embeddings using Sentence Transformers.
- Retrieve relevant information using FAISS similarity search.
- Generate context-aware answers using the Groq API.
- Interactive interface built with Streamlit.

## 🛠️ Tech Stack

- Python
- Streamlit
- Sentence Transformers
- FAISS
- Groq API
- PDF text extraction library

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/lifnasnowlin-ui/RAG-document-Chatbot.git
cd RAG-document-Chatbot
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the project root directory and add:

```env
GROQ_API_KEY=your_groq_api_key
GROQ_MODEL=openai/gpt-oss-20b
```

Replace the placeholder values with your own Groq API key and a model supported by your account.

**Security:** Never upload your `.env` file or share your API key publicly.

### 5. Run the application

```bash
streamlit run app.py
```

Open the local URL shown in the terminal to use the chatbot.

## 🔍 How It Works

1. Upload a PDF document.
2. Extract the text from the PDF.
3. Split the text into smaller chunks.
4. Convert the chunks into embeddings.
5. Use FAISS to retrieve relevant chunks for a question.
6. Send the retrieved context to the Groq language model to generate an answer.

## 📂 Project Structure

```text
RAG-document-Chatbot/
├── app.py
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

## 🔮 Future Improvements

- Support multiple PDF documents.
- Display source references for answers.
- Add chat history.
- Deploy the application online.

## 👩‍💻 Author

**Lifna Snowlin**

GitHub: https://github.com/lifnasnowlin-ui

---

Built with Python, Streamlit, FAISS, Sentence Transformers, and Groq.
