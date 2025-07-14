# 🤖 Chatbot OpenAI with Streamlit

This project implements a chatbot interface using the OpenAI API, built with the Streamlit framework. It allows users to interact with OpenAI models in a chat-style environment, manage multiple conversation sessions, and securely store API keys and conversations locally.

## 📌 Features

### 🧠 OpenAI Integration
- Supports GPT-3.5-turbo and GPT-4 models.
- Real-time responses using streaming API.
- Simple interface with `st.chat_message`.

### 💬 Conversation Management
- Users can create, load, and switch between multiple conversation threads.
- Messages are saved locally using Python's `pickle` module.
- Custom filenames are automatically generated from the first user message.

### 🔐 API Key Storage
- Secure local storage of the user's OpenAI API key.
- Simple configuration interface via the sidebar.

### 🧱 Modular Architecture
- `projeto_finalizado.py`: Main interface logic with Streamlit UI.
- `utils_openai.py`: Handles connection to the OpenAI API.
- `utils_files.py`: Manages saving/loading conversations and API keys.

## 🚀 How to Run

```bash
pip install streamlit openai unidecode
streamlit run projeto_finalizado.py
```

## 🗂️ Folder Structure

```
📁 chatbot-openai-streamlit
├── projeto_finalizado.py        # Main Streamlit app
├── utils_openai.py              # OpenAI response handler
├── utils_files.py               # File and API key management
├── configuracoes/               # Stores the API key locally
└── mensagens/                   # Stores serialized conversations
```

## ✅ Requirements

- Python 3.8+
- OpenAI API Key
- Streamlit
- Unidecode

## 📌 Notes

- Ensure your OpenAI API key is added in the "Configurations" tab.
- All conversation data is stored locally; no cloud storage is used.
- The assistant response supports real-time streaming.

## 🧪 Example Use

1. Launch the app.
2. Input your API key in the "Configurations" tab.
3. Start chatting and your messages will be saved under "Conversations".
4. Return to past chats anytime.

---
