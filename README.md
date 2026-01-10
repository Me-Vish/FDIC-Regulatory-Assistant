# 🏦 FDIC Regulatory Assistant

An AI-powered regulatory assistant that analyzes loan documents by strictly referencing the **FDIC Risk Management Supervision (RMS) Manual – Section 3.2 (Loans)** to produce document-grounded, audit-ready regulatory insights.

## 📌 Overview
The FDIC Regulatory Assistant is designed to demonstrate the responsible use of Large Language Models (LLMs) in a highly regulated financial environment.  
It assists in regulatory analysis by extracting loan details, retrieving relevant regulatory context, and generating responses that are **strictly limited to the provided FDIC document**.

⚠️ This system does **not** approve, reject, or determine compliance for loans.

## 🎯 Problem Statement
Banks must review a large number of loan applications while ensuring strict adherence to complex federal regulations.  
Manual review is time-consuming, error-prone, and difficult to scale, while unrestricted AI systems risk hallucination and non-compliance.

## 💡 Solution
This project implements a regulation-restricted AI assistant that:
- Extracts loan information using OCR  
- Performs semantic search only on FDIC RMS Manual Section 3.2  
- Generates regulation-aligned responses  
- Explicitly refuses to answer when information is not found in the document
  
## 🔍 Key Features
- **OCR-Based Loan Processing**  
  Supports scanned PDFs and image-based loan documents.
- **Structured Loan Data Extraction**  
  Converts unstructured loan text into clean JSON.
- **Semantic Retrieval with Embeddings**  
  Retrieves only the most relevant regulatory sections.
- **Prompt-Restricted LLM Reasoning**  
  Prevents hallucination and external knowledge usage.
- **Interactive Web Interface**  
  Built with Gradio for transparent and user-friendly interaction.
  
## 🛠 Technology Stack
- Python  
- OpenAI API  
- Embeddings (text-embedding-3-small)  
- Tesseract OCR  
- pypdf, pdf2image  
- Gradio
  
## ⚙️ Workflow
1. Upload loan document  
2. Extract text using OCR  
3. Structure loan data into JSON  
4. Retrieve relevant FDIC regulatory sections  
5. Generate document-grounded regulatory response  
