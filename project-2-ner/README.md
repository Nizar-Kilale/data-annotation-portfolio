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

---

## Case Study – Named Entity Recognition (NER)

## 1. Introduction

This project focuses on building a Named Entity Recognition (NER) dataset as part of a structured data annotation workflow. The goal was to identify and label key entities in text, including people, locations, organizations, dates, and time expressions.

Unlike simple labeling exercises, this project was designed to reflect real-world annotation conditions where language is often inconsistent, ambiguous, and context-dependent. The dataset was built progressively through multiple annotation batches, each increasing in complexity to simulate real production-level data scenarios.

The final output is a structured dataset intended for machine learning use, with a strong emphasis on consistency, annotation precision, and handling of edge cases.

---

## 2. Problem Statement

Named Entity Recognition (NER) is a fundamental task in Natural Language Processing, but it becomes significantly more complex when applied to real-world text. Language is often inconsistent, context-dependent, and includes ambiguous references that cannot be labeled using simple rules alone.

The challenge in this project was to create a high-quality NER dataset that could reflect these real-world conditions while maintaining strict consistency in annotation decisions. This required more than just identifying entities; it required defining clear boundaries for what should and should not be labeled under different contexts.

Another key challenge was ensuring that annotation decisions remained consistent across different sentence structures and levels of complexity. As the dataset evolved through multiple batches, the difficulty increased from simple named entity recognition to more ambiguous cases involving partial names, role-based references, and possessive structures.

The objective was to simulate a realistic annotation environment where decisions must remain consistent even when the text does not provide clear or direct answers.

---

## 3. Dataset Design

The dataset was structured using a progressive batch system to simulate increasing levels of annotation complexity. This approach was intentional, allowing the annotation process to move from simple, well-defined cases to more realistic and ambiguous scenarios.

The dataset consists of four main batches:

Batch 1 focused on basic named entity recognition, including clear instances of PERSON, LOCATION, and ORGANIZATION entities. These sentences were structured to reduce ambiguity and establish consistent annotation patterns at the foundational level.

Batch 2 introduced temporal information, adding DATE and TIME entities. This required the annotation process to expand beyond static entities and account for time-based expressions while maintaining consistency with earlier entity types.

Batch 3 increased complexity by introducing multiple entities within single sentences. This stage required careful attention to entity boundaries and reinforced consistency when different entity types appeared in close proximity.

Batch 4 focused on edge cases and ambiguity. This included challenges such as partial names, possessive structures, role-based references, and cases where entity boundaries were not immediately clear. This batch was designed to simulate real-world annotation difficulties where strict rules must be applied under uncertain conditions.

Overall, this structured progression allowed for controlled complexity growth, ensuring that annotation quality remained stable while gradually introducing more realistic data scenarios.

---

## 4. Annotation Strategy

The annotation process was guided by strict and consistent rules to ensure high-quality and reliable dataset creation. The primary focus was on maintaining precision in entity labeling while avoiding unnecessary or incorrect annotations.

Only clearly defined named entities were labeled. This included explicit mentions of individuals, organizations, locations, dates, and time expressions. Generic terms, roles, or descriptive phrases were intentionally excluded to avoid introducing noise into the dataset.

Entity boundaries were carefully controlled to ensure full and accurate span selection. Multi-word entities were treated as single units, meaning the complete name was always labeled rather than partial fragments.

A strict rule was applied regarding ambiguity: when an entity could not be confidently identified, it was excluded rather than guessed. This ensured that the dataset remained clean and reduced the risk of introducing inconsistent labeling patterns.

Special attention was given to possessive and contextual references. In such cases, the annotation focused on extracting the core named entity rather than the surrounding grammatical structure.

Consistency across batches was also a key priority. The same entity type was always handled in the same way regardless of sentence structure or complexity level.

---

## 5. Challenges & Fixes

One of the main challenges in this project was handling ambiguity in natural language. Many sentences did not contain clearly defined entities or included references that could be interpreted in multiple ways. In such cases, the decision was to prioritize precision over coverage by excluding uncertain labels rather than introducing inconsistent annotations.

Another challenge was maintaining consistent entity boundaries across different sentence structures. The same entity could appear in multiple formats, and ensuring that it was always labeled in a uniform way required continuous validation throughout the annotation process.

Batch 4 introduced additional complexity through edge cases such as partial names, possessive structures, and role-based references. For example, phrases combining titles and names required careful separation to ensure only the actual named entity was labeled.

A technical challenge was encountered during dataset merging and cleaning, where sentences without entities were at risk of being removed due to standard preprocessing steps. This was resolved by adjusting the cleaning logic to preserve all valid sentences while only filtering out incomplete or corrupted rows.

Consistency across batches was another key issue. As complexity increased, there was a risk of drifting away from earlier annotation decisions. This was addressed through continuous review of earlier batches to ensure alignment in labeling rules.

---

## 6. Outcome & Final Result

The final output of this project is a structured Named Entity Recognition (NER) dataset built through a progressive annotation process. The dataset includes multiple levels of complexity, ranging from basic entity recognition to advanced edge cases involving ambiguity and contextual interpretation.

All data was carefully labeled using consistent annotation rules and validated through multiple review cycles to ensure quality and uniformity. Special attention was given to maintaining correct entity boundaries, handling ambiguous cases, and ensuring consistency across all batches.

The dataset includes both entity-rich sentences and sentences without entities, which helps improve realism for machine learning applications and reduces bias toward over-labeling.

The final dataset is fully merged and cleaned into two versions:
- A raw version preserving original annotations
- A cleaned version prepared for machine learning use

This project demonstrates the full lifecycle of an annotation workflow, including dataset design, structured labeling, quality control, and final data preparation.

The result is a model-ready dataset suitable for Named Entity Recognition tasks and a documented workflow that reflects practical experience in real-world NLP data annotation.
