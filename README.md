# Linux RAG Assistant

A simple Retrieval-Augmented Generation (RAG) application that answers Linux-related questions using a custom Linux knowledge base.

## Features

- Answers questions related to the Linux operating system.
- Retrieves relevant information using semantic vector search.
- Splits large documents into smaller chunks.
- Generates vector embeddings using SentenceTransformers.
- Stores and searches embeddings using Qdrant Cloud.
- Uses Groq API to generate answers.
- Rejects questions unrelated to Linux.

## Tech Stack

- Python
- LangChain
- SentenceTransformers
- Qdrant Cloud
- Groq API
- python-dotenv

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/RRRRRRRAhul/linux_commands_rag.git
cd linux_commands_rag
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the virtual environment

**Windows:**

```bash
.venv\Scripts\activate
```

**Linux/macOS:**

```bash
source .venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Create the `.env` file

Create a `.env` file in the project root:

```env
API_KEY=your_groq_api_key
QDRANT_API_KEY=your_qdrant_api_key
QDRANT_END_POINT=your_qdrant_cluster_endpoint
```

You need:

- A Groq API key
- A Qdrant Cloud API key
- A Qdrant Cloud cluster endpoint

### 6. Run the application

```bash
python rag.py
```

## Example Questions

```text
What does the pwd command do?
How can I list files in Linux?
What is chmod?
How can I check disk usage?
What is the difference between Linux and Windows?
```

## Security

Never commit your API keys or virtual environment.

Do not push:

```text
.env
.venv/
```

Keep your API keys private.

## Author

**Rahul Mandal**

GitHub: [RRRRRRRAhul](https://github.com/RRRRRRRAhul)
