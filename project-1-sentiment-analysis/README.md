# Sentiment Annotation (Product Reviews) – Project v2

## Overview

This project involves annotating product review text into Positive and Negative sentiment categories. The goal is to build a high-quality, structured dataset suitable for machine learning, NLP experimentation, and sentiment classification tasks.

The dataset has evolved from an initial small-scale version into a structured multi-batch annotation system designed to capture different linguistic and emotional patterns in real-world product reviews.

---

## Dataset Versions

### v1 – Initial Dataset
- `dataset-v1.csv` → Raw export from Label Studio  
- `dataset-clean-v1.csv` → Cleaned and structured version for basic ML use  

### v2 – Expanded Structured Dataset (Current)
- `sentiment-product-reviews_v2_full_raw.csv` → Combined raw dataset (all batches)
- `sentiment-product-reviews_v2_full_clean.csv` → Final cleaned dataset for ML training

The v2 dataset contains **120 annotated samples** across four structured batches.

---

## Dataset Structure (v2)

The dataset is built from four controlled annotation batches:

- **Batch 1 – General Sentiment:** basic positive and negative product feedback  
- **Batch 2 – Emotion Intensity:** strong emotional expressions and subjective sentiment  
- **Batch 3 – Value vs Quality:** price perception, value-for-money evaluation, and expectation alignment  
- **Batch 4 – Edge Cases:** sarcasm, ambiguity, mixed sentiment, and subtle dissatisfaction  

This structure ensures diversity, consistency, and real-world language coverage.

---

## Annotation Guidelines

Each review is labeled based on overall customer sentiment.

### Positive
- Satisfaction is expressed  
- Product meets expectations  
- User is happy or satisfied  
- Recommendation is implied  

### Negative
- Dissatisfaction is expressed  
- Expectations are not met  
- Complaint or regret appears  
- Frustration or disappointment exists  

---

## Key Rule

If unclear, label based on whether the sentence leans toward satisfaction or dissatisfaction rather than tone or wording style.

---

## Label Definitions (v2 Standard)

- **Positive:** Acceptable performance, satisfaction, or met expectations  
- **Negative:** Unmet expectations, dissatisfaction, or clear negative sentiment  

---

## Workflow

1. Data collected and structured into four annotation batches  
2. Text labeled using Label Studio  
3. Batch-level exports generated (raw and cleaned)  
4. All batches merged into a unified dataset (v2)  
5. Final dataset cleaned, validated, and exported for ML use  

---

## Final Dataset

- Total Samples: 120  
- Format: CSV  
- Columns: text, label (and optional batch metadata)  

---

## Skills Demonstrated

- Data annotation design and consistency control  
- Multi-batch dataset structuring  
- Guideline-based labeling decisions  
- Data cleaning and preprocessing for ML  
- GitHub-based dataset versioning and management  

---

## Tools Used

- Label Studio  
- Python (pandas)  
- GitHub  
- CSV data processing  

---

## Certifications

- Elements of AI Certification  
  [View Certificate](certifications/elements-ai-data-annotation-certification.png)

## Status

Project completed at v2 stage with structured expansion from basic annotation to multi-dimensional sentiment dataset design. Further improvements may include model training and dataset scaling.
