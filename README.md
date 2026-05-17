# 🏥 Health Assistant RAG

A **Retrieval-Augmented Generation (RAG)** powered health assistant that analyzes patient medical records and provides intelligent health insights by connecting current symptoms to historical medical data.

## 🎯 Project Overview

Health Assistant RAG is an AI-powered medical document analysis system that:
- **Processes** patient medical records (PDFs)
- **Creates vector embeddings** for semantic search
- **Retrieves** relevant historical medical information
- **Generates** contextual health insights using Google Gemini AI

The system combines LangChain, Pinecone vector databases, and Google's Generative AI to provide intelligent medical consultations based on patient history.

## ✨ Key Features

- 📄 **PDF Document Processing**: Extract and analyze medical PDFs with automatic text chunking
- 🔍 **Semantic Search**: Find relevant medical information using vector embeddings
- 🧠 **AI-Powered Insights**: Generate context-aware health analysis using Gemini AI
- 👨‍⚕️ **Multi-Patient Support**: Manage and query data for multiple patients
- 🎨 **Interactive UI**: User-friendly Streamlit interface for easy access
- 🔐 **Secure Configuration**: Environment-based API key management

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Frontend** | Streamlit, Streamlit PDF Viewer |
| **Vector Database** | Pinecone |
| **Embeddings** | Google Gemini (embedding-001) |
| **LLM** | Google Gemini 2.5 Pro |
| **Document Processing** | PyMuPDF (fitz) |
| **Framework** | LangChain with Google GenAI |
| **Language** | Python 3.8+ |

## 📋 Prerequisites

- Python 3.8 or higher
- [Pinecone API Key](https://www.pinecone.io/)
- [Google API Key](https://aistudio.google.com/app/apikey) (with Gemini access)
- PDF medical documents

## 🚀 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Utkrisha-kandel/Health-Assistant-RAG-.git
cd Health-Assistant-RAG-
