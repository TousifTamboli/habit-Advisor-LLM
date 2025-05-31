# Life Advice LLM — Personalized Habit Coaching with Atomic Habits

## Project Overview

This project builds a Local Language Model (LLM) that provides life advice based on the book *Atomic Habits* by James Clear.  
It processes the book text, creates embeddings for meaningful chunks, and uses a similarity search to retrieve relevant content for any user query.  
The retrieved context and user prompt are fed into a GPT-2 model (or similar) running locally, which generates personalized, helpful advice on habits and self-improvement topics.

---

## Features

- Text chunking and embedding generation from the *Atomic Habits* book  
- Vector similarity search to retrieve relevant advice snippets  
- Local GPT-2 language model for generating context-aware advice  
- Supports querying with natural language prompts  
- Works completely offline (no external API required)  
- Easy to extend with fine-tuning and improved models  

---

## Requirements

- Python 3.8 or higher  
- [transformers](https://huggingface.co/transformers/)  
- [sentence-transformers](https://www.sbert.net/)  
- [faiss](https://github.com/facebookresearch/faiss) (for vector similarity search)  
- torch (PyTorch)  

Install dependencies (recommended inside a virtual environment):

```bash
pip install torch transformers sentence-transformers faiss-cpu certifi
