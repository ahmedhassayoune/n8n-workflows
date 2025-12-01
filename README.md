# My n8n Workflows Repository

A collection of production-ready n8n workflows for various automation purposes. This repository serves as both version control and deployment system for my n8n automations.

## Available Workflows
1. **📨 Featured Workflow: AI-Powered Cover Letter Generator**

    The first workflow in this collection is an intelligent cover letter generation system that:

    - Monitors Google Drive for new resume/CV files (PDF, DOCX, TXT/MD)
    - Processes both structured and unstructured experience data
    - Stores and retrieves information from Pinecone vector database
    - Generates personalized cover letters using RAG (Retrieval-Augmented Generation)

2. **🔍 Automated LinkedIn Job Scraper & Tracker**
   
    A fully automated workflow that **scrapes, filters, and tracks** relevant LinkedIn job postings, powered by LLM-based analysis and Notion integration.
   
    - **Scheduled Runs**: Executes twice daily (9 AM & 3 PM) to capture fresh offers.
    - **Smart Job Search**: Keyword-based queries with location, experience, and job-type filters.
    - **Automatic Pagination**: Scrolls through search results (up to ~200 offers per keyword).
    - **Relevance Filter**: First LLM pass selects offers matching your profile (junior / CV / ML / healthcare, etc.).
    - **Structured Extraction**: Second LLM extracts relevant offer fields: Title, company, location, salary, required skills, a 3-sentence summary of job description.
    - **Notion Sync**: Automatically creates/updates entries to a notion table to keep track of offers.
    - **Email Alerts**: Sends a clean summary of new opportunities with links and skill highlights.
    - **Rate Limiting**: Randomized delays to avoid LinkedIn throttling.

## 🚀 Quick Start

Manualy import JSON workflows to n8n instance and fill out necessary API credentials.

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

## 🤝 Contributing

This is a personal repository, but feel free to adapt the structure for your own n8n workflows!

## 📄 License

This repository contains personal automation workflows. Please respect the license terms of any third-party services integrated in these workflows.
