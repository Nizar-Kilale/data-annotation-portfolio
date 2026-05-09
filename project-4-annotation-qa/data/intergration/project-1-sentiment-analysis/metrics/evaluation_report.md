# Sentiment Classification Evaluation Report

## Project Overview

This project simulates a real-world sentiment analysis evaluation workflow using a manually reviewed dataset of 60 product-review examples.

The dataset was intentionally extended beyond simple labels to support advanced machine learning evaluation concepts commonly used in NLP and data annotation projects.

The goal is to demonstrate practical understanding of:

- Precision
- Recall
- F1-score
- Error analysis
- Confidence scoring
- Classification outcomes
- Difficulty tagging
- Ambiguous sentiment handling

This repository is structured to resemble professional annotation and evaluation pipelines used in production ML environments.

---

# Dataset Summary

| Metric | Value |
|---|---|
| Total Samples | 60 |
| Positive Labels | 35 |
| Negative Labels | 25 |
| Correct Predictions | 55 |
| Incorrect Predictions | 5 |
| Accuracy | 91.67% |

---

# Classification Breakdown

## True Positives (TP)

Positive reviews correctly predicted as Positive.

Total: 35

Examples:
- "The product arrived quickly and works perfectly."
- "Great quality and definitely worth the price."

---

## True Negatives (TN)

Negative reviews correctly predicted as Negative.

Total: 20

Examples:
- "I regret buying this product."
- "Too expensive for such low quality."

---

## False Positives (FP)

Negative reviews incorrectly predicted as Positive.

Total: 1

Example:
- "The product is good but too expensive for what it offers."

Analysis:
The model focused heavily on the positive wording ("good") while failing to properly weight the negative pricing complaint.

---

## False Negatives (FN)

Positive reviews incorrectly predicted as Negative.

Total: 4

Examples:
- "It's okay nothing special but works fine."
- "It's just average nothing impressive."
- "It's not great but not terrible either."
- "Decent product for the cost."

Analysis:
Most false negatives occurred in weak-positive or neutral-positive statements containing mixed wording and reduced emotional intensity.

---

# Precision Calculation

Precision measures how many predicted positive results were actually positive.

Formula:

Precision = TP / (TP + FP)

Using this dataset:

Precision = 35 / (35 + 1)

Precision = 35 / 36

Precision = 0.9722

Precision Score = 97.22%

Interpretation:
When the model predicts Positive sentiment, it is correct most of the time.

---

# Recall Calculation

Recall measures how many actual positive examples were successfully identified.

Formula:

Recall = TP / (TP + FN)

Using this dataset:

Recall = 35 / (35 + 4)

Recall = 35 / 39

Recall = 0.8974

Recall Score = 89.74%

Interpretation:
The model misses some softer or ambiguous positive reviews.

---

# F1-Score Calculation

F1-score balances Precision and Recall into a single metric.

Formula:

F1 = 2 × ((Precision × Recall) / (Precision + Recall))

Using this dataset:

F1 = 2 × ((0.9722 × 0.8974) / (0.9722 + 0.8974))

F1 = 0.9333

F1 Score = 93.33%

Interpretation:
The model performs strongly overall while still struggling with subtle sentiment phrasing.

---

# Confidence Score Analysis

The dataset includes simulated confidence values to imitate real ML classifier probabilities.

## High Confidence Predictions

Most easy examples received confidence scores between:

- 0.92
- 0.99

These usually contain strong emotional language such as:

- "amazing"
- "terrible"
- "waste of money"
- "love it"

---

## Medium Confidence Predictions

More balanced reviews received confidence scores between:

- 0.80
- 0.89

Examples:
- "It does the job well enough."
- "It's somewhat useful in daily use."

These contain weaker emotional intensity.

---

## Low Confidence Predictions

Misclassified samples generally received confidence scores between:

- 0.55
- 0.66

Examples:
- "It's okay nothing special but works fine."
- "It's not great but not terrible either."

These examples intentionally simulate uncertain model behavior in ambiguous sentiment situations.

---

# Difficulty Tag Analysis

The dataset includes manual difficulty labels.

## Easy

Characteristics:
- Strong sentiment
- Clear emotional language
- Direct opinions

Examples:
- "I regret buying this product."
- "This works perfectly and I love it."

---

## Medium

Characteristics:
- Moderate emotional intensity
- Mixed wording
- Softer opinions

Examples:
- "It's somewhat useful in daily use."
- "I expected better quality for this price."

---

## Hard

Characteristics:
- Mixed polarity
- Neutral-positive wording
- Ambiguous sentiment
- Contradictory phrasing

Examples:
- "It's not great but not terrible either."
- "The product is good but too expensive for what it offers."

These difficult examples were intentionally included to simulate real NLP edge cases.

---

# Error Type Analysis

The dataset includes categorized error labels to support detailed ML evaluation.

## Error Categories Included

| Error Type | Description |
|---|---|
| neutral_misclassification | Neutral wording interpreted incorrectly |
| neutral_sentiment_miss | Weak positive sentiment predicted as negative |
| mixed_sentiment_confusion | Contradictory wording confused the classifier |
| polarity_conflict_price_bias | Positive and negative cues conflicted |
| value_sentiment_confusion | Pricing/value wording reduced prediction confidence |

---

# Why Extra Fields Were Added

The original dataset only supported basic annotation practice.

Additional fields were intentionally added to simulate professional machine learning evaluation pipelines.

## Added Fields

| Field | Purpose |
|---|---|
| prediction | Simulated model output |
| is_correct | Enables evaluation metrics |
| tp_fp_fn_tn | Supports confusion matrix analysis |
| error_type | Enables structured error analysis |
| confidence_simulated | Simulates model certainty |
| difficulty_tag | Represents annotation complexity |

These additions transform the dataset from a simple annotation set into a realistic ML evaluation project suitable for portfolio presentation.

---

# Intentional Errors

The dataset intentionally contains a small number of incorrect predictions.

This was done deliberately because real-world ML systems are never perfectly accurate.

Including controlled mistakes allows demonstration of:

- Precision
- Recall
- F1-score
- Error categorization
- Confidence analysis
- Ambiguous sentiment handling
- Evaluation reporting

Without prediction errors, meaningful evaluation metrics and error analysis would not be possible.

---

# Key Findings

## Strengths

- Strong overall accuracy
- Excellent precision
- Reliable detection of strong sentiment
- High confidence on easy examples

## Weaknesses

- Struggles with mixed sentiment
- Lower recall on weak-positive reviews
- Confusion around neutral wording
- Reduced certainty on ambiguous examples

---

# Conclusion

This project demonstrates a complete beginner-to-intermediate ML evaluation workflow for sentiment classification.

The repository now includes:

- Structured annotation data
- Simulated predictions
- Classification outcomes
- Error categories
- Confidence scoring
- Difficulty tagging
- Metric calculations
- Evaluation reporting

The project is intentionally designed to resemble real NLP quality analysis pipelines used in annotation operations and machine learning evaluation environments.
