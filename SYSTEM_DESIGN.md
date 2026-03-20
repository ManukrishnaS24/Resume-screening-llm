

```markdown
## System Design Document

## Overview
The system is designed to automate resume screening using LLMs and rule-based scoring.

---

## Architecture

Resume PDF → Text Extraction → LLM Parsing → Scoring Engine → Report Generation

---

## Data Flow
1. Input resume (PDF)
2. Extract raw text using PDFPlumber
3. Parse structured data using Gemini LLM model and generates 4 multi‑dimensional scores (Exact, Similarity, Achievement, Ownership).
4. Compute scores:
   - Skill match
   - Semantic similarity
   - Achievement score
   - Ownership score
5. Generate final report using LangChain

---

## Components

### 1. Resume Parser
- Uses Gemini API
- Converts unstructured text → structured JSON

### 2. Scoring Engine
- Rule-based + embedding similarity
- Outputs candidate score

### 3. Report Generator
- Uses LangChain + Gemini

---

## Tech Stack
- Python
- Google Gemini API
- LangChain
- PDFPlumber
- FAISS (optional)

---

## Design Choices
- Used Gemini for strong NLP capabilities and because its free. Chatgpt and Claude requires billing
- LangChain for prompt orchestration
- Modular pipeline for scalability

---

## Future Improvements
- Add web UI
- Batch resume processing to prevent error 429 of too much input data into free gemini model.
- Real-time ATS integration
