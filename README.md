# My n8n Workflows Repository

A collection of production-ready n8n workflows for various automation purposes. This repository serves as both version control and deployment system for my n8n automations.

## Available Workflows
1. **🌟 Featured Workflow: AI-Powered Cover Letter Generator**

    The first workflow in this collection is an intelligent cover letter generation system that:

    - Monitors Google Drive for new resume/CV files (PDF, DOCX, TXT/MD)
    - Processes both structured and unstructured experience data
    - Stores and retrieves information from Pinecone vector database
    - Generates personalized cover letters using RAG (Retrieval-Augmented Generation)

## 🚀 Quick Start

**Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-n8n-workflows.git
   cd your-n8n-workflows
   ```

## 📁 Repository Structure

```
├── workflows/          # All n8n workflow JSON files
├── scripts/           # Import/export utilities            [TODO]
├── docker-compose.yml # Local development setup            [TODO]
└── README.md          # This file
```

## 🔧 Requirements

- n8n instance (local or hosted)
- Docker (optional, for local development)
- Various API credentials (Google Drive, Pinecone, AI services)

## 📝 Usage

Workflows can be:
- Manually imported through n8n UI
- [TODO] Automatically deployed via CI/CD pipelines
- [TODO] Imported using the included scripts

## 🤝 Contributing

This is a personal repository, but feel free to adapt the structure for your own n8n workflows!

## 📄 License

This repository contains personal automation workflows. Please respect the license terms of any third-party services integrated in these workflows.
