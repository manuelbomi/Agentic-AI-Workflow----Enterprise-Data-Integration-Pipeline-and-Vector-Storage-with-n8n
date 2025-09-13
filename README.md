# Agentic AI Workflow----Enterprise Data Integration Pipeline and Vector Storage with n8n

#### Introduction 📌
##### This repository demonstrates an Agentic AI workflow built with n8n that enables enterprises to:
    • Seamlessly ingest unstructured data from Google Drive
    • Preprocess and split documents into manageable chunks
    • Generate OpenAI embeddings
    • Store the resulting vectors in Pinecone for semantic search and downstream AI applications
    
##### By combining agentic AI patterns, n8n orchestration, and a scalable vector database architecture, this workflow forms a foundation for enterprise-grade AI systems such as:
    • Knowledge management platforms
    • AI-powered decision support systems
    • Intelligent document search and retrieval
    • Data-driven enterprise automation

The Agentic AI is shown in the figure below:

<img width="982" height="462" alt="Image" src="https://github.com/user-attachments/assets/71e76da7-1cbb-47ce-9834-6d24e2301eb0" />

---

#### Workflow Overview  ⚙️ 
##### The pipeline automates the following steps:

    1. Google Drive Trigger
        ◦ Watches a specified folder for newly created files.
        ◦ Automatically reacts when enterprise data is added.
        
    2. Download File
        ◦ Retrieves the uploaded file from Google Drive.
        
    3. Recursive Character Text Splitter
        ◦ Splits large documents into smaller, overlapping text chunks.
        ◦ Ensures context preservation for embeddings.
        
    4. Default Data Loader
        ◦ Prepares the document for AI processing.
        
    5. OpenAI Embeddings
        ◦ Transforms text chunks into vector embeddings.
        
    6. Pinecone Vector Store
        ◦ Inserts embeddings into a scalable vector database.
        ◦ Enables semantic search, retrieval-augmented generation (RAG), and enterprise AI knowledge systems.


---

#### Architecture  🏗️ 
##### Google Drive → n8n Workflow → Text Splitter → OpenAI Embeddings → Pinecone Vector Database

##### This architecture enables enterprises to build retrieval-augmented AI applications with a modular, scalable, and extensible design.

---

#### How To Use this Repository for Your Enterprise Project  🚀 

##### Prerequisites
    • n8n installed locally or in the cloud
    • Google Drive API credentials
    • OpenAI API key
    • Pinecone API key
    
Installation
    1. Clone this repository:
       git clone https://github.com/<your-username>/agentic-ai-workflow.git
       cd agentic-ai-workflow
    2. Import the workflow JSON into n8n:
        ◦ Open n8n → Workflows → Import from file
        ◦ Select Enterprise_Data_from_Drive_to_Pinecone.json
    3. Configure your credentials inside n8n:
        ◦ Google Drive OAuth
        ◦ OpenAI API
        ◦ Pinecone API
    4. Activate the workflow.

📂 Repository Contents
    • Enterprise_Data_from_Drive_to_Pinecone.json → The full n8n workflow definition
    • README.md → Documentation for architecture, setup, and usage

💡 Enterprise Applications
This workflow forms the backbone for enterprise AI solutions, including:
    • Knowledge Graphs & Semantic Search: Connect siloed business documents
    • Decision Intelligence: AI-powered reasoning over enterprise datasets
    • Document Automation: Streamline contracts, reports, and knowledge bases
    • AI Architecture Blueprints: Extendable to CRM, ERP, HR, or Finance systems

🧩 Customization
You can adapt this workflow for other enterprise data sources and applications:
    • Replace Google Drive with SharePoint, S3, or Dropbox
    • Swap Pinecone with Weaviate, Milvus, or Qdrant
    • Extend embedding generation with domain-specific models
    • Integrate with LLM-based Q&A bots for RAG


