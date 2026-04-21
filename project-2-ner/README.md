# Project 2: Named Entity Recognition (NER)

## Overview

This project focuses on Named Entity Recognition (NER), a core Natural Language Processing (NLP) task that involves identifying and classifying key entities in text.

The objective is to build a structured, high-quality dataset by labeling entities such as people, locations, organizations, dates, and time expressions. The project simulates real-world annotation workflows, with a strong emphasis on consistency, precision, and clear labeling standards.

---

## Dataset Structure

The dataset is organized into four progressive batches, each introducing increasing levels of complexity:

* **Batch 1 – Basic Entities**  
  Focus on PERSON, LOCATION, and ORGANIZATION in clear and structured sentences.

* **Batch 2 – Temporal Entities**  
  Introduction of DATE and TIME alongside existing entity types.

* **Batch 3 – Mixed Complexity**  
  Sentences containing multiple entities within more natural language structures.

* **Batch 4 – Edge Cases & Ambiguity**  
  Advanced scenarios involving ambiguous references, role vs entity distinctions, partial names, possessive structures, and strict boundary enforcement.

---

## Entity Labels

The following entity types are used throughout the dataset:

* **PERSON** → Names of individuals  
* **LOCATION** → Countries, cities, regions, and geographical areas  
* **ORGANIZATION** → Companies, institutions, and groups  
* **DATE** → Specific dates or temporal references (e.g., “2024”, “January 10”)  
* **TIME** → Time expressions (e.g., “3 PM”, “morning”)  

---

## Annotation Approach

Entities are labeled based on strict and consistent guidelines:

* Only clear, specific named entities are labeled  
* Full entity spans are selected (e.g., “Elon Musk”, not “Elon”)  
* Multi-word entities are treated as a single unit (e.g., “South Africa”)  
* Titles and roles (e.g., CEO, president) are not labeled as entities  
* Generic or descriptive phrases are excluded  
* Ambiguous cases are skipped rather than guessed  

The focus is on **precision, consistency, and model-ready quality**, rather than over-labeling.

---

## Workflow

* Data structured into progressive batches  
* Annotation performed using Label Studio  
* Raw datasets exported after annotation  
* Clean datasets created through preprocessing and validation  
* Final dataset merged into a unified version  

Special care was taken to:

* Preserve sentences with no entities (labeled as "O")  
* Maintain consistency across batches  
* Avoid data loss during merging and cleaning  

---

## Files

Each batch includes:

* Raw dataset → original export from Label Studio  
* Clean dataset → processed and structured for machine learning use  

Final datasets:

* **ner_v1_full_raw.csv** → merged raw dataset  
* **ner_v1_full_clean.csv** → cleaned, model-ready dataset  

---

## Skills Demonstrated

* Named Entity Recognition (NER) annotation  
* Entity boundary detection and span precision  
* Multi-entity handling in complex sentences  
* Ambiguity resolution and edge case handling  
* Annotation guideline design and enforcement  
* Data cleaning, validation, and merging  
* Dataset structuring for machine learning workflows  

---

## Tools Used

* Label Studio  
* Python (pandas)  
* GitHub  
* CSV data processing  

---

## Status

All batches (1–4) completed.  
Dataset fully merged, cleaned, and validated.

This project represents a complete NER annotation pipeline, from dataset design and labeling to quality assurance and final dataset preparation for real-world NLP applications.
