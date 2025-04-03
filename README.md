#  Summarization and Query Answering System

This project involves building an end-to-end system for summarizing academic papers from the Arxiv dataset and answering questions based on the generated summaries. It includes the following key components:

## Features
- **Data Preprocessing**: Load and preprocess the Arxiv summarization dataset using Hugging Face's `datasets` library.
- **Model Fine-Tuning**: Fine-tune the `T5-small` model for abstractive summarization.
- **PDF Text Extraction**: Extract text from PDFs using `pdfplumber` and preprocess it for summarization.
- **Summarization Pipeline**: Generate summaries from text chunks using a fine-tuned T5 model.
- **Semantic Search**: Use FAISS to index and retrieve relevant summaries based on a query.
- **Interactive Query Answering**: Use OpenAI's GPT-3.5 to generate answers based on retrieved summaries.

## Installation

### Requirements
To run this project, you'll need the following libraries:

```bash
pip install datasets transformers pdfplumber sentence-transformers faiss-cpu openai spacy
```
Make sure to install the spaCy model:

```bash
Copy
python -m spacy download en_core_web_sm
