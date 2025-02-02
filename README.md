# PDF Insight - Conversational RAG with PDF Including Chat History

## Project Description

PDFInsight is an AI chatbot designed to allow users to upload PDF documents and ask questions about the content. It uses Retrieval-Augmented Generation (RAG) for dynamic and context-aware question answering, integrating chat history for more natural interactions. The project leverages **Hugging Face Embeddings**, **Groq LLM**, and **Chroma Vector Store** for enhanced document retrieval and response generation.
## Problem Statement

In today's fast-paced educational and professional environments, individuals often struggle to quickly extract relevant information from large documents like textbooks, research papers, and notes. Traditional methods of reading and studying are time-consuming, leading to frustration and reduced productivity. There is a need for a solution that not only provides quick and accurate answers but also makes the learning process more interactive and engaging. PDF Insight addresses this need by allowing users to chat with their documents, retrieving and summarizing key information on demand.


# **PDFInsight: Conversational AI with PDF Documents (RAG Q&A)**



## **Key Features**
- **Upload PDF Files**: Load multiple PDFs and interact with them via a conversational interface.
- **Context-Aware Q&A**: The system uses the chat history to maintain the context of questions asked.
- **Efficient Search**: Combines document chunking, embeddings, and a retrieval system for precise information extraction.

## **Technology Stack**
- **Frontend**: [Streamlit](https://streamlit.io/)
- **NLP and AI**: [Hugging Face Embeddings](https://huggingface.co/), [Groq LLM](https://groq.com/)
- **Document Processing**: [PyPDFLoader](https://pypi.org/project/pypdfloader/)
- **Vector Store**: [Chroma](https://docs.trychroma.com/)
- **Orchestration**: [LangChain](https://langchain.com/)

## **Installation Instructions**

### **Prerequisites**
Make sure you have the following installed:
- **Python 3.8+**
- **pip** (Python package installer)

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/yourusername/pdf-insight-chatbot.git
cd pdf-insight-chatbot
```
### **Step 2: Install Dependencies**


```bash
pip install streamlit langchain chromadb huggingface-hub pypdfloader python-dotenv
```
### **Step 3: Set Up Environment Variables**
```bash
HF_TOKEN=your_huggingface_api_key
GROQ_API_KEY=your_groq_api_key
```
## **Step 4: Run the Application**

To start the chatbot, run the following command:

## **Step 5: Use the Chatbot**

- Open your browser and go to http://localhost:8501.
- Upload one or more PDF files using the file uploader.
- Enter your Hugging Face and Groq API keys in the sidebar.
- Start asking questions about the PDF content!
### **Project Structure**
      
      pdf-insight-chatbot/
      │
      ├── app.py                  # Main Streamlit app script
      ├── requirements.txt         # Required Python packages
      ├── .env                     # Environment variables (Hugging Face & Groq API keys)
      ├── README.md                # Project documentation
      └── temp.pdf                 # Temporary file for uploaded PDFs (auto-generated)



### Explanation of Sections:
- **Project Title and Description**: Provides a brief overview of what the project does.
- **Key Features**: Lists the main features of your application.
- **Technology Stack**: Details the technologies used in the project.
- **Installation Instructions**: Step-by-step guide on how to set up the project locally.
- **Project Structure**: Explains the structure of the project and its files.
- **Code Overview**: Includes the main application code (`app.py`) with syntax highlighting.
- **Future Enhancements**: Lists potential improvements for the project.
- **Contributing**: Guidelines for others who wish to contribute to the project.
- **License**: Specifies the licensing for the project.
