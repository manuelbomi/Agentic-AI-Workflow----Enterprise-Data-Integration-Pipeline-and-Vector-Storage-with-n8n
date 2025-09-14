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

##### Select on changes involving specific folders
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/e23265f3-1579-4c77-9412-f1c3853ee363" />

---

#####  Click select credentials and pick create new credentials

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/c74d0563-74e4-4702-ae53-ac6aba334872" />

---

##### Pick create new credentials
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/12b400ae-179f-4b69-aea0-1c96f3a7c1d5" />

---

##### Go to Google Console and select your n8n project. See (here: https://github.com/manuelbomi/Enterprise-Agentic-AI---Scalable-Meeting-Orchestration-with-n8n ) regarding how to create you n8n project on GCP 
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/e9d3eec5-0700-4f9e-b1fb-ccc88f52e293" />

---

##### Select Enable API and Services
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/fc4525e2-1806-4773-bed8-3faca50aeb7a" />

---

##### Click + Enabled API and Services again

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/59f1c53f-8725-43a9-971f-f7a85c0891b9" />

---

##### Type to search for drive

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/f68e90d4-a376-4742-8835-246a870eb140" />

---

##### Select Google Drive API
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/0cb66ad9-8f6a-41ee-aa7b-209e105b51c9" />

---

##### Click on Enable
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/74374ec2-8518-44c9-9ee7-43d784c0d21c" />

---

##### On Google Drive API, go to Credentials
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/01c11767-e220-4e4b-ad5e-ba8eef086e77" />

---

##### Copy credentials ID for OAuth client
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/b4a8345b-82c0-4ff0-8e4a-bb682c1e190d" />

---

##### Paste the client ID on your Agent
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/936f6149-d151-40ed-9621-c3ed9f5754e4" />

---

##### Click on Edith OAuth Client
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/c983e5ea-bb3b-4c7f-893b-1c114b75adb7" />

---

##### Copy client secret
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/0c51d1f3-8055-4011-a329-788a2571c5fc" />

---

##### Copy the redirect URL from your agent
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/a1f6be98-62aa-479b-a994-e7b814846dab" />

---

##### Click on Add URI on Google Console and clisk to save

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/1a3576a9-dcd2-4596-8209-6a018a263ff7" />

---

##### Now try and sign in with Google mail
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/d43c24bb-38f0-49a2-9b0a-4035a89d7dfe" />

---

##### Sign on with Google mail
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/890d2c94-354d-4f46-90f7-1d9eac3735f9" />

---

#####  It will show connected successful for the Google Drive account that you use to store your files
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/dc6a9b6c-bc40-4bc5-87ef-06cadc30d93b" />

---

##### It will also show account connceted on your Agent UI
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/8018ad0d-d188-49bb-9285-5fdfa86464da" />

---

#####  Create a new folder in your Google Drive
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/ca909c9a-e557-44ec-8a65-e5a0ef642839" />

---

##### Create folder in your google drive and load up unstructured data about an interest e.g. Avanade
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/b8818c3c-1339-4967-97c1-1f0fb48f0c76" />

---

##### Create folder in your google drive and load up unstructured data about an interest e.g. GE Vernova or GE Aerospace
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/069d4269-062a-4e3c-aba2-e5f1622e61b8" />

---

##### Double click your Google drive trigger on n8n and select a folder e.g. Avanade
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/eee33a1f-0cc8-469d-af88-afebf737f68a" />

---

##### Under watch for select File Created
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/5016bc6d-4bcc-4b53-87b7-d637ca3565f7" />

---

##### Click on Fetch Test Event to test the file pull connectivity
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/eb72e730-b7e5-4aaf-8e21-0d7b334c4fad" />

---

##### Go back to canvas and add another node to download the file

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/1e6b73fa-d3a2-48a3-bdc8-92eaef0819a4" />

---

##### Select the download file node
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/568a3134-a887-4e3b-b0d5-62aa6b779fd9" />
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/09256bdd-3981-4bc9-84fa-e3f600f3cb5d" />

---

##### Select the By ID download method
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/653e7bf7-0b44-463a-bacd-f3944a2d41e0" />

---

##### Scroll through the node input and locate the ID and drag the ID into the node ID tab on the RHS
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/c09d8f3c-ca78-4d5c-96e6-fbdddb7ec2a5" />

---

##### Scroll thru the node input and locate the ID and drag the ID into the node ID tab on the RHS
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/672aa9cb-852b-4b21-b54f-36ed2b05b664" />

---

##### Click on the Execute step tab
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/1e9edfee-f014-4d5a-89a6-f5d9f46cb55c" />
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/3ce4483e-59e5-4300-a568-401b28fb5f0a" />

---

##### If a new file is added to the folder, it will download it
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/8b80d49f-fd86-43f0-9451-29d1c2390509" />

---

##### Create a Pinecone free account
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/9f5a5c65-f6f7-46c4-9a7c-b2317226905a" />

---

##### Create an index name n8n-agentic-ai in this instance
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/3ff07bdd-b7ec-48dc-a54f-1b6deee012cb" />

---

#####  Select (the desired OpenAI embedding) text-embedding-3-small in this instance
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/bf60c8c2-2c7c-47fd-9b21-05e53d140255" />

---

#####  Select serverless and click create index
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/8e768734-4ed4-43b8-9f67-8e39aeb8c806" />

---

##### Now, go to API keys
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/308e3b16-93b1-45c9-a9ba-18b3cc7ee1d2" />

---

##### Create API key
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/e0ca0630-d189-414b-a74f-911fca9ff068" />

---

##### Give your key a name
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/03596cd9-80d8-4407-8537-c1f1d34161df" />

---

##### Copy you API key immediately
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/2aaf1f98-94b4-43a0-9000-9657d0500443" />


---

##### Nw, go back to your n8n workflow
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/c3b9e0e3-85af-4426-9b7d-a307ab744b20" />

---

#####  Click the plus sign on Download File search for Pinecone and select Pinecone Vector Store
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/8e1b7a95-745d-4da5-a5bc-4123bf210892" />

---

##### Select Add Document to Vector Store
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/69d86f6a-76c2-47f7-84f2-ae0e913580fa" />

---

#####  Click on Credential to Connect with
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/d5c039d8-3fea-4097-9d37-257caae39cc9" />

---

##### Click Create New Credential
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/fc6ed245-5638-4a5c-b7ed-05cde578df32" />

---

##### Paste your API key
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/7dc1eb22-d4ff-450c-92dd-71296fa34986" />

---

##### Click save and you will see Connection Tested Successfully
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/451277c1-81f9-4ef5-ae6a-e2456f298366" />

---

##### On operation mode select Insert Document
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/61f73e5c-75c3-492b-95cb-4eb87772eb88" />









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



