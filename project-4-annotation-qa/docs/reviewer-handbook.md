# Reviewer Handbook

## Overview

This handbook defines operational rules and decision-making standards for annotation QA reviewers.

It ensures consistent, objective, and reproducible evaluation of annotated datasets across all NLP tasks in this project.

---

# 1. Core Reviewer Responsibility

The primary responsibility of a reviewer is to ensure:

- annotation accuracy
- label consistency
- completeness of annotations
- adherence to guidelines
- dataset reliability for downstream ML use

Reviewers do not introduce personal interpretation outside defined rules.

---

# 2. Decision-Making Principles

## 2.1 Guideline Priority

All review decisions must follow:
1. Project annotation guidelines
2. Error taxonomy definitions
3. Existing dataset patterns (consistency rule)

If conflicts arise, guidelines take priority.

---

## 2.2 Consistency Rule

Similar inputs must receive similar annotation treatment.

Inconsistent labeling is considered a high-severity issue.

---

## 2.3 Minimal Assumption Policy

Reviewers must avoid:
- guessing missing information
- inferring unsupported meanings
- introducing external knowledge not present in data

Only contextually supported decisions are allowed.

---

# 3. Handling Edge Cases

## 3.1 Ambiguous Inputs

If an example is unclear:

- check guidelines first
- compare similar labeled cases
- apply consistency logic
- document uncertainty if needed

---

## 3.2 Low Confidence Decisions

If reviewer confidence is low:

- mark case for secondary review
- document reasoning
- avoid final irreversible decisions

---

# 4. Correction Standards

All corrections must:

- follow taxonomy definitions
- include clear justification
- maintain dataset consistency
- avoid subjective bias

Major corrections require reviewer notes explaining:
- issue identified
- correction applied
- reason for decision

---

# 5. Quality Expectations

Reviewers are expected to maintain:

- high labeling accuracy
- consistent annotation behavior
- strict adherence to schema
- reproducible decision logic

---

# 6. Professional Conduct Model

This system simulates real-world annotation QA environments.

Reviewers should behave as if:
- dataset quality impacts production ML systems
- inconsistencies affect model performance
- precision and recall depend on their decisions

---

# 7. Final Rule

When uncertain, prioritize:
> consistency over assumption
> guideline adherence over intuition
