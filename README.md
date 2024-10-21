# PDF Insight - Conversational RAG with PDF Including Chat History

## Project Description

PDF Insight is an interactive tool designed to enhance the learning experience by enabling users to engage in a conversational interface with their PDF documents. Whether you're a student, researcher, or professional, this application allows you to upload PDFs and ask questions related to the content. The system retrieves the relevant information from the document, contextualizes the queries using chat history, and provides concise answers.

## Problem Statement

In today's fast-paced educational and professional environments, individuals often struggle to quickly extract relevant information from large documents like textbooks, research papers, and notes. Traditional methods of reading and studying are time-consuming, leading to frustration and reduced productivity. There is a need for a solution that not only provides quick and accurate answers but also makes the learning process more interactive and engaging. PDF Insight addresses this need by allowing users to chat with their documents, retrieving and summarizing key information on demand.

## Features

- Upload and interact with multiple PDF documents simultaneously.
- Ask questions about the content of the uploaded documents.
- The system retrieves and summarizes relevant information based on the user's query.
- Maintains chat history to provide context-aware responses.
- Supports Hugging Face and Groq API integration for embeddings and large language models.


PDFInsight: Conversational AI with PDF Documents (RAG-based Q&A)
PDFInsight is an AI-powered chatbot that allows users to upload PDF files and ask questions about the content. It uses a combination of Retrieval-Augmented Generation (RAG), Hugging Face Embeddings, and Groq's Large Language Model (LLM) to provide accurate, context-aware answers while maintaining a conversation history.

Features
Upload and interact with PDFs through a conversational interface.
RAG-based question-answering for retrieving relevant sections from PDFs.
Maintains context throughout the conversation using chat history.
Uses embeddings for efficient document search and retrieval.
Technology Stack
Frontend: Streamlit
NLP and AI: Hugging Face Embeddings, Groq LLM
Document Processing: PyPDFLoader
Vector Store: Chroma
Orchestration: LangChain
Installation Instructions
Prerequisites
Make sure you have the following installed:

Python 3.8+
pip (Python package installer)
Streamlit: Install via pip install streamlit
Chroma: Install via pip install chromadb
LangChain: Install via pip install langchain
PyPDFLoader: Install via pip install pypdfloader
Hugging Face: Install via pip install huggingface-hub
dotenv: Install via pip install python-dotenv
You will also need API keys for:

Hugging Face (for embeddings)
Groq (for LLM)
Step 1: Clone the Repository
bash
Copy code
git clone https://github.com/yourusername/pdf-insight-chatbot.git
cd pdf-insight-chatbot
Step 2: Install Dependencies
bash
Copy code
pip install -r requirements.txt
Step 3: Set Up Environment Variables
Create a .env file in the root directory and add your Hugging Face and Groq API keys:

env
Copy code
HF_TOKEN=your_huggingface_api_key
GROQ_API_KEY=your_groq_api_key
Step 4: Run the Application
To start the chatbot, run the following command:

bash
Copy code
streamlit run app.py
Step 5: Use the Chatbot
Open your browser and go to http://localhost:8501.
Upload one or more PDF files using the file uploader.
Enter your Hugging Face and Groq API keys in the sidebar.
Start asking questions about the PDF content!
Project Structure
bash
Copy code
pdf-insight-chatbot/
│
├── app.py                  # Main Streamlit app script
├── requirements.txt         # Required Python packages
├── .env                     # Environment variables (Hugging Face & Groq API keys)
├── README.md                # Project documentation
└── temp.pdf                 # Temporary file for uploaded PDFs (auto-generated)
Key Components
PDF Upload & Processing:
Upload PDFs and extract content using PyPDFLoader.
Embeddings & Vector Store:
Create document embeddings with Hugging Face's all-MiniLM-L6-v2 model.
Store embeddings in the Chroma vector store for efficient retrieval.
Conversational Q&A:
Uses LangChain to create a conversational interface and maintain chat history.
Integrates Groq's LLM (Gemma2-9b-It) for context-aware answers.
Session Management:
Streamlit’s session state is used to store and manage the chat history, ensuring seamless multi-turn conversations.
Future Enhancements
Add support for additional file formats (e.g., Word, Excel).
Implement advanced visualization of PDF content (e.g., highlighting text references).
Integrate more LLMs and improve the response generation with further fine-tuning.
