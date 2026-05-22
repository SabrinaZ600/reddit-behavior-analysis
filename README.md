# Reddit Behavior Analysis: Toxicity & Cross-Community Spillover

End-to-end NLP pipeline for analyzing how participation in controversial online communities influences user behavior across mainstream Reddit spaces.

## Project Overview

Social media behavior is highly contextual, but an open question is whether participation in toxic communities changes how users behave elsewhere.

This project analyzes **223+ million Reddit comments across 18 subreddits** to investigate whether users active in controversial communities exhibit measurable differences in toxicity when interacting in unrelated mainstream spaces.

Rather than classifying isolated comments, the goal was to transform large-scale unstructured text into structured behavioral representations and identify broader patterns across users and communities.

### Research Question

**Are users active in controversial subreddits more likely to exhibit toxic behavior in mainstream subreddits?**

---

## System Pipeline

```text
Raw Reddit Data
        ↓
ConvoKit Collection & Filtering
        ↓
Subreddit Classification
(Mainstream vs Controversial)
        ↓
Text Preprocessing
        ↓
Toxic-BERT Classification
        ↓
User-Level Feature Engineering
        ↓
Behavioral Analysis
        ↓
Visualization & Interpretation
```
<img width="357" height="214" alt="image" src="https://github.com/user-attachments/assets/8b8754db-50df-44c1-adde-6f5ee0634050" />

Toxicity Distribution Graph

---

## Technical Stack

### Languages
- Python

### NLP / Machine Learning
- Hugging Face Transformers
- Toxic-BERT
- ConvoKit

### Data Processing
- Pandas
- NumPy

### Visualization
- Matplotlib
- Seaborn

---

## Key Results

### Cross-community toxicity spillover

Users active in controversial communities exhibited higher mean toxicity scores in mainstream communities:

- Controversial users: **0.148**
- Mainstream-only users: **0.140**

This corresponded to approximately **22% more comments classified as toxic.**

### Behavioral adaptation effect

Users moderated their behavior outside their primary communities, suggesting adaptation to different community norms.

### Dose-response relationship

Higher participation in controversial communities was associated with increasing toxicity levels:

0.140 → 0.152

suggesting a measurable relationship between participation intensity and behavioral outcomes.

<img width="357" height="179" alt="image" src="https://github.com/user-attachments/assets/f766b858-80fd-4c90-bd20-900cc0717ec6" />

<img width="468" height="152" alt="image" src="https://github.com/user-attachments/assets/9c6e0255-45b9-400f-b91c-57f769066ddf" />

<img width="357" height="214" alt="image" src="https://github.com/user-attachments/assets/46b58c83-e59b-4ec5-8955-806ecd42cbd0" />

<img width="357" height="238" alt="image" src="https://github.com/user-attachments/assets/2cc099ee-2586-43bb-8f57-851f145062e8" />

<img width="273" height="182" alt="image" src="https://github.com/user-attachments/assets/04e4c51e-3dfc-4cf6-98e1-c2a015ff8392" />


---

## Technical Challenges

The most difficult challenge was not model training—it was building a workflow that generated reliable conclusions.

Challenges included:

- sarcasm and contextual language affecting toxicity scores
- differing norms across communities
- preserving user-level relationships across large datasets
- preventing misleading conclusions from correlations alone

This project pushed me from thinking about individual model outputs to thinking about reproducible ML systems.

---

## Future Directions

Potential extensions:

- Retrieval-Augmented Generation (RAG) workflows
- LLM-based contextual reasoning
- Agent-based behavioral analysis pipelines
- Improved evaluation and benchmarking frameworks
- Scalable deployment architecture

---

## Project Report

Full write-up:

[Project Report](YOUR_LINK)

---
