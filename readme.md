# 🩺 Medical Chatbot

A Medical Chatbot application that uses **Natural Language Processing (NLP)** and **Semantic Search** to provide intelligent and context-aware responses to medical-related queries. The system integrates a pretrained language model with a vector database and serves responses through a Flask-based web interface.

---

## 🚀 Features

- Interactive medical chatbot UI
- Semantic search using vector embeddings
- Context-aware and relevant medical responses
- Flask-based backend API
- Scalable architecture for adding more data or models

---

## 🧰 Tech Stack

### 🐍 Python
Python is the core programming language used for backend logic, machine learning integration, and data processing. It provides rich libraries for AI/ML and easy web integration.

### 🌐 Flask
Flask is a lightweight web framework used to:
- Handle HTTP requests
- Serve the chatbot interface
- Connect frontend with the AI backend

### 🤗 Hugging Face Transformers
Used to load pretrained language models that:
- Understand medical queries
- Generate natural language responses

### 🧠 Sentence Transformers
Converts text into vector embeddings to enable semantic understanding of queries and documents.

### 📦 FAISS (or Pinecone)
A vector database used for:
- Storing document embeddings
- Performing fast similarity search
- Retrieving relevant medical context

### 🎨 HTML / CSS
Used to build the chatbot frontend interface for user interaction.

### 📊 Jupyter Notebook
Used for experimentation, testing embeddings, model behavior, and research during development.

---

## ⚙️ How the System Works

1. User enters a medical query in the chatbot UI
2. Flask backend receives the request
3. Query is converted into vector embeddings
4. FAISS searches for the most relevant medical data
5. Retrieved context is passed to the language model
6. Model generates a response
7. Flask returns the response to the frontend


medical_chatbot/
│

├── app.py # Flask application

├── store_index.py # Vector index creation

├── data/ # Medical documents

├── faiss_index/ # Stored vector index

├── templates/ # HTML files

├── static/ # CSS & assets

├── research/ # Experiments & notes

├── implementation_of_chatbot.ipynb

├── requirements.txt

└── setup.py