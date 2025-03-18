# Real-Time-RAG-with-pw
Leveraging Pathway’s Vector Store, Agentic Frameworks and Real-Time Data Updates

# Real-Time Agentic RAG with Pathway (Finance Domain)

🚀 **An end-to-end real-time Retrieval-Augmented Generation (RAG) system** leveraging Pathway’s Vector Store, multi-agent frameworks, and real-time data updates.

This project demonstrates a fully functional Agentic RAG pipeline tailored for the finance domain, where real-time information retrieval is critical for accurate decision-making. The system empowers AI-driven financial analysis by dynamically retrieving, verifying, and synthesizing multi-modal financial data from diverse sources.

---

## Table of Contents

- [Key Features](#key-features)
- [System Architecture](#system-architecture)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Future Enhancements](#future-enhancements)
- [Contributors](#contributors)

---

## Key Features

- **Real-Time Data Processing** – Utilizes Pathway’s incremental indexing to ensure information is always up-to-date.
- **Agentic Query Execution** – Employs a multi-agent approach with frameworks like LangGraph, CrewAI, or AutoGen for advanced reasoning.
- **Multi-Modal Data Handling** – Processes financial PDFs, tables, and web data for comprehensive, accurate responses.
- **Adaptive Retrieval Strategies** – Balances retrieval complexity and efficiency dynamically for optimal performance.
- **Tool-Enhanced Querying** – Integrates APIs such as Yahoo Finance, Python Calculator, Edgar Tool, and Bing Web Search to address knowledge gaps.

---

## System Architecture

- **Data Ingestion** – Parses PDFs (text, tables, images) and converts tables into HTML format for structured access.
- **Chunking & Storage** – Extracts and processes text, indexing it efficiently in Pathway’s Vector Store.
- **Agent-Orchestrated Retrieval** – Leverages an LLM-powered agent to fetch the most relevant data chunks.
- **Multi-Agent Reasoning** – Dynamically selects external tools for additional data when required.
- **Query Execution** – Delivers responses via a scalable REST API using Pathway’s serve method.

---

## Tech Stack

- **Core Orchestrator**: Pathway
- **Agentic Frameworks**: LangGraph / CrewAI / AutoGen (optional)
- **LLM**: OpenAI GPT-4, Gemini, or LLaMA
- **Data Sources**: Financial PDFs, APIs (Yahoo Finance, Edgar, Bing Search)
- **Deployment**: FastAPI / Flask, Docker, Kubernetes (optional)

---

## Getting Started

Follow these steps to set up and run the project locally:

1. **Install Dependencies**

   ```bash
   pip install pathway langchain openai crewai flask

2. **Run The API **
  
    ```bash
python main.py


3. **Queery The API**

     ```bash
     curl -X POST "http://localhost:5000/query" -H "Content-Type: application/json" -d '{"query": "What are the latest Apple stock trends?"}'

##Contributor
[Shiveshwar Kumar Sah]
🤝 Open to collaboration! Feel free to contribute, open issues, or reach out with suggestions.

