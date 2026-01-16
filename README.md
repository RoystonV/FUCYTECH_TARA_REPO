# FUCYTECH_TARA_REPO
ISO/SAE 21434 compliant Threat Analysis and Risk Assessment (TARA) report generator using RAG and LLMs.

# TARA Report Generator (ISO/SAE 21434)

An internal web application for generating **ISO/SAE 21434–aligned Threat Analysis and Risk Assessment (TARA)** reports for automotive ECUs and systems.

The tool leverages **Retrieval‑Augmented Generation (RAG)** and **Large Language Models (LLMs)** to assist cybersecurity engineers in producing structured, consistent, and auditable TARA outputs.

---

##  Overview

This application supports the early phases of automotive cybersecurity engineering by:
- Structuring TARA activities according to ISO/SAE 21434
- Assisting with threat identification, risk assessment, and mitigation reasoning
- Providing both **human‑readable** and **machine‑readable** outputs

The tool is intended for **internal engineering use** and **decision support**.

---

##  Features

- ECU / system–based TARA generation
- ISO/SAE 21434–aligned report structure
- Markdown preview of generated reports
- High‑quality **PDF export (A4 landscape)**
- **JSON export** for traceability and downstream tooling
- Damage scenario generation with SFOP‑style scoring
- Explicit assumptions when data is incomplete
- Environment‑variable–based secret handling (no hardcoded keys)

---
User (Browser)
│
▼
Streamlit Web App (app.py)
│
▼
RAG Pipeline (tara_backend.py)
│
▼
ISO/SAE 21434 Documents + LLM


- **Streamlit** – UI layer
- **Haystack** – RAG orchestration
- **Google Gemini** – LLM reasoning
- **WeasyPrint** – PDF rendering

---

##  Tech Stack

- Python 3.10+
- Streamlit
- Haystack
- Google Gemini (LLM)
- WeasyPrint
- Markdown2

---

##  Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/<org-or-username>/tara-report-generator.git
cd tara-report-generator

