# 📊 Dataset Description — Search Relevance Evaluation Dataset

---

## 📌 Overview

This dataset contains manually annotated search relevance evaluations designed to simulate real-world search engine behavior. Each record represents a user query paired with three simulated search results, along with structured labels for intent and relevance.

The dataset is part of a broader Data Annotation Portfolio and is designed to demonstrate practical skills in NLP annotation, search evaluation, and intent classification.

---

## 🧠 Purpose

The main purpose of this dataset is to:

-- Simulate real-world search result evaluation tasks  
-- Train consistent judgment of relevance between queries and results  
-- Model different levels of user intent understanding  
-- Provide structured data for potential NLP or ranking model use  

---

## 📊 Data Structure

Each row in the dataset contains:

-- Query (user search input)  
-- Result 1, Result 2, Result 3 (simulated search results)  
-- Relevance scores for each result (High, Medium, Low)  
-- Intent classification (Informational, Transactional, Navigational)  
-- Reasoning explaining annotation decisions  

---

## 🧪 Dataset Batches

The dataset is organized into progressive difficulty levels:

### ✔ Batch 1 — Easy
Clear and unambiguous queries with straightforward relevance judgments.

### ✔ Batch 2 — Medium
Queries with partial matches, mixed relevance, and realistic ambiguity.

### 🔜 Batch 3 — Hard (Planned)
Ambiguous queries requiring deeper reasoning and interpretation.

### 🔜 Batch 4 — Advanced (Planned)
Noisy, incomplete, or real-world messy queries with misleading results.

---

## 🧠 Annotation Principles

-- Relevance is based on user intent satisfaction, not keyword matching  
-- Intent classification reflects the user’s underlying goal  
-- Medium relevance represents partial usefulness, not uncertainty  
-- Low relevance indicates misalignment with user intent  

---

## ⚙️ Creation Method

-- Queries were manually designed to reflect real search behavior  
-- Results were simulated to reflect realistic search engine outputs  
-- Labels were assigned based on structured evaluation rules  

---

## 🚀 Use Cases

This dataset can be used for:

-- Search relevance evaluation tasks  
-- NLP training and benchmarking  
-- Intent classification studies  
-- Data annotation practice and QA systems  

---

## 📌 Notes

This dataset is intentionally designed to include ambiguity and edge cases to reflect real-world search engine challenges.
