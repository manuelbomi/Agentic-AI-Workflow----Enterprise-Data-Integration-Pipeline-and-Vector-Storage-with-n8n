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

#### Google Drive 🠊  n8n Workflow 🠊 Text Splitter 🠊  OpenAI Embeddings 🠊 Pinecone Vector Database

##### This architecture enables enterprises to build retrieval-augmented AI applications with a modular, scalable, and extensible design.

---

#### How To Use this Repository for Your Enterprise Project  🚀 

##### Prerequisites
    • n8n installed locally or in the cloud
    • Google Drive API credentials
    • OpenAI API key
    • Pinecone API key
    
##### Installation
    1. Clone this repository:
       git clone https://github.com/manuelbomi/Agentic-AI-Workflow----Enterprise-Data-Integration-Pipeline-and-Vector-Storage-with-n8n.git  
       cd agentic-ai-workflow
       
    2. Import the workflow JSON into n8n:
        ◦ Open n8n → Workflows → Import from file
        ◦ Select Enterprise_Data_from_Drive_to_Pinecone.json
        
    3. Configure your credentials inside n8n:
        ◦ Google Drive OAuth
        ◦ OpenAI API
        ◦ Pinecone API
        
    4. Activate the workflow.

#### Repository Contents  📂 
    • Enterprise_Data_from_Drive_to_Pinecone.json → The full n8n workflow definition
    • README.md → Documentation for architecture, setup, and usage

#### Enterprise Applications  💡 

##### This workflow forms the backbone for enterprise AI solutions, including:

    • Knowledge Graphs & Semantic Search: Connect siloed business documents
    
    • Decision Intelligence: AI-powered reasoning over enterprise datasets
    
    • Document Automation: Streamline contracts, reports, and knowledge bases
    
    • AI Architecture Blueprints: Extendable to CRM, ERP, HR, or Finance systems. 

#### Customization  🧩 
##### You can adapt this workflow for other enterprise data sources and applications:

    • Replace Google Drive with SharePoint, S3, or Dropbox
    
    • Swap Pinecone with Weaviate, Milvus, or Qdrant
    
    • Extend embedding generation with domain-specific models
    
    • Integrate with LLM-based Q&A bots for RAG
    
    * See (here: https://github.com/manuelbomi/Enterprise-Agentic-AI---Scalable-Meeting-Orchestration-with-n8n  ) for a comprehensive discourse regarding how you may fully integrate this workflow or similar workflows for your enterprise needs. 
    
    * See (here:https://github.com/manuelbomi/Automating-Complex-Enterprise-Business-Financial-Decisions-Using-Agentic-AI-in-n8n ) for example of financial or business applications
    
    * See (here: https://github.com/manuelbomi/An-Enterprise-Generative-AI-LLM-System-for-Manufacturing-and-Business-Applications- ) for example of deployment to Kubernetes clusters (e.g. Azure AKS) complete wit metrics monitoring (Prometheus & Grafana)
    
    * See (here: https://app.emmanueloyekanluprojects.com/ ) for actual deployment of a variant of the system. You may upload your own pdf files onto the system and query the system based on the uploaded data. 

---

> [!NOTE]
> Feel free to ignore the rest of the discourse if you are not interested in step-by-step method of designimg the Agentic AI workflow in n8n

---
---


# Step-by-Step Method for Designing the Agentic AI System in n8n

#### In this section, we provide step-by-step method by which interested users can design the Agentic AI workflow in their own system. 

#### Prerequisites
    • n8n installed locally or in the cloud.  You can read through a primer (here: https://github.com/manuelbomi/An-Enterprise-Agentic-AI-Primer-with-n8n  ) to get you started on installing your own instance of n8n .
    • Google Drive API credentials
    • OpenAI API key
    • Pinecone API key

### <ins>Workflow Design Procedure</ins>

#####  On your n8n canvas, type drive and select Google Drive
<img width="1366" height="768" alt="1 type drive and select Google Drive" src="https://github.com/user-attachments/assets/49021d6b-7c64-422d-b385-8556fd61264c" />

---

##### Select on changes inbolving specific folders
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/e23265f3-1579-4c77-9412-f1c3853ee363" />

---










---
#### License  📜 
##### MIT License. Free to use, adapt, and extend for enterprise and research applications.

---

Thank you for reading 

---



### **AUTHOR'S BACKGROUND**
### Author's Name:  Emmanuel Oyekanlu
```
Skillset:   I have experience spanning several years in data science, developing scalable enterprise data pipelines,
enterprise solution architecture, architecting enterprise systems data and AI applications,
software and AI solution design and deployments, data engineering, high performance computing (GPU, CUDA), machine learning,
NLP, Agentic-AI and LLM applications as well as deploying scalable solutions (apps) on-prem and in the cloud.

I can be reached through: manuelbomi@yahoo.com

Websites (professional):  http://emmanueloyekanlu.com/
Websites (application):  https://app.emmanueloyekanluprojects.com/
Publications:  https://scholar.google.com/citations?user=S-jTMfkAAAAJ&hl=en
LinkedIn:  https://www.linkedin.com/in/emmanuel-oyekanlu-6ba98616
Github:  https://github.com/manuelbomi

```
[![Icons](https://skillicons.dev/icons?i=aws,azure,gcp,scala,mongodb,redis,cassandra,kafka,anaconda,matlab,nodejs,django,py,c,anaconda,git,github,mysql,docker,kubernetes&theme=dark)](https://skillicons.dev)



