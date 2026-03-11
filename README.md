# Hiremate
# HireMate – LLM-based Resume Information Extraction System

HireMate is an AI-powered system that extracts structured candidate information from unstructured resumes using Large Language Models (LLMs).

The goal of the system is to automate resume screening by converting free-form resumes into structured data that can be used by recruiters, ATS systems, or analytics pipelines.

---

## Problem

Recruiters often spend significant time manually reading resumes and extracting key information such as:

- Candidate name
- Skills
- Education
- Work experience
- Contact information

Resumes come in many formats, making traditional rule-based extraction difficult.

HireMate uses LLM-powered extraction workflows to automatically convert unstructured resumes into structured data.

---

## Solution

HireMate uses a prompt-driven LLM pipeline that performs:

1. Resume text extraction
2. Information extraction using LLM prompts
3. Structured data validation
4. JSON output generation

The system focuses on extracting:

- Personal information
- Skills
- Education history
- Work experience
- Projects

---

## Architecture

The system follows a modular architecture:

Resume → Text Extraction → LLM Prompt Pipeline → Validation → Structured JSON Output

Components:

- **Extractor**: Processes raw resume text
- **LLM Prompt Engine**: Extracts structured fields
- **Validator**: Ensures correct formatting
- **Pipeline**: Orchestrates the workflow

---

## Example Output

Example structured data produced by the system:

```json
{
"name": "John Doe",
"email": "john.doe@email.com",
"skills": ["Python", "Machine Learning", "SQL"],
"education": [
{
"degree": "MS Computer Science",
"university": "Arizona State University"
}
],
"experience": [
{
"company": "Tech Company",
"role": "Software Engineer",
"years": "2022-2024"
}
]
}
