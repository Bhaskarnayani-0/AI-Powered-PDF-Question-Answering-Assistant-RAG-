# AI-Powered-PDF-Question-Answering-Assistant-RAG-
# PDF-QA-RAG

AI-Powered PDF Question-Answering (RAG) — demo using LangChain + OpenAI + FAISS.

## What it does
- Upload PDF
- Extract text → chunk → embed → index
- Answer user queries using retrieved context + OpenAI LLM

## Quickstart (Colab)
1. Open the provided Colab notebook.
2. Install dependencies (first cell).
3. Upload a PDF to /content/sample.pdf or modify path.
4. Set OPENAI_API_KEY.
5. Run the indexing cell, then run queries.

## Local (Streamlit)
1. pip install -r requirements.txt
2. export OPENAI_API_KEY="sk-..."
3. streamlit run app.py
4. Open browser, upload PDF, ask questions.

## Files
- colab_rag_pdf_qa.ipynb  -> Colab demo
- app.py                 -> Streamlit UI
- README.md

## Notes
- Add OCR if PDFs are scanned images.
- Persist FAISS index for production use.
pdf-qa-rag/
├─ README.md
├─ app.py
├─ requirements.txt
├─ colab_rag_pdf_qa.ipynb
├─ LICENSE
└─ assets/
   └─ sample.pdf
langchain
openai
faiss-cpu
pypdf
tiktoken
streamlit

