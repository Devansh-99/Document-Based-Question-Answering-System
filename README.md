Document Based Question Answering

This project implements a document-based question answering system using LangChain. It loads a PDF document, splits the extracted content into smaller chunks, converts the chunks into embeddings using OpenAI embeddings, stores them in ChromaDB, and uses a vector-based QA chain to answer questions from the document.

Features

PDF document loading

Document text extraction

Text chunking

OpenAI embeddings

ChromaDB vector search

Context-based question answering

Tech Stack

Python

LangChain

OpenAI

ChromaDB

Tiktoken

Unstructured

NLTK

Google Colab

How It Works

The PDF is loaded using UnstructuredFileLoader.

The extracted document is divided into chunks using CharacterTextSplitter with a chunk size of 800.

OpenAI embeddings are generated for the document chunks.

The embeddings are stored in ChromaDB for similarity-based retrieval.

A VectorDBQA chain uses OpenAI to retrieve relevant document content and generate an answer to the user's question.

Example

The project uses a TCS-NQT aptitude PDF as the input document and allows the user to ask questions based on its content.
