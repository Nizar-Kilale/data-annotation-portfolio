# 📊 Dataset Description — Search Relevance Evaluation Dataset (v1)

---

## 📌 Overview

This dataset contains manually annotated search relevance evaluations designed to simulate real-world search engine behavior.

Each record represents a user query paired with three simulated search results, along with structured labels for intent classification and relevance scoring.

Unlike simple classification datasets, this project focuses on evaluating multiple results per query, reflecting how modern search systems rank and present information.

The dataset is part of a broader Data Annotation Portfolio and demonstrates practical skills in NLP annotation, search evaluation, and user intent interpretation.

---

## 🧠 Purpose

The main purpose of this dataset is to:

-- Simulate real-world search result evaluation workflows  
-- Train consistent and structured relevance judgment  
-- Model varying levels of user intent complexity  
-- Develop decision-making skills under ambiguity  
-- Provide structured data suitable for NLP and ranking model use  

---

## 📊 Dataset Structure

The dataset is available in both full and batch-level formats.

### 🔹 Full Dataset

-- `search-relevance-v1-raw.csv` (includes annotation reasoning)  
-- `search-relevance-v1-clean.csv` (model-ready, standardized)  

### 🔹 Batch-Level Datasets

Each batch includes both raw and clean versions:

-- Batch 1 — Clear Intent (Easy)  
-- Batch 2 — Mixed Intent (Medium)  
-- Batch 3 — Ambiguous & Decision-Based (Hard)  
-- Batch 4 — Noisy & Real-World Queries (Advanced)  

---

## 🧾 Data Fields

Each row contains:

-- Query (user search input)  
-- Result 1, Result 2, Result 3 (simulated search results)  
-- Relevance scores (High, Medium, Low for each result)  
-- Intent classification (Informational, Transactional, Navigational)  
-- Difficulty level (Easy, Medium, Hard, Noisy)  
-- Annotation notes (raw dataset only)  

---

## 🧪 Dataset Design Philosophy

This dataset follows a **progressive complexity model**, where each batch introduces new challenges:

### ✔ Batch 1 — Easy  
Clear, explicit queries with direct intent and obvious relevance matches.

### ✔ Batch 2 — Medium  
Mixed intent queries with partial matches and early-stage ambiguity.

### ✔ Batch 3 — Hard  
Ambiguous queries requiring interpretation, comparison, and decision-based reasoning.

### ✔ Batch 4 — Advanced  
Noisy, vague, and real-world queries with misleading or competing results.

This structure reflects how search relevance tasks evolve in real-world annotation environments.

---

## 🧠 Annotation Principles

-- Relevance is based on **user intent satisfaction**, not keyword overlap  
-- Intent classification reflects the **underlying user goal**, not surface wording  
-- High relevance = directly answers or fulfills the query  
-- Medium relevance = supports decision-making or partially satisfies intent  
-- Low relevance = irrelevant or represents a different user need  

Special attention is given to:

-- Ambiguity handling  
-- Alternative vs direct results  
-- Decision-support vs direct answers  
-- Realistic user behavior patterns  

---

## ⚙️ Creation Methodology

-- Queries were manually designed to reflect real user search behavior  
-- Results were intentionally simulated to include both relevant and misleading options  
-- Labels were assigned using structured annotation guidelines  
-- Multiple refinement passes were conducted to improve consistency and accuracy  
-- Raw datasets preserve annotation reasoning for transparency and QA  

---

## 🔍 Key Features

-- Multi-result evaluation per query  
-- Intent-driven relevance scoring  
-- Progressive batch-based complexity  
-- Real-world ambiguity and noise simulation  
-- Dual dataset format (raw + clean)  
-- Annotation reasoning included (raw datasets)  

---

## 🚀 Use Cases

This dataset can be used for:

-- Search ranking and relevance modeling  
-- NLP training and evaluation  
-- Intent classification systems  
-- Annotation quality benchmarking  
-- Human-in-the-loop AI training workflows  

---

## 📌 Notes

This dataset is intentionally designed to reflect real-world search challenges, including ambiguity, incomplete queries, and competing result relevance.

The clean dataset is optimized for machine learning pipelines, while the raw dataset provides insight into annotation reasoning and decision-making processes.

---
