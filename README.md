# Resume-screening-llm
LLM-based Resume Screening System using Gemini

## Overview

This project implements an intelligent resume screening system using Large Language Models (LLMs). It automates candidate evaluation by extracting structured information from resumes, computing relevance scores, and generating recruiter-style summaries.

---

## Features

*  Resume Parsing using Gemini LLM
*  Candidate Scoring System
  * Skill matching
  * Semantic similarity
  * Achievement analysis
  * Ownership evaluation
*  AI-generated Recruitment Report using (LangChain + Gemini)
*  Lightweight and modular pipeline

---

##  Tech Stack

* **Python**
* **Google Gemini API**
* **LangChain**
* **PDFPlumber**
* **Pydantic**

---

## System Workflow

1.  Input resume (PDF)
2.  Extract raw text using PDFPlumber
3.  Parse structured data using Gemini
4.  Evaluate candidate using scoring logic
5.  Generate final recruitment report using LangChain

---

##  How to Run

### 1. Install Dependencies

```
pip install pdfplumber google-generativeai langchain langchain-core langchain-google-genai pydantic
```

---

### 2. Set API Key

```
get an api key from llm model used.
in my implementation I have used an api key from gemini as I used gemini model for my llm.
```

---

### 3. Run the Program

```
python ipynb file
```

---

##  Output

The system produces:

*  Structured resume data (JSON format)
*  Candidate evaluation scores
*  Final recruiter-style report with verdict

---

##  Approach

The system combines **rule-based scoring** with **LLM reasoning**:

* Gemini is used for **resume parsing and understanding**
* Scoring logic evaluates candidate relevance
* LangChain generates a **human-like recruitment summary**

---

##  Project Structure

```
resume-screening-llm/
│
├── main.py
├── README.md
├── SYSTEM_DESIGN.md
```

---

##  Future Improvements

*  Web interface (Streamlit)
*  Batch resume processing
*  Explainable AI insights
*  Integration with ATS systems

---


**Your Name**

