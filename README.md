# Health Assistant RAG

A health assistant that reads patient medical records and answers questions about them. Upload PDFs, ask about symptoms or history, and get responses grounded in the actual documents.

---

## What it does

You upload a patient's medical records as PDFs. The app chunks and embeds them into a Pinecone vector database. When you ask a question, it pulls the relevant sections and sends them to Gemini to generate a response — so answers are always tied to real document content, not hallucinated.

---

## Stack

- **Streamlit** — UI
- **Pinecone** — vector database
- **Google Gemini 2.5 Pro** — LLM
- **Gemini embeddings** — document embedding
- **LangChain** — RAG pipeline
- **PyMuPDF** — PDF parsing

---

## Setup

```bash
git clone https://github.com/Utkrisha-kandel/Health-Assistant-RAG-.git
cd Health-Assistant-RAG-
pip install -r requirements.txt
```

Create a `.env` file:
Then:

```bash
# First, embed your documents
python create_vector.py

# Then run the app
streamlit run frontend.py
```

---

## How it works

1. `create_vector.py` reads PDFs from the `/documents` folder, chunks the text, and stores embeddings in Pinecone
2. `frontend.py` takes a user query, retrieves the most relevant chunks, and passes them to Gemini to generate an answerSonnet 4.6