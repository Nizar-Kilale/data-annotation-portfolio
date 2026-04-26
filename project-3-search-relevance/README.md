# 🔎 Search Relevance Evaluation Dataset (v1)

---

## 📌 Project Overview

This project is a structured Search Relevance Evaluation Dataset designed to simulate real-world search engine ranking and evaluation workflows.

It focuses on how effectively search results satisfy user intent across varying levels of query clarity, ambiguity, and noise.

Unlike simple classification tasks, this dataset evaluates **multiple results per query**, reflecting how modern search systems rank competing results.

The dataset is part of a broader Data Annotation Portfolio, demonstrating practical skills in NLP annotation, search evaluation, and intent classification.

---

## 🎯 Objective

The goal of this project is to:

-- Evaluate relevance of multiple results for a single query  
-- Accurately classify user intent  
-- Simulate real-world search ranking evaluation tasks  
-- Develop consistent decision-making under ambiguity  
-- Build a dataset suitable for NLP and ranking model training  

---

## 🧠 Intent Classification System

Each query is categorized into one of the following:

-- **Informational** → User wants to learn or understand  
-- **Transactional** → User intends to take action (buy, visit, book, choose)  
-- **Navigational** → User is searching for a specific site or destination  

---

## 📊 Relevance Scoring System

Each result is evaluated independently:

-- **High** → Directly satisfies user intent  
-- **Medium** → Partially helpful or supports decision-making  
-- **Low** → Irrelevant or does not match user need  

---

## 🧩 Dataset Structure

Each row contains:

-- Query  
-- Result 1, Result 2, Result 3  
-- Relevance labels for each result  
-- Intent classification  
-- Difficulty level (Easy → Noisy)  
-- Annotation notes (raw dataset only)  

---

## 🧪 Dataset Design (Progressive Complexity)

The dataset is structured into four batches:

### ✔ Batch 1 — Clear Intent (Easy)
Straightforward queries with direct relevance mapping.

### ✔ Batch 2 — Mixed Intent (Medium)
Queries with overlapping intent and partial matches.

### ✔ Batch 3 — Ambiguous & Decision-Based (Hard)
Queries requiring interpretation, comparison, and reasoning.

### ✔ Batch 4 — Noisy & Real-World (Advanced)
Vague, incomplete, and realistic queries with misleading results.

This progression reflects real-world annotation difficulty in production environments.

---

## ⚙️ Methodology

-- Queries were manually designed to reflect real user behavior  
-- Results were intentionally simulated to include both relevant and misleading outputs  
-- Relevance was judged based on intent satisfaction, not keyword matching  
-- Multiple review passes were conducted to improve consistency  
-- Edge cases were included to simulate real-world ambiguity  

---

## 🧠 Key Challenges Addressed

-- Interpreting ambiguous user intent  
-- Differentiating High vs Medium relevance  
-- Handling alternative vs direct results  
-- Avoiding keyword bias in evaluation  
-- Evaluating noisy and incomplete queries  

---

## 📂 Dataset Files

```text
data/
├── search-relevance-v1-raw.csv
├── search-relevance-v1-clean.csv
├── search-relevance-batch-01-raw.csv
├── search-relevance-batch-01-clean.csv
├── search-relevance-batch-02-raw.csv
├── search-relevance-batch-02-clean.csv
├── search-relevance-batch-03-raw.csv
├── search-relevance-batch-03-clean.csv
├── search-relevance-batch-04-raw.csv
└── search-relevance-batch-04-clean.csv
```


---

## 🔍 Key Features

-- Multi-result relevance evaluation  
-- Intent-driven labeling system  
-- Progressive difficulty design  
-- Real-world ambiguity simulation  
-- Raw + clean dataset pipeline  
-- Annotation reasoning included  

---

## 🚀 Use Cases

-- Search ranking model training  
-- NLP relevance evaluation tasks  
-- Intent classification systems  
-- Dataset benchmarking  
-- Human-in-the-loop AI workflows  

---

## 🛠 Tools Used

-- Google Sheets  
-- Manual annotation framework  
-- Structured labeling methodology  
-- GitHub (version control & dataset management)  

---

## 📌 Project Significance

This project goes beyond basic annotation by replicating **real-world search evaluation workflows**, where:

-- Multiple results compete for relevance  
-- User intent is often unclear or mixed  
-- Not all useful results are direct answers  

It demonstrates the ability to make consistent, high-quality annotation decisions in complex scenarios.

---

## 🚀 Author Notes

This project demonstrates:

-- Search relevance evaluation skills  
-- Intent classification expertise  
-- Handling ambiguity in NLP tasks  
-- Dataset structuring and cleaning  
-- Annotation consistency and QA thinking  

---

## 📎 Repository Structure

```text
project-3-search-relevance/

├── data/
├── docs/
└── README.md
```


---
