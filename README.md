# Vertex AI RAG Agent with ADK

This repository contains a Google Agent Development Kit (ADK) implementation of a Retrieval Augmented Generation (RAG) agent using Google Cloud Vertex AI.

## Overview

The Vertex AI RAG Agent allows you to:

- Query document corpora with natural language questions
- List available document corpora
- Create new document corpora
- Add new documents to existing corpora
- Get detailed information about specific corpora
- Delete corpora when they're no longer needed

## Prerequisites

- A Google Cloud account
- A Google Cloud project with the Vertex AI API enabled
- Appropriate access to create and manage Vertex AI resources
- Python 3.9+ environment


## Installation

1. **Set up a virtual environment**:
   ```bash
   python -m venv .venv
   source .venv/bin/activate 
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Using the Agent

The agent provides the following functionality through its tools:

### 1. Query Documents
Allows you to ask questions and get answers from your document corpus:
- Automatically retrieves relevant information from the specified corpus
- Generates informative responses based on the retrieved content

### 2. List Corpora
Shows all available document corpora in your project:
- Displays corpus names and basic information
- Helps you understand what data collections are available

### 3. Create Corpus
Create a new empty document corpus:
- Specify a custom name for your corpus
- Sets up the corpus with recommended embedding model configuration
- Prepares the corpus for document ingestion

### 4. Add New Data
Add documents to existing corpora or create new ones:
- Supports Google Drive URLs and GCS (Google Cloud Storage) paths
- Automatically creates new corpora if they don't exist

### 5. Get Corpus Information
Provides detailed information about a specific corpus:
- Shows document count, file metadata, and creation time
- Useful for understanding corpus contents and structure

### 6. Delete Corpus
Removes corpora that are no longer needed:
- Requires confirmation to prevent accidental deletion
- Permanently removes the corpus and all associated files

## Resources

- [Vertex AI RAG Documentation](https://cloud.google.com/vertex-ai/generative-ai/docs/rag-overview)
- [Google Agent Development Kit (ADK) Documentation](https://github.com/google/agents-framework)
- [Google Cloud Authentication Guide](https://cloud.google.com/docs/authentication)
