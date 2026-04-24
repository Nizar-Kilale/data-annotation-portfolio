# 🔎 Search Relevance Evaluation Dataset

## 📌 Project Overview

This project is a structured Search Relevance Evaluation Dataset designed to simulate real-world search engine behavior. It focuses on understanding how well different search results satisfy user intent across varying levels of query clarity and ambiguity.

The dataset was built manually using a multi-batch approach to reflect increasing levels of difficulty in search evaluation tasks.

This project is part of a broader Data Annotation Portfolio.

---

## 🎯 Objective

The goal of this project is to:

-- Evaluate how relevant different search results are to a given user query  
-- Classify user intent accurately  
-- Simulate real-world search engine ranking evaluation scenarios  
-- Train consistent decision-making in relevance labeling  

---

## 🧠 Intent Classification System

Each query is categorized into one of the following intent types:

-- **Informational** → User is seeking knowledge or understanding  
-- **Transactional** → User is comparing, choosing, or preparing to take action  
-- **Navigational** → User is trying to reach a specific website, app, or page  

---

## 📊 Relevance Scoring System

Each search result is labeled based on usefulness to the query:

-- **High Relevance** → Directly satisfies the user’s intent  
-- **Medium Relevance** → Partially useful or indirectly helpful  
-- **Low Relevance** → Not useful or unrelated to the intent  

---

## 🧩 Dataset Structure

Each row contains:

-- Query  
-- Three simulated search results  
-- Relevance scores for each result  
-- Intent classification  
-- Reasoning explanation  

---

## 🧪 Batch Structure

This dataset is built in progressive difficulty levels:

### ✔ Batch 1 — Easy
Clear queries with obvious intent and straightforward relevance judgments.

### ✔ Batch 2 — Medium
Queries with mixed relevance, partial matches, and realistic ambiguity.

### 🔜 Batch 3 — Hard (Planned)
Ambiguous queries with multiple possible interpretations requiring deeper reasoning.

### 🔜 Batch 4 — Advanced (Planned)
Noisy, real-world-like queries including slang, incomplete phrases, and misleading results.

---

## ⚙️ Methodology

-- Queries were manually designed to simulate real user search behavior  
-- Search results were synthetically generated to reflect real-world ranking noise  
-- Relevance was evaluated based on user intent satisfaction, not keyword matching  
-- Edge cases were included to test ambiguity handling  

---

## 🧠 Key Challenges Addressed

-- Intent ambiguity in real-world queries  
-- Distinguishing medium vs high relevance  
-- Avoiding keyword-based bias in evaluation  
-- Handling incomplete or vague queries  

---

## 📁 Technologies Used

-- Google Sheets (dataset creation)  
-- Manual annotation process  
-- Structured labeling framework  

---

## 📌 Future Work

-- Completion of Batch 3 (Ambiguous queries)  
-- Completion of Batch 4 (Noisy real-world queries)  
-- Potential conversion into ML training dataset format  

---

## 🚀 Author Notes

This project demonstrates skills in:

-- Data annotation for NLP tasks  
-- Search relevance evaluation  
-- Intent classification systems  
-- Dataset design and quality control  

---

## 📎 Repository Structure

project-3-search-relevance/  
-- data/  
-- docs/  
-- README.md  
