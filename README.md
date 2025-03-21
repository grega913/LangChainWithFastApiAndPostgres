# Langchain-FastAPI Integration

https://www.youtube.com/watch?v=Arf7UwWjGyc&ab_channel=CodingCrashCourses

## Overview

This project integrates Langchain with FastAPI, providing a framework for document indexing and retrieval, as well as chat functionality, using PostgreSQL and pgvector. It is designed to support both synchronous and asynchronous operations.

## Features

- **Document Management**: Methods for adding, retrieving, and deleting documents.
- **Vector Store**: Utilizes Langchain's vector store for efficient document retrieval.
- **Chat Functionality**: Includes a chat endpoint that leverages Langchain for response generation.
- **Asynchronous Support**: Offers async operations for enhanced performance.

## Configuration

Ensure to set environment variables such as `POSTGRES_DB`, `POSTGRES_USER`, `POSTGRES_PASSWORD`, `DB_HOST`, `DB_PORT`, and `OPENAI_API_KEY`. Configure the database connection string appropriately and initialize Langchain and OpenAI embeddings according to project needs.

## How to run

1. docker compose up - this will start postgres db within docker container - check running postgres with pgAdmin
2. create venv if not exists and install dependencies - pip install -r requirements.txt
3. activate virtual environment
4. uvicorn main:app --port 8000 - start fastapi with uvicorn - add some records on add route on 127.0.0.1:8000/docs
5. python myrequests.py - this will test langchain chat
