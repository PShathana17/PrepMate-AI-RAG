# PrepMate AI — RAG-Based Interview Preparation Assistant

## Overview

PrepMate AI is a Retrieval-Augmented Generation (RAG) project designed to help students prepare for technical interviews. It retrieves relevant information from interview preparation PDFs and uses Large Language Models (LLMs) to generate simple, context-based answers.

The project focuses on Python, Machine Learning, Deep Learning, and Natural Language Processing (NLP).

## Key Features

- **PDF Question Answering:** Retrieves information from technical interview preparation documents.
- **Semantic Search:** Finds relevant content using sentence embeddings and FAISS.
- **Context-Aware Responses:** Generates answers using retrieved document content.
- **Multiple LLMs:** Experiments with FLAN-T5, TinyLlama through Hugging Face Transformers, and TinyLlama GGUF through llama.cpp.
- **Answer Evaluation:** Explores factual correctness and groundedness using a reference-answer-based evaluation approach.
- **Beginner-Friendly Answers:** Aims to provide clear and easy-to-understand technical explanations.

## Technologies Used

- Python
- Hugging Face Transformers
- Sentence Transformers
- FAISS
- FLAN-T5
- TinyLlama
- llama.cpp
- PyPDF
- Google Colab

##

## Architecture

User Question → FAISS Retriever → Relevant PDF Chunks → Prompt Construction → LLM → Generated Answer

## Model Experiments

The notebook explores three model configurations:

- FLAN-T5 Base
- TinyLlama 1.1B Chat using Hugging Face Transformers
- TinyLlama 1.1B Chat in GGUF format using llama.cpp

The experiments help explore how different model configurations generate answers from retrieved context.

## Evaluation

- Compared different language model configurations based on their generated responses.
- Examined answer relevance and how well responses align with the retrieved document context.
- Explored the ability of LLMs to generate useful answers for technical interview preparation.
