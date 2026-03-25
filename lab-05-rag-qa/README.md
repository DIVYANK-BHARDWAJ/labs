# Lab 05: RAG Q&A 📚

**Points: 20 | Time: ~1-2 hours**

## Problem
Build a minimal RAG system: given a "knowledge base" (a list of text chunks) and a question, retrieve the most relevant chunk and answer the question based only on it.

## Your Task
Implement the functions in `solution.py`. No vector DB or LLM call is needed — use keyword/word-overlap matching as a simple retrieval proxy.

## Requirements
- `retrieve(chunks, question)` → returns the single chunk (string) with the most word overlap with the question
- `answer(chunks, question)` → returns a dict `{"context": <chunk>, "answer": <string>}` where `answer` is any non-empty string derived from the context
