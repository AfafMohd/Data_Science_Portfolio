Medical RAG System for Alzheimer's Research
A Retrieval-Augmented Generation (RAG) system designed to help medical researchers get instant, accurate answers from a curated corpus of recent Alzheimer's disease research articles.

🚀 Overview
This project addresses the challenge of keeping up with rapid advancements in medical research by building a question-answering system that grounds its responses in a trusted knowledge base. It combines efficient data ingestion, semantic search, and a state-of-the-art language model to provide contextually relevant answers while refusing out-of-domain queries.

🛠️ Tech Stack
Frameworks: LlamaIndex, Ollama

Language Model: Microsoft Phi-3 (via Ollama)

Embeddings: BAAI/bge-small-en-v1.5 (Sentence Transformers)

Vector Database: ChromaDB

Languages: Python

Libraries: Requests, BeautifulSoup, pdfplumber

📁 Project Architecture
The system follows a standard RAG pipeline:

Data Ingestion: Web scraping to collect recent research articles.

Preprocessing & Chunking: Cleaning text and splitting into semantically meaningful sentences.

Embedding & Indexing: Generating vector embeddings and storing them in ChromaDB.

Retrieval & Generation: Using LlamaIndex to retrieve relevant context and Phi-3 to generate final answers.

📦 Installation
Clone the repository:

bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install dependencies:

bash
pip install -r requirements.txt
Set up Ollama & Pull the Model:

Install Ollama from https://ollama.ai

Pull the Phi-3 model:

bash
ollama pull phi3
🏃‍♂️ Usage
Build the Knowledge Base:

bash
python build_knowledge_base.py
This script scrapes the target articles, processes the text, and populates the vector database.

Run the Query Application:

bash
python query_engine.py
Launch the interactive session to ask questions about Alzheimer's research.

📝 Example Queries
Domain-Specific (Answered):

"What is the focus of the EU-funded RobustSynapses project?"

"What role do reactive astrocytes play in Alzheimer's disease?"

Out-of-Domain (Rejected):

"Where is Kerala?"

"How to treat ulcers?"

🗺️ Future Improvements
Integration of multimodal data (images, audio).

Automated periodic knowledge base updates via scheduled scraping.

Experimentation with different embedding models and re-ranking techniques.

Development of a simple web interface for easier access.
