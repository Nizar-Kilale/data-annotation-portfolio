# Named Entity Recognition (NER) – Annotation Guidelines

---

## 📌 1. Task Description

This project focuses on Named Entity Recognition (NER), which involves identifying and labeling specific entities within natural language text.

The goal is to:
- detect entities in text
- classify them into predefined categories
- maintain consistency across all annotations
- simulate real-world NLP dataset creation

Each sentence may contain:
- multiple entities
- a single entity
- or no entities at all

---

## 🧠 2. Entity Types

The following entity categories are used:

- PERSON → Names of people (real individuals)
- LOCATION → Cities, countries, regions, landmarks
- ORGANIZATION → Companies, institutions, brands, agencies
- DATE → Specific dates or calendar references
- TIME → Specific times or time expressions

---

## 🧾 3. Annotation Rules

### General Rules

- Only label clearly defined entities
- Do NOT label generic nouns or roles as entities
- Do NOT guess — if uncertain, do not label
- Maintain consistency across similar cases

---

### PERSON

✔ Label:
- Full names (e.g., "John Smith")
- First or last names if clearly referring to a person

✖ Do NOT label:
- Roles (e.g., "doctor", "teacher")
- Titles without names (e.g., "the president")

---

### LOCATION

✔ Label:
- Countries (e.g., "Tanzania")
- Cities (e.g., "Dar es Salaam")
- Regions or known places

✖ Do NOT label:
- Generic places (e.g., "the city", "the park")

---

### ORGANIZATION

✔ Label:
- Company names (e.g., "Google")
- Institutions (e.g., "World Bank")
- Agencies and brands

✖ Do NOT label:
- Generic business types (e.g., "the company", "a bank")

---

### DATE

✔ Label:
- Specific dates (e.g., "January 5, 2023")
- Years (e.g., "2020")
- Relative dates (e.g., "last year", "next month")

---

### TIME

✔ Label:
- Exact times (e.g., "3 PM", "14:30")
- Time expressions (e.g., "in the morning", "at night")

---

## ⚖️ 4. Entity Boundary Rules (VERY IMPORTANT)

- Label the FULL entity span only
  ✔ "New York City" → one LOCATION
  ✖ "New" + "York" separately

- Do NOT include extra words
  ✔ "Google" → ORGANIZATION
  ✖ "the Google company"

- Keep entity spans clean and precise

---

## 🔀 5. Edge Cases

### Ambiguity

- If a word can be multiple entity types, use context
  Example:
  - "Apple released a new product" → ORGANIZATION
  - "He ate an apple" → NOT an entity

---

### Partial Names

- Label if clearly referring to a known entity
  Example:
  - "Obama" → PERSON (if context supports it)

---

### No-Entity Sentences

- Some sentences will contain NO entities
- These should remain unlabeled
- This is important for realistic dataset training

---

### Overlapping Entities

- Do NOT create overlapping labels
- Choose the most accurate single span

---

## 🧩 6. Batch Design Logic

The dataset is structured in increasing complexity:

- Batch 1 → Simple, clear entities
- Batch 2 → Multiple entities per sentence
- Batch 3 → Ambiguity and context-dependent entities
- Batch 4 → Edge cases and difficult scenarios

---

## 🔍 7. Quality Assurance (QA Process)

All annotations are reviewed to ensure:

- correct entity classification
- consistent labeling decisions
- proper entity boundaries
- removal of incorrect or over-labeled entities

Corrections focus on:
- resolving ambiguity
- standardizing labeling patterns
- eliminating inconsistencies across batches

---

## 🎯 8. Core Principle

Consistency is more important than perfection.

When uncertain:
- rely on context
- follow existing patterns in the dataset
- avoid over-labeling
