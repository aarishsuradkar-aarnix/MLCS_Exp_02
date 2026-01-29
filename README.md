A Hybrid Machine Learning Approach for Phishing Detection — Documentation
Purpose

This documentation describes the problem framework, dataset strategy, hybrid feature engineering pipeline, classification methodology, evaluation process, and refinement workflow based on the hybrid machine learning approach proposed for phishing detection. The system aims to deliver accurate, efficient, and deployable detection of phishing URLs in real-world cybersecurity environments.

1. Problem Overview

The research focuses on binary classification of websites into phishing or legitimate categories using a hybrid machine learning model. The hybrid framework combines feature selection with classification to reduce computational complexity while preserving detection accuracy.

The objective is to design a system capable of adapting to evolving phishing techniques and supporting automated web security defenses.

2. Goals & Success Criteria
Primary Goals

Detection accuracy ≥ 90%

F1-score ≥ 0.88 for phishing class

Low inference latency suitable for real-time use

Secondary Goals

Minimized false positive rate

Generalization to unseen phishing patterns

Reduced feature redundancy

3. Data Summary
Data Sources

Public phishing repositories (PhishTank, OpenPhish)

Public cybersecurity datasets

Research benchmark datasets

Data Format

Structured feature datasets (CSV)

Label: phishing / legitimate

Bias & Privacy Considerations

No personal data collected

Diverse domain coverage

Balanced dataset handling

Removal of outdated samples

4. Feature Engineering

The hybrid model relies on optimized feature extraction and selection.

URL & Website Features

URL length and structure

Symbol frequency

Subdomain complexity

Presence of phishing keywords

Host-based indicators

Hybrid Optimization

Feature selection reduces dimensionality

Eliminates redundant attributes

Improves classification efficiency

5. Modeling Approach

The hybrid system integrates feature selection with supervised classification.

Classifiers Used

Decision Tree

Random Forest

Support Vector Machine

Feature selection is applied before classification to create a lightweight and accurate detection pipeline.

Explainability

Feature importance ranking

Transparent decision rules

Interpretable phishing indicators

6. Evaluation Strategy
Offline Metrics

Accuracy

Precision

Recall

F1-score

Operational Metrics

False positive rate

Stability across new datasets

Efficiency under real-time constraints

7. Versioning & Refinement Workflow

Continuous dataset updates

Periodic retraining

Performance monitoring

Documented experiment logs

Feature refinement based on drift detection

8. Reproducibility

Fixed random seed

Stored experiment configurations

Recorded dataset versions

Traceable model parameters

9. Ethics & Risk Considerations

Avoid unfair blocking of legitimate websites

Minimize false positives

Maintain explainability

Support human cybersecurity analysts

10. Architecture & Workflow

High-Level Pipeline

URL Collection

Feature Extraction

Hybrid Feature Selection

Supervised Classification

Decision Output

Feedback & Model Update

The workflow enables continuous learning and adaptation to emerging phishing threats.
