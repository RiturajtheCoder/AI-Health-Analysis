# ⚕️ AI Health Diagnosis

> An AI-powered health analytics system that transforms CBC blood reports into structured medical insights, pattern analysis, contextual summaries, and safe recommendations.

---

## 📌 Overview

**AI Health Diagnosis** is an end-to-end AI application that automatically analyzes Complete Blood Count (CBC) reports uploaded as PDFs or images.

The system extracts medical parameters, validates them against clinical reference ranges, identifies health patterns, generates human-readable summaries, and allows users to ask questions about their reports through an AI-powered assistant.

The project combines:

* OCR-based report understanding
* Multi-model AI reasoning
* Retrieval-Augmented Generation (RAG)
* Clinical rule validation
* Medical safety guardrails
* Interactive Streamlit interface

---

## 🎯 Problem Statement

Blood reports are often difficult for non-medical users to understand.

Patients commonly face challenges such as:

* Complex medical terminology
* Unstructured report formats
* Lack of immediate interpretation
* Difficulty understanding abnormal values
* No personalized explanation of results

This project aims to bridge the gap between raw laboratory reports and understandable health insights using Artificial Intelligence.

---

## 🚀 Features

### 📄 Automated Report Analysis

* Upload CBC reports as PDF or image
* Automatic extraction of blood parameters
* OCR-assisted text processing

### 🧠 Multi-Model AI Pipeline

* Parameter extraction
* Validation & standardization
* Parameter interpretation
* Pattern recognition
* Contextual analysis
* Data synthesis
* Recommendations generation

### 💬 AI Health Assistant

* Ask natural-language questions about your report
* Context-aware responses
* Retrieval-Augmented Generation (RAG)

### 🔐 Medical Safety Guardrails

* No medicine prescriptions
* No dosage recommendations
* Educational guidance only
* Encourages professional consultation

### 📊 Interactive Dashboard

* Visualization of blood parameters
* Reference range comparison
* Risk assessment display
* Summary and recommendations

---

# 🏗️ System Architecture

```text
Blood Report (PDF / Image)
            │
            ▼
  Parameter Extraction
     (OCR + AI)
            │
            ▼
 Validation & Standardization
            │
            ▼
 Model 1: Interpretation
            │
            ▼
 Model 2: Pattern Recognition
            │
            ▼
 Contextual Analysis
            │
            ▼
     Data Synthesis
            │
            ▼
    Recommendations
            │
            ▼
   AI Health Assistant
```

---

# 🔄 Workflow

### 1️⃣ Extract Parameters

The uploaded report is processed using OCR and AI-assisted extraction techniques.

Example:

```text
Hemoglobin → 13.5 g/dL
WBC → 7800 /cumm
Platelets → 250000 /cumm
```

### 2️⃣ Validate & Standardize

Extracted values are:

* Normalized
* Converted to standard formats
* Validated against clinical reference ranges

### 3️⃣ Model 1 – Interpretation

Each parameter is individually classified as:

* LOW
* NORMAL
* HIGH

### 4️⃣ Model 2 – Pattern Recognition

The system detects meaningful clinical patterns.

Examples:

* Possible Anemia
* Infection Indicators
* Thrombocytopenia
* Leukocytosis

### 5️⃣ Context Analysis

Patient demographics such as:

* Age
* Gender

are incorporated into interpretation.

### 6️⃣ Data Synthesis

The system generates a concise doctor-style summary.

### 7️⃣ Recommendations

Generates safe and educational recommendations such as:

* Dietary guidance
* Lifestyle suggestions
* Follow-up recommendations

---

## 🛠️ Tech Stack

### Programming Language

* Python

### Frontend

* Streamlit

### AI & LLM

* Groq
* LangChain
* LangGraph

### OCR & Document Processing

* PyMuPDF
* Tesseract OCR
* Pillow

### Data Processing

* Pandas
* Pydantic

### Visualization

* Matplotlib

### Retrieval

* Retrieval-Augmented Generation (RAG)

---

## 📂 Project Structure

```text
AI_Health_Diagnosis/
│
├── app.py
│
├── graph/
│   ├── graph_builder.py
│   ├── run_pipeline.py
│   └── rag_pipeline.py
│
├── nodes/
│   ├── extract_parameters.py
│   ├── validate_standardize.py
│   ├── model1_interpretation.py
│   ├── model2_patterns.py
│   ├── model3_context.py
│   ├── synthesis.py
│   └── recommendations.py
│
├── utils/
│   ├── llm_utils.py
│   ├── reference_ranges.py
│   └── helpers.py
│
├── requirements.txt
│
└── README.md
```

---

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/AI-Health-Diagnosis.git
cd AI-Health-Diagnosis
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create a `.env` file:

```env
GROQ_API_KEY=your_groq_api_key
```

### Run the Application

```bash
streamlit run app.py
```

---

## 📈 Results

### Achievements

✅ Successfully analyzed 40+ real-world CBC reports

✅ Reduced manual interpretation effort by approximately 85%

✅ Automated extraction and interpretation pipeline

✅ Interactive AI-powered report assistant

✅ Safe healthcare-oriented AI workflow

---

## ⚠️ Limitations

* Supports CBC reports only
* OCR quality affects extraction accuracy
* Not intended to replace professional medical diagnosis
* Educational use only

---

## 🔮 Future Scope

* Support for additional laboratory reports
* Multi-language report analysis
* Longitudinal health trend tracking
* Doctor-facing dashboard
* Explainable AI confidence scores
* Healthcare platform integration

---

## 📷 Example Questions

```text
What does my hemoglobin level mean?

Are my blood parameters normal?

What foods may support healthy blood counts?

Explain my CBC report in simple language.

What does MCHC indicate?
```

---

## 🤝 Acknowledgements

This project was developed during an internship organized by:

* Infosys Springboard Virtual Internship

---

## ⭐ Support

If you found this project useful, please consider giving it a **Star ⭐** on GitHub.
