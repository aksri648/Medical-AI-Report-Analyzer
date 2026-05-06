# 🧬 Medical AI Insights Platform

A lightweight AI-powered medical report analysis platform that extracts information from uploaded laboratory PDFs using OCR and generates structured healthcare insights using specialized medical language models running locally through Ollama.

The system is designed as a privacy-focused medical AI assistant capable of processing lab reports, summarizing abnormalities, generating patient-friendly explanations, and exporting professional AI-generated reports in Markdown and PDF formats.

---

# 🚀 Core Features

## 📄 Medical Report Upload

* Upload laboratory reports in PDF format
* Supports scanned/image-based reports

---

# 🔍 OCR-Based Text Extraction

Uses:

## EasyOCR

to:

* detect medical text
* extract laboratory values
* process scanned medical documents

---

# 🧠 Medical AI Analysis

Uses:

## MedGemma

(`medgemma:4b`)

to generate:

* abnormal findings
* medical insights
* risk indicators
* healthcare recommendations

while avoiding direct diagnosis.

---

# 📝 AI Report Summarization

Uses:

## Llama 3.2

(`llama3.2:3b`)

to:

* format reports professionally
* generate readable summaries
* create patient-friendly explanations
* structure the final healthcare report

---

# 📊 Real-Time Workflow Visualization

Interactive compact execution flow UI showing:

* OCR status
* Medical AI execution
* Summarizer execution
* PDF generation status

with dynamic:

* 🟡 Running
* 🟢 Completed
* 🔴 Error

state indicators.

---

# 📑 Export Functionality

Automatically generates:

* Markdown medical analysis report
* Downloadable PDF healthcare report

using:

## ReportLab

---

# 🌐 Cloud Deployment Architecture

Built to run efficiently on:

* Google Colab GPU runtime
* Ollama local model server
* Streamlit frontend
* Ngrok public tunnel

allowing full cloud-hosted AI execution without dedicated infrastructure.

---

# 🏗️ Tech Stack

| Layer          | Technology           |
| -------------- | -------------------- |
| Frontend UI    | Streamlit            |
| OCR Engine     | EasyOCR              |
| Medical AI     | MedGemma             |
| Summarization  | Llama 3.2            |
| AI Runtime     | Ollama               |
| PDF Generation | ReportLab            |
| Deployment     | Ngrok + Google Colab |

---

# ⚡ Key Highlights

* Fully local AI inference using Ollama
* Lightweight architecture optimized for low VRAM environments
* Sequential model execution with GPU memory cleanup
* Privacy-focused medical document processing
* Real-time workflow visualization
* Automated Markdown → PDF healthcare report generation
* Designed for rapid prototyping and healthcare AI experimentation

---

# 🎯 Use Cases

* AI-assisted laboratory report summarization
* Medical document intelligence
* Healthcare AI prototyping
* AI-powered clinical workflow automation
* Educational healthcare analysis tools
* OCR-to-LLM medical pipelines

---

# 🔮 Future Improvements

* Multi-model consensus analysis
* RAG-based medical knowledge retrieval
* Doctor verification workflows
* Medical image analysis support
* FastAPI backend architecture
* React-based frontend
* Vector database integration
* Multi-user authentication system


Setup Instructions

1)Download the notebook (.iypnb file)
2)Upload it to Google Colab
3)Change the Runtime to T4-GPU
4)Go to secrets section in the google colab and add a new secret "NGROK_AUTH_TOKEN" and turn the toggle on so that the repository can access it.
5)Run the notebook and click on the ngrok url created.