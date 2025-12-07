\# 🏥 Medical Research Assistant



RAG-based AI system for analyzing medical research papers and providing evidence-based answers to health questions.



\## 🎯 Project Overview



This system uses Retrieval-Augmented Generation (RAG) to:

\- Search through medical research papers

\- Find relevant scientific evidence

\- Generate accurate, citation-backed responses

\- Help users understand complex medical topics



\## 🏗️ Architecture

```

User Query → Embeddings → Vector Search → Context Retrieval → LLM Response

```



\*\*Components:\*\*

\- \*\*Vector DB\*\*: ChromaDB for document storage

\- \*\*Embeddings\*\*: OpenAI text-embedding-3-small

\- \*\*LLM\*\*: OpenAI GPT-4

\- \*\*UI\*\*: Streamlit web application



\## 📊 Dataset



50-100 curated medical research paper abstracts covering:

\- General health

\- Nutrition

\- Exercise

\- Mental health



\## 🚀 Quick Start



\### Prerequisites

```bash

Python 3.9+

OpenAI API key

```



\### Installation



1\. Clone the repository:

```bash

git clone https://github.com/your-username/medical-rag-assistant.git

cd medical-rag-assistant

```



2\. Install dependencies:

```bash

pip install -r requirements.txt

```



3\. Set up environment variables:

```bash

cp .env.example .env

\# Edit .env and add your OPENAI\_API\_KEY

```



4\. Prepare the database:

```bash

python scripts/prepare\_data.py

python scripts/load\_to\_db.py

```



5\. Run the application:

```bash

streamlit run app.py

```



\## 📁 Project Structure

```

medical-rag-assistant/

├── data/               # Dataset files

├── scripts/            # Data processing scripts

├── src/                # Core application code

├── docs/               # Documentation and screenshots

├── app.py              # Streamlit UI

├── requirements.txt    # Python dependencies

└── README.md           # This file

```



\## 🎥 Demo Video



\[Link will be added]



\## ⚠️ Disclaimer



This system is for educational purposes only. Always consult healthcare professionals for medical advice.



\## 📝 License



This project is created as part of a RAG development course.



---



\*\*Author\*\*: \[Your Name]  

\*\*Date\*\*: December 2024

