# Data Annotation Portfolio – Nizar Kilale

A structured portfolio of data annotation projects for machine learning datasets and AI training workflows.

---

## 📌 Overview

This repository showcases practical data annotation projects designed to demonstrate real-world dataset creation, labeling consistency, and preparation for machine learning applications.

The focus is on building high-quality, structured datasets while following clear annotation guidelines, progressive complexity design, and reproducible workflows.

Each project reflects a different aspect of annotation work, starting from sentiment classification, progressing into named entity recognition, and advancing into search relevance evaluation systems.

---

## 📂 Repository Structure

data-annotation-portfolio/
│
├── project-1-sentiment-analysis/
│   ├── data/
│   ├── docs/
│   └── README.md
│
├── project-2-ner/
│   ├── data/
│   ├── docs/
│   └── README.md
│
├── project-3-search-relevance/
│   ├── data/
│   ├── docs/
│   └── README.md
│
└── README.md   (Portfolio overview)

---

## 🚀 Projects

---

### 1. Sentiment Annotation – Product Reviews (v2)

A structured sentiment classification dataset built using a multi-batch annotation approach.

**Key Features:**
- 120 labeled samples  
- Binary sentiment classification (Positive / Negative)  
- Multi-batch design:
  - General sentiment  
  - Emotion intensity  
  - Value vs quality perception  
  - Edge cases (sarcasm, ambiguity, mixed sentiment)

📁 Location: `project-1-sentiment-analysis/`

---

### 2. Named Entity Recognition – General Text (v1)

A structured Named Entity Recognition (NER) dataset designed to identify and classify key entities within natural language text.

This project focuses on building annotation consistency across increasing levels of complexity, from simple entity extraction to advanced ambiguity handling.

**Key Features:**
- Multi-stage annotation pipeline (4 batches)  
- Entity types:
  - PERSON  
  - LOCATION  
  - ORGANIZATION  
  - DATE  
  - TIME  
- Includes entity-rich and no-entity sentences for realistic model training  
- Edge case handling (ambiguity, partial names, role vs entity conflicts)  
- Fully structured dataset with consistent labeling rules and QA validation  

📁 Location: `project-2-ner/`

---

### 3. Search Relevance Evaluation Dataset (v1–v2)

A structured dataset designed to simulate real-world search engine behavior by evaluating how well search results satisfy user intent.

This project introduces intent classification, relevance scoring, and multi-result evaluation per query.

**Key Features:**
- Query-based evaluation system (3 results per query)  
- Intent classification system:
  - Informational  
  - Transactional  
  - Navigational  
- Relevance scoring:
  - High  
  - Medium  
  - Low  
- Multi-batch design:
  - Batch 1: Easy / clear queries  
  - Batch 2: Medium / realistic ambiguity  
  - Batch 3: Hard (planned – ambiguous queries)  
  - Batch 4: Advanced (planned – noisy real-world queries)  
- Includes reasoning explanations for annotation decisions  
- Designed to simulate real-world search ranking evaluation scenarios  

📁 Location: `project-3-search-relevance/`

---

## 🧠 Skills Demonstrated

- Data annotation and labeling consistency  
- Sentiment classification dataset design  
- Named Entity Recognition (NER) annotation  
- Search relevance evaluation and ranking judgment  
- Intent classification systems  
- Handling ambiguity and edge cases in NLP tasks  
- Dataset structuring, cleaning, and versioning  
- Annotation guideline development  
- Multi-batch dataset design for progressive difficulty  
- Python (pandas) for dataset processing  
- Git/GitHub for version control and portfolio organization  

---

## 🛠 Tools Used

- Label Studio  
- Python (pandas)  
- Google Sheets  
- GitHub  

---

## 🎓 Certification

- Elements of AI Certification  
  Stored in `certifications/elements-ai-data-annotation-certification.png`

---

## 🎯 Career Goal

To develop professional-level data annotation and dataset engineering skills applicable to AI, NLP, and machine learning workflows.

This portfolio demonstrates progression from basic sentiment classification to structured entity recognition and advanced search relevance evaluation systems used in real-world AI training pipelines.
