# Agri-Intel: RAG for Sustainable Farming

Agri-Intel is a Retrieval-Augmented Generation (RAG) application designed to provide farmers with expert agricultural advice. By using **Endee** as a high-performance vector database, the system performs semantic searches over crop data to provide grounded, accurate answers via an LLM.

## 🏗️ System Design
1. **Data Ingestion**: Agricultural guides are converted into 384-dimensional embeddings.
2. **Vector Storage**: Endee stores these embeddings and manages similarity searches.
3. **Retrieval**: When a user asks a question, Endee retrieves the most relevant context.
4. **Augmentation**: The context is fed into an LLM to generate a precise response.

## 🚀 Setup Instructions

### 1. Prerequisites
* Python 3.9+
* A running instance of the **Endee** server (from this forked repo).

### 2. Installation
```bash
# Clone your fork
git clone [https://github.com/YOUR_USERNAME/endee.git](https://github.com/YOUR_USERNAME/endee.git)
cd endee

# Install dependencies
pip install -r requirements.txt
