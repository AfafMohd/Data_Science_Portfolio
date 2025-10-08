### Medical RAG System for Alzheimer's Research
A Retrieval-Augmented Generation (RAG) system designed to help medical researchers get instant, accurate answers from a curated corpus of recent Alzheimer's disease research articles.

## Overview
This project addresses the challenge of keeping up with rapid advancements in medical research by building a question-answering system that grounds its responses in a trusted knowledge base. It combines efficient data ingestion, semantic search, and a state-of-the-art language model to provide contextually relevant answers while refusing out-of-domain queries.

## Tech Stack
Frameworks: LlamaIndex, Ollama

Language Model: Microsoft Phi-3 (via Ollama)

Embeddings: BAAI/bge-small-en-v1.5 (Sentence Transformers)

Vector Database: ChromaDB

Languages: Python

Libraries: Requests, BeautifulSoup, pdfplumber

## Project Architecture
The system follows a standard RAG pipeline:

1. Data Ingestion: Web scraping to collect recent research articles.

2. Preprocessing & Chunking: Cleaning text and splitting into semantically meaningful sentences.

3. Embedding & Indexing: Generating vector embeddings and storing them in ChromaDB.

4. Retrieval & Generation: Using LlamaIndex to retrieve relevant context and Phi-3 to generate final answers.

## Installation
1. Clone the repository:

bash

git clone https://github.com/AfafMohd/Data_Science_Portfolio/RAG_Alzheimer's_Disease_Research.git
cd your-repo-name

2. Install dependencies:

bash
pip install -r requirements.txt

3. Set up Ollama & Pull the Model:

- Install Ollama from https://ollama.ai

- Pull the Phi-3 model:

  bash
  
  ollama pull phi3
  
## Usage
1. Build the Knowledge Base:

bash

python build_knowledge_base.py

This script scrapes the target articles, processes the text, and populates the vector database.

2. Run the Query Application:

bash

python query_engine.py

Launch the interactive session to ask questions about Alzheimer's research.

## Example Queries
Domain-Specific (Answered):

"What is the focus of the EU-funded RobustSynapses project?"

"What role do reactive astrocytes play in Alzheimer's disease?"

Out-of-Domain (Rejected):

"Where is Kerala?"

"How to treat ulcers?"

## Future Improvements
Integration of multimodal data (images, audio).

Automated periodic knowledge base updates via scheduled scraping.

Experimentation with different embedding models and re-ranking techniques.

Development of a simple web interface for easier access.
