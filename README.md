# AI-Powered-Regulatory-Compliance-Checker-for-Contracts
AI-powered system for automated contract compliance analysis using LLMs, detecting GDPR &amp; HIPAA risks, generating safe amendments, and producing audit-ready reports.

## 🚀 Project Overview

Manual contract compliance review is time-consuming, error-prone, and difficult to scale.
This project automates the entire compliance lifecycle using Large Language Models (LLMs).

The system is modular, explainable, reliable, and production-ready.

## 🧠 Key Features

- 📂 PDF Contract Upload  
- 🔍 Clause Extraction using Generative AI  
- ⚠️ Clause-Level Risk Analysis  
- 📜 GDPR & HIPAA Compliance Checks  
- ✏️ Automatic Amendment Generation (High-Risk Clauses Only)  
- 🧱 Safe Contract Rebuilding  
- 📊 Compliance Reports (JSON, CSV)  
- 📄 Updated Contract Output (TXT & PDF)  
- 🔔 Email & Slack Notifications  
- 📈 Google Sheets Audit Logging  
- 🛡️ LLM Fail-Safe & Fallback Mechanisms  

## 🏗️ System Architecture

Streamlit UI  
↓  
Pipeline Orchestrator (run.py)  
↓  
PDF Extraction → Text Cleaning → Chunking  
↓  
Clause Extraction (LLM)  
↓  
Risk Analysis (LLM)  
↓  
Compliance Gap Detection  
↓  
Amendment Generation (High Risk Only)  
↓  
Contract Rebuilding  
↓  
Outputs + Notifications + Audit Logs

## 🧩 Project Structure

.
├── app.py                         # Streamlit UI
├── run.py                         # Main pipeline orchestrator
├── src/
│   ├── clause_engine/
│   │   └── clause_extractor.py
│   ├── risk_engine/
│   │   └── risk_engine.py
│   ├── contract_modification/
│   │   ├── amendment_generator.py
│   │   ├── gap_analyzer.py
│   │   └── contract_rebuilder.py
│   ├── regulatory/
│   │   ├── gdpr_live_tracker.py
│   │   └── hipaa_live_tracker.py
│   ├── llm/
│   │   └── llm_router.py
│   ├── integrations/
│   │   ├── email_notifier.py
│   │   ├── slack_notifier.py
│   │   └── google_sheets/
│   │       ├── gsheet_client.py
│   │       └── gsheet_writers.py
│   └── utils/
│       ├── pdf_extract.py
│       ├── cleaner.py
│       ├── annotate_csv.py
│       └── pdf_writer.py
├── results/
├── data/
├── .env
└── README.md


