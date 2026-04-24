# 📄 Annotation Guidelines — Search Relevance Evaluation Dataset

---

## 1. Task Description

This project focuses on building a structured dataset for search relevance evaluation. The main objective is to simulate real-world search engine behavior by analyzing how well different results satisfy a user’s query intent.

The annotation process includes:

-- Evaluating search relevance between a query and multiple retrieved results  
-- Classifying user intent based on the query meaning  
-- Simulating realistic search scenarios with varying levels of ambiguity and noise  

The dataset is designed to reflect real-world search systems where results are not always perfectly aligned, requiring careful judgment of usefulness and relevance.

---

## 2. Intent Definitions

Each query is assigned one primary intent based on the user’s underlying goal.

---

### 📘 Informational
The user is looking to learn, understand, or explore a topic.

Examples:
-- what is machine learning  
-- how to build a website  
-- digital marketing explained simply  

---

### 🛒 Transactional
The user is preparing to take action such as:
-- buying a product  
-- booking a service  
-- choosing between options  
-- comparing alternatives  

Examples:
-- best laptop for programming students  
-- iPhone 15 worth it  
-- cheap flights to Zanzibar  

---

### 🌐 Navigational
The user is trying to reach a specific website, platform, or page.

Examples:
-- YouTube login  
-- Facebook sign in  
-- Google Maps  

---

## 3. Relevance Criteria

Each result is evaluated based on how well it supports the user’s intent.

---

### ⭐ High Relevance
-- Directly satisfies the user’s query intent  
-- Provides exact or highly useful information or action support  
-- Closely aligned with user goal  

---

### ⚖️ Medium Relevance
-- Partially helpful  
-- Indirectly related to the query  
-- Supports understanding or decision-making but not directly  

---

### ❌ Low Relevance
-- Not aligned with user intent  
-- Off-topic or distracting  
-- Misleading or unrelated domain  

---

## 4. Edge Cases (Important)

Some queries are ambiguous or can be interpreted in multiple ways. In these cases, intent must be inferred from user behavior patterns and common search expectations.

---

### Examples:

-- “best safari vs Tanzania parks”  
→ Transactional (comparison and decision-making intent)

-- “how to start investing”  
→ Informational (learning process, not execution)

-- “best side hustles online”  
→ Transactional (user evaluating options to act)

-- “cheap safari Tanzania” with unrelated results like casino ads  
→ Casino result = Low relevance (irrelevant intent mismatch)

---

### Key Rule for Edge Cases:
If a result does not help the user move closer to their goal, it must be classified as **Low relevance**, even if it shares keywords.

---

## 5. Quality Assurance (QA) Process

To ensure consistency and dataset quality, the following QA steps were applied:

-- Reviewed all query-result pairs for intent consistency  
-- Identified and corrected intent drift (e.g., misclassifying informational queries as transactional)  
-- Standardized relevance labeling across batches  
-- Ensured that Medium relevance is only used for partially useful or indirectly helpful results  
-- Validated that Low relevance strictly represents irrelevant or distracting outputs  

---

## 6. Final Notes

This dataset is designed to simulate real-world search engine evaluation scenarios. The goal is not keyword matching, but understanding **user intent and result usefulness in practical contexts**.

---
