# Get-Started-with-Qdrant-Vector-DB
Get Started with Qdrant Vector DB. From Setup to First RAG Implementation using Qdrant.

## Installation & Setup

### Prerequisites
- Python 3.8+
- pip package manager
- Docker

### Quick Start

1. **Clone and navigate to project:**
   ```bash
   cd QdrantLearning
   ```

2. **Create virtual environment:**
   ```bash
   #Then open the terminal in pwd:
   python -m venv .venv
   # On Windows PowerShell:
   .venv\Scripts\Activate.ps1
   # On Windows CMD:
   .venv\Scripts\activate.bat
   # On macOS/Linux:
   source .venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up docker**
   ```bash
   # docker information:
   docker info
   # docker pull:
   docker pull qdrant/qdrant 
   # docker run:
   docker run -p 6333:6333 -v .:/qdrant/storage qdrant/qdrant
   ```




Now, 
- run the ingest.py to create the embeddings. Once the embeddings are created
- run the app.py to retrieve the relevant docs/chunks
