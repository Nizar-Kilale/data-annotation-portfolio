# Project 2: Named Entity Recognition (NER)

## Overview
This project focuses on Named Entity Recognition (NER), a core Natural Language Processing (NLP) task that involves identifying and classifying key entities in text.

The objective is to build a structured, high-quality dataset by labeling entities such as people, locations, organizations, dates, and time expressions. The project is designed to simulate real-world annotation workflows, with an emphasis on consistency, precision, and clear labeling rules.

---

## Dataset Structure

The dataset is organized into multiple batches, each designed to introduce increasing levels of complexity:

- **Batch 1 – Basic Entities**  
  Focus on PERSON, LOCATION, and ORGANIZATION in clear and structured sentences.

- **Batch 2 – Temporal Entities**  
  Introduction of DATE and TIME, alongside existing entity types.

- **Batch 3 – Mixed Complexity**  
  Sentences with multiple entities and more natural language structure.

- **Batch 4 – Edge Cases**  
  Ambiguity, overlapping entities, and more complex annotation scenarios.

---

## Entity Labels

The following entity types are used throughout the dataset:

- **PERSON** → Names of individuals  
- **LOCATION** → Countries, cities, regions, and geographical areas  
- **ORGANIZATION** → Companies, institutions, and groups  
- **DATE** → Specific dates or time references (e.g., “2024”, “January 10”)  
- **TIME** → Time expressions (e.g., “3 PM”, “morning”)  

---

## Annotation Approach

Entities are labeled based on clearly defined rules:

- Full entity spans are always selected (e.g., “Elon Musk”, not “Elon”)  
- Multi-word entities are treated as a single unit (e.g., “South Africa”)  
- Only relevant entities are labeled; no over-labeling  
- Labels are applied consistently across all batches  

The focus is on accuracy and consistency rather than speed.

---

## Workflow

- Data structured into progressive batches  
- Annotation performed using Label Studio  
- Raw datasets exported after annotation  
- Clean datasets created for machine learning use  
- All batches combined into a unified dataset  

---

## Files

Each batch includes:

- Raw dataset → original export from Label Studio  
- Clean dataset → processed and structured for ML use  

Final datasets:

- Combined dataset (raw)  
- Combined dataset (clean)  

---

## Skills Demonstrated

- Named Entity Recognition (NER) annotation  
- Entity boundary detection and span precision  
- Multi-entity handling in single sentences  
- Dataset structuring and batch design  
- Data cleaning and preparation for ML workflows  

---

## Tools Used

- Label Studio  
- Python (pandas)  
- GitHub  
- CSV data processing  

---

## Status

Batch 1 completed. Further batches in progress with increasing complexity and additional entity types.
