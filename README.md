# reddit-behavior-analysis
## Project Overview

This project investigates how participation in toxic Reddit communities influences user behavior in mainstream subreddits. By analyzing 223 million comments across 18 subreddits, we quantify cross-community toxicity using the Toxic-Bert classifier.

### Research Question: Are users active in controversial subreddits more likely to exhibit toxicity in mainstream subreddits?

## Architecture / Pipeline Diagram
[User Data Collection] -> [Subreddit Classification (Mainstream vs Controversial)] -> [Toxic-Bert Classification] -> [User-Level Aggregation] -> [Analysis & Visualization]

<img width="357" height="214" alt="image" src="https://github.com/user-attachments/assets/8b8754db-50df-44c1-adde-6f5ee0634050" />

Toxicity Distribution Graph


## Tech Stack
Programming: Python
NLP & ML: Toxic-Bert, Transformers, ConvoKit
Data Analysis: Pandas, NumPy
Visualization: Matplotlib, Seaborn
Repository Management: GitHub

## Key Findings
Users in controversial subreddits score higher mean toxicity in mainstream subreddits (0.148 vs 0.140), ~22% more comments flagged toxic.
Behavior adapts to subreddit norms: users post less toxically outside their home subreddit.
Dose-response effect: more controversial subreddit participation → higher mainstream toxicity (0.140 → 0.152).

<img width="357" height="179" alt="image" src="https://github.com/user-attachments/assets/f766b858-80fd-4c90-bd20-900cc0717ec6" />

<img width="468" height="152" alt="image" src="https://github.com/user-attachments/assets/9c6e0255-45b9-400f-b91c-57f769066ddf" />

<img width="357" height="214" alt="image" src="https://github.com/user-attachments/assets/46b58c83-e59b-4ec5-8955-806ecd42cbd0" />

<img width="357" height="238" alt="image" src="https://github.com/user-attachments/assets/2cc099ee-2586-43bb-8f57-851f145062e8" />

<img width="273" height="182" alt="image" src="https://github.com/user-attachments/assets/04e4c51e-3dfc-4cf6-98e1-c2a015ff8392" />

Questions explored:

- Do users from toxic communities behave differently elsewhere?
- Does behavior transfer across communities?
- How strongly are community-level characteristics associated with individual behavior?

*Results and interpretations are discussed in the project report.*

---

## Challenges

The hardest challenge was designing a workflow that produced results I could trust.

Language is contextual and noisy:

- sarcasm can resemble toxicity
- community norms differ significantly
- model outputs require careful interpretation

This project pushed me beyond training models and toward thinking about complete ML systems, evaluation, and reproducibility.

---
## Future Improvements

If continuing this project, I would explore:

- Retrieval-augmented workflows (RAG)
- LLM-based contextual reasoning
- Agent-based analysis pipelines
- Improved evaluation frameworks
- Scalable deployment architecture

---

## Project Report

Full project write-up:

[Project Report](https://www.overleaf.com/project/69f25c25968926daaf9572b5)

---
