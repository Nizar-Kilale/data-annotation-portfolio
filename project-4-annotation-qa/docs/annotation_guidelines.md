# Annotation Guidelines — Sentiment Analysis Evaluation Project

## Project Overview

This project contains a manually reviewed sentiment analysis dataset designed for NLP annotation practice and machine learning evaluation workflows.

The dataset focuses on binary sentiment classification using short product-review-style text samples. Each sample was assigned a sentiment label and later extended with simulated machine learning evaluation metadata to support error analysis and metric calculation.

The project demonstrates:
- Manual sentiment annotation
- Dataset structuring
- Simulated model evaluation
- Error categorization
- Confidence scoring
- Precision, Recall, and F1-score analysis

Several controlled prediction mismatches were intentionally introduced to simulate realistic NLP model evaluation conditions and enable precision, recall, F1-score, and error analysis workflows.

---

# Sentiment Labels

## Positive

Assign the `Positive` label when the text expresses:
- Satisfaction
- Approval
- Recommendation
- Successful product experience
- Acceptable or favorable value

### Positive Examples
- “The product arrived quickly and works perfectly.”
- “Great quality and definitely worth the price.”
- “I’m very pleased with the results.”
- “Good value for the price.”

### Notes
Some positive samples may contain mild criticism while still expressing overall satisfaction.

Example:
> “It’s not the best but it’s acceptable.”

This remains labeled as Positive because the overall sentiment is acceptable rather than negative.

---

## Negative

Assign the `Negative` label when the text expresses:
- Disappointment
- Regret
- Frustration
- Poor quality
- Negative value perception
- Product failure

### Negative Examples
- “This is a complete waste of money.”
- “It arrived damaged and unusable.”
- “Too expensive for such low quality.”
- “I regret this purchase so much.”

### Notes
Negative labels are assigned based on overall sentiment, even when positive wording appears in the sentence.

Example:
> “The product is good but too expensive for what it offers.”

This is labeled Negative because the final sentiment outcome reflects dissatisfaction.

---

# Ambiguous and Mixed Sentiment Cases

Some dataset items intentionally contain:
- Mixed polarity
- Mild approval
- Neutral phrasing
- Contradictory wording

These examples were included to simulate realistic NLP classification challenges.

Examples:
- “It’s okay nothing special but works fine.”
- “It’s just average nothing impressive.”
- “It’s not great but not terrible either.”

These samples may confuse models because they contain both positive and neutral/negative language simultaneously.

---

# Evaluation Metadata Fields

The dataset was extended beyond standard annotation labels to simulate a realistic machine learning evaluation environment.

## prediction

Represents the simulated NLP model output.

Example:
```json
"prediction": "Negative"
```

This field allows comparison between:
- Human annotation (`label`)
- Model output (`prediction`)

---

## is_correct

Boolean field indicating whether the model prediction matches the human label.

Example:
```json
"is_correct": true
```

---

## tp_fp_fn_tn

Represents confusion matrix classification categories.

Possible values:
- TP = True Positive
- TN = True Negative
- FP = False Positive
- FN = False Negative

This field supports:
- Precision calculation
- Recall calculation
- F1-score analysis
- Error distribution analysis

---

## error_type

Used to categorize model failure patterns.

Examples include:
- `neutral_misclassification`
- `mixed_sentiment_confusion`
- `value_sentiment_confusion`
- `polarity_conflict_price_bias`

### Purpose
This field demonstrates structured NLP error analysis beyond simple accuracy measurement.

---

## confidence_simulated

Represents simulated model confidence scores ranging from 0 to 1.

Example:
```json
"confidence_simulated": 0.97
```

### Confidence Interpretation
- High confidence (0.90–0.99):
  Clear sentiment expression

- Medium confidence (0.75–0.89):
  Mild ambiguity or softer wording

- Lower confidence (0.50–0.74):
  Mixed sentiment or neutral phrasing

These values were intentionally simulated to imitate real-world model output probabilities.

---

## difficulty_tag

Represents estimated annotation or classification difficulty.

Possible values:
- easy
- medium
- hard

### Difficulty Logic

#### Easy
Clear emotional polarity.

Example:
> “This is a complete waste of money.”

#### Medium
Contains softer or partially mixed sentiment.

Example:
> “It does the job well enough.”

#### Hard
Contains ambiguity, conflicting sentiment, or neutral-positive overlap.

Example:
> “It’s not great but not terrible either.”

---

# Batch Structure

The dataset is divided into three batches:

## B1 — Basic Sentiment
Contains straightforward positive and negative sentiment examples.

Focus:
- Clear polarity
- High-confidence classification

---

## B2 — Ambiguous and Mixed Sentiment
Introduces:
- Neutral wording
- Mixed polarity
- Mild sentiment expressions

Focus:
- Error simulation
- Harder classification scenarios

---

## B3 — Value and Price-Based Sentiment
Focuses on:
- Cost vs quality reasoning
- Value perception
- Price-related polarity conflicts

These examples simulate real-world e-commerce review complexity.

---

# Intentional Error Injection

Several incorrect predictions were intentionally added to:
- Simulate NLP model limitations
- Enable confusion matrix generation
- Support realistic evaluation metrics
- Demonstrate structured error analysis

These intentional mismatches help showcase:
- Precision
- Recall
- F1-score
- Failure pattern analysis

within a controlled educational dataset.

---

# Project Purpose

This repository was created as a practical NLP annotation and evaluation portfolio project demonstrating:
- Data annotation workflows
- Sentiment classification logic
- Dataset structuring
- Evaluation methodology
- Error analysis techniques
- Machine learning metric interpretation

The project is intended for educational and portfolio demonstration purposes.
