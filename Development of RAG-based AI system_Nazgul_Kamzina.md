\# Development of RAG-based AI system

\*\*Student\*\*: Nazgul Kamzina

\*\*Date\*\*: 8 December 2024



---



\## 🔗 Project Links



\- \*\*GitHub Repository\*\*: https://github.com/Nazgulyalya/medical-rag-assistant

\- \*\*Demo Video\*\*: \[будет добавлено после записи]



---



\## 📋 Project Overview



\# Medical Research Assistant - RAG-based AI System



\## 🎯 Main Idea

An AI-powered assistant that helps users understand medical research papers and get evidence-based answers to health-related questions by retrieving relevant information from a curated database of scientific articles.



\## 💡 Core Concepts

\- \*\*Knowledge Base\*\*: Collection of medical research abstracts and summaries

\- \*\*Vector Search\*\*: Semantic search through embeddings to find relevant research

\- \*\*Context-Aware Responses\*\*: LLM generates answers based on retrieved scientific evidence

\- \*\*Citation Support\*\*: Responses include references to source papers



\## 🏗️ System Architecture



\### Components:

1\. \*\*Vector Database\*\*: ChromaDB for storing document embeddings

2\. \*\*Embedding Model\*\*: OpenAI text-embedding-3-small (1536 dimensions)

3\. \*\*LLM Provider\*\*: OpenAI GPT-4 via API

4\. \*\*User Interface\*\*: Streamlit web application

5\. \*\*Data Pipeline\*\*: Python scripts for data processing and ingestion



\### Data Flow:

```

User Query → Embedding → Vector Search → Context Retrieval → LLM + Context → Response

```



\## 📊 Dataset Concept



\### Source Data:

\- \*\*Type\*\*: Medical research paper abstracts

\- \*\*Topics\*\*: General health, nutrition, exercise, mental health

\- \*\*Format\*\*: JSON with fields: title, abstract, authors, year, DOI

\- \*\*Size\*\*: 50-100 papers (representative sample)

\- \*\*Sources\*\*: PubMed, arXiv, open-access journals



\### Data Structure:

```json

{

&nbsp; "id": "paper\_001",

&nbsp; "title": "Effects of Exercise on Mental Health",

&nbsp; "abstract": "Full abstract text...",

&nbsp; "authors": \["Smith J.", "Doe A."],

&nbsp; "year": 2023,

&nbsp; "doi": "10.1234/example",

&nbsp; "topic": "mental\_health"

}

```



\## 🔧 Technical Details



\### Technology Stack:

\- \*\*Language\*\*: Python 3.9+

\- \*\*Database\*\*: ChromaDB (persistent local storage)

\- \*\*Embeddings\*\*: OpenAI API (text-embedding-3-small)

\- \*\*LLM\*\*: OpenAI API (gpt-4)

\- \*\*UI Framework\*\*: Streamlit

\- \*\*Dependencies\*\*: openai, chromadb, streamlit, pandas, python-dotenv



\### System Requirements:

\- Python 3.9 or higher

\- 4GB RAM minimum

\- 1GB free disk space

\- Internet connection for API calls

\- OpenAI API key



\### Vector Database Configuration:

\- \*\*Collection Name\*\*: medical\_papers

\- \*\*Embedding Dimension\*\*: 1536

\- \*\*Distance Metric\*\*: Cosine similarity

\- \*\*Top-K Retrieval\*\*: 3-5 most relevant documents



\### RAG Pipeline:

1\. \*\*Chunking Strategy\*\*: Each paper abstract as a single chunk

2\. \*\*Metadata Storage\*\*: Title, authors, year, DOI for citations

3\. \*\*Retrieval\*\*: Top 3 semantically similar papers

4\. \*\*Prompt Template\*\*: Includes retrieved context + user question

5\. \*\*Response Format\*\*: Answer + citations with paper titles



\## ✅ Requirements



\### Functional:

\- Accept natural language health questions

\- Retrieve relevant research papers

\- Generate evidence-based answers

\- Provide source citations

\- Handle "I don't know" gracefully when no relevant data found



\### Non-Functional:

\- Response time < 10 seconds

\- Accurate retrieval (relevant papers in top 3)

\- Clear citation format

\- User-friendly interface



\## ⚠️ Limitations



\### Scope:

\- Not a replacement for medical advice

\- Limited to papers in the database

\- English language only

\- No real-time medical data



\### Technical:

\- Requires API keys (OpenAI)

\- Internet connection needed

\- Limited by embedding quality

\- Context window size (8K tokens for GPT-4)



\### Disclaimer:

System provides information for educational purposes only. Users should consult healthcare professionals for medical advice.



\## 🎥 Demo Video



---



\## ✅ Implementation Checklist



\- \[x] Step 1: Project description created

\- \[ ] Step 2: Dataset prepared

\- \[ ] Step 3: Vector database set up

\- \[ ] Step 4: Embeddings client implemented

\- \[ ] Step 5: Database populated with data

\- \[ ] Step 6: LLM client created

\- \[ ] Step 7: UI implemented

\- \[ ] Step 8: RAG system integrated

\- \[ ] Step 9: Demo video recorded



---



\## 🚀 Quick Start Guide



\### Prerequisites

```bash

Python 3.9+

OpenAI API key

```



\### Installation

```bash

git clone https://github.com/ваш-username/medical-rag-assistant.git

cd medical-rag-assistant

pip install -r requirements.txt

cp .env.example .env

\# Add your OPENAI\_API\_KEY to .env

```



\### Run Application

```bash

streamlit run app.py

```



---



\## 📸 Screenshots



\[Будут добавлены после разработки]



---



\## 🎓 Learning Outcomes



\[Здесь опишете, чему научились после завершения]



---



\*\*Repository\*\*: All code, data, and documentation available at GitHub link above.

