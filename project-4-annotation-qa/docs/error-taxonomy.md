# Error Taxonomy

## Overview

This document defines the error classification framework used during annotation QA review.

The taxonomy standardizes how annotation issues are identified, categorized, and corrected across all reviewed NLP datasets.

A structured taxonomy improves:
- reviewer consistency,
- quality measurement,
- dataset reliability,
- correction tracking.

---

# Error Categories

## 1. Label Error

### Definition
The annotation label assigned is incorrect for the given example.

### Examples
- PERSON labeled as ORGANIZATION
- Positive sentiment labeled Negative
- Informational intent labeled Transactional

### Severity
High

---

## 2. Boundary Error

### Definition
The annotation captures only part of the correct span or includes unnecessary text.

### Examples

Correct:
New York City

Incorrect:
- York City
- New York

### Severity
Medium to High

---

## 3. Missing Annotation Error

### Definition
A required annotation was omitted entirely.

### Examples
- Missing named entity
- Missing sentiment indicator
- Missing relevance signal

### Severity
High

---

## 4. Over-Annotation Error

### Definition
Text was annotated unnecessarily or beyond guideline requirements.

### Examples
- Common noun labeled as entity
- Irrelevant result marked highly relevant

### Severity
Medium

---

## 5. Consistency Error

### Definition
Similar examples receive inconsistent annotation treatment across the dataset.

### Examples
- Same entity labeled differently
- Different intent decisions for equivalent queries

### Severity
High

---

## 6. Formatting Error

### Definition
Annotation structure or formatting does not follow project standards.

### Examples
- Invalid label formatting
- Incorrect casing
- Broken CSV schema

### Severity
Low to Medium

---

## 7. Ambiguity Resolution Error

### Definition
The annotation fails to handle ambiguous cases according to guideline standards.

### Examples
- Unsupported assumption
- Inconsistent interpretation of unclear context

### Severity
Medium to High

---

# Severity Levels

| Severity | Description |
|---|---|
| Low | Minor issue with minimal downstream impact |
| Medium | Noticeable quality issue affecting consistency |
| High | Critical issue affecting dataset reliability and model training quality |

---

# Reviewer Notes Requirement

All High severity corrections should include:
- explanation of the issue,
- correction reasoning,
- reference to applicable guidelines where necessary.
