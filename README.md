# 🚀 LangChain Groq Chatbot

A beginner-friendly conversational AI chatbot built using **Python, LangChain, Groq LLM APIs, and Streamlit**.

This project demonstrates how to integrate Large Language Models (LLMs) into a Python application using LangChain's prompt templates and LCEL (LangChain Expression Language), with streaming responses through an interactive Streamlit interface.

## 📌 Project Overview

This application allows users to interact with a Groq-powered LLM through a simple conversational interface.

Users can enter their Groq API key, select an available model, ask questions, and receive responses in real time.

The project was developed to understand the fundamentals of LangChain and LLM application development.

## ✨ Features

- Interactive chatbot interface using Streamlit.
- Integration with Groq LLM APIs.
- Support for selecting between available Groq models.
- Prompt engineering using LangChain ChatPromptTemplate.
- LCEL pipeline using prompt templates, ChatGroq, and StrOutputParser.
- Streaming LLM responses.
- Basic conversation history display using Streamlit session state.
- Clear chat functionality.
- Basic exception handling for API errors.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| LangChain | LLM application framework |
| Groq API | LLM inference |
| ChatGroq | Groq model integration |
| Streamlit | Interactive chatbot interface |
| LCEL | Building the LLM processing chain |

## 🏗️ Application Architecture

The application follows this workflow:

```text
User
  |
  v
Streamlit Chat Interface
  |
  v
Groq API Key & Model Selection
  |
  v
ChatPromptTemplate
  |
  v
LangChain LCEL Pipeline
  |
  v
ChatGroq LLM
  |
  v
StrOutputParser
  |
  v
Streaming Response
  |
  v
Streamlit Chat Interface
```

## 📂 Project Structure

```text
langchain-groq-chatbot/
│
├── qachatbot.py
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   ├── langchainbasics.ipynb
│   └── tools.ipynb
│
└── screenshots/
    └── chatbot.png
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/Kavita6398/langchain-groq-chatbot.git
```

### 2. Navigate to the project directory

```bash
cd langchain-groq-chatbot
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Get your Groq API key

Visit:

https://console.groq.com/keys

Generate an API key.

Do not share or upload your API key publicly.

### 6. Run the application

```bash
streamlit run qachatbot.py
```

### 7. Start chatting

- Enter your Groq API key in the sidebar.
- Select an available Groq model.
- Enter your question in the chat input.
- Receive a streamed response.

## 🧠 LangChain Concepts Demonstrated

This project helped me understand the following concepts:

- LLM integration using ChatGroq.
- Prompt templates using ChatPromptTemplate.
- LangChain Expression Language (LCEL).
- Chaining components using the pipe operator.
- Output parsing using StrOutputParser.
- Streaming responses from LLMs.
- Basic chat interface and session state management.

## 📚 Learning Resources

- [LangChain Documentation](https://python.langchain.com/docs/introduction/)
- [Groq Documentation](https://console.groq.com/docs)
- [Streamlit Documentation](https://docs.streamlit.io/)

## 🔮 Future Improvements

- Implement proper conversational memory so previous messages are included in model requests.
- Add document ingestion and Retrieval-Augmented Generation (RAG).
- Integrate ChromaDB for vector storage.
- Implement LangGraph-based agent workflows and tool calling.
- Add automated tests and improved error handling.
- Improve security and API key management.

## ⚠️ Current Limitations

- The current application is a basic LLM chatbot, not a RAG application.
- Previous messages are displayed in the interface but are not passed to the LLM as conversation context.
- No vector database or document retrieval pipeline is implemented.
- No agent or tool execution workflow is implemented.

## 👩‍💻 Author

**Kavita Gupta**

Software Developer | Exploring Generative AI, Agentic AI, RAG, and LLM Engineering.

- GitHub: [Kavita6398](https://github.com/Kavita6398)

---

⭐ If you find this project useful, feel free to explore the repository and learn from it.