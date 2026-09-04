# 🤖 AI Customer Support Agent

An AI-powered customer support workflow built using *n8n*. The agent can understand customer queries, maintain conversation context, search customer order details, and retrieve relevant information from a knowledge base using RAG.

## 📸 Workflow Preview

![AI Customer Support Agent Workflow](workflow(AI-Customer-Support).png)

## 🚀 Features

- 💬 AI-powered customer conversations
- 🧠 Conversation memory for maintaining context
- 📦 Customer order lookup using Airtable
- 🔎 Knowledge-base search using Pinecone
- 📚 RAG-based information retrieval
- 🤖 Groq LLM for generating responses
- 🔤 Hugging Face embeddings for vector search

## 🏗️ Workflow

```text
Customer Message
       ↓
   Chat Trigger
       ↓
    AI Agent
    ↙  ↓  ↘
Memory  │   Tools
        │    ↙  ↘
      Groq  Airtable  Pinecone
                  Orders   Knowledge Base
                              ↓
                     Hugging Face Embeddings
