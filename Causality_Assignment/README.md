# 🧭 Crash Course in Causality  
### Understanding How Data Preparation Shapes Causal Inference

This repository contains three complete case studies created as part of the **Crash Course in Causality** — a structured exploration of how **data preparation decisions** (handling missing data, encoding, and confounder control) affect **causal inference** in machine learning.  

The course demonstrates that *clean data isn’t automatically causal data* — and that causal interpretation requires thoughtful preprocessing and domain reasoning.

---

## 📘 Project Overview

Each case study examines a real-world dataset through the lens of **causal inference**, combining:
- Theory and causal graph (DAG) formulation  
- Practical implementation using Python and [DoWhy](https://microsoft.github.io/dowhy/)  
- Interpretation of results with attention to confounders, mediators, and colliders  
- Short educational videos explaining each analysis  

---

## 🧩 Case Studies

### 1. 🚢 **Titanic Dataset — When Data Meets History**
**Objective:** Estimate the causal effect of **gender (`sex`)** on **survival (`survived`)**, controlling for socioeconomic and demographic factors.  

**Key Learnings:**
- Imputing missing ages and adding a `missing_age` indicator avoids selection bias.  
- One-Hot Encoding is preferred over Ordinal Encoding to prevent artificial order.  
- Confounders such as `class`, `fare`, and `age` influence both `sex` and `survival`.  
- The estimated Average Treatment Effect (ATE) for `sex_male` ≈ **–0.5**, meaning men had ~50% lower survival probability.  
- Demonstrates that *data preparation directly affects causal validity.*

**YouTube Videos:**  
- 🎬 [Screen Recording — “When Data Meets History: The Causal Truth Behind the Titanic Disaster”](https://youtu.be/H7yJYrAURcQ)  
- ✍️ [Story-Style Video — “From History to Data: The Human Side of Causality”](https://youtu.be/xjYsmYo6QcI)  

---

### 2. ☕ **Tips Dataset — Smoking and Tipping Behavior**
**Objective:** Investigate whether **being a smoker (`smoker`)** causes lower **tips (`tip`)**, controlling for contextual variables like bill size, day, time, and group size.  

**Key Learnings:**
- `smoker` is the treatment; `tip` is the outcome.  
- Confounders (`total_bill`, `size`, `day`, `time`, `sex`) affect both treatment and outcome.  
- Proper one-hot encoding prevents order bias in categorical variables.  
- The causal estimate shows a **negative effect** — smokers tend to tip less, even after adjusting for confounders.  
- Reinforces the principle that social behavior data must be causally adjusted before interpretation.

**Outcome:**  
A small, behavior-driven dataset can still demonstrate how **data preparation**, **confounder control**, and **causal reasoning** uncover insights into real human behavior.

---

### 3. 🚗 **Car Crashes Dataset — Alcohol and Road Safety**
**Objective:** Determine if **alcohol involvement (`alcohol`)** increases the **total number of crashes (`total`)** after adjusting for confounders such as speeding, distraction, and insurance costs.  

**Key Learnings:**
- `alcohol` → `total` is the treatment–outcome pair.  
- Confounders include `speeding`, `not_distracted`, `no_previous`, `ins_premium`, `ins_losses`, and `abbrev` (state).  
- One-hot encoding for states ensures each state’s baseline risk is modeled independently.  
- The **causal effect of alcohol is positive**, confirming that higher alcohol involvement causes higher crash rates.  
- Demonstrates the **policy relevance** of causal inference — separating correlation from actionable cause.

**Outcome:**  
Causal models reveal how societal and behavioral factors interact, providing a foundation for evidence-based policy and safety decisions.

---

## 🧠 What We Learned Across All Datasets

| Concept | Insight |
|----------|----------|
| **Missing Data Handling** | Imputation + missingness indicators preserve causal validity and prevent selection bias. |
| **Encoding Choices** | One-Hot Encoding prevents false ordering and maintains causal independence among categories. |
| **Confounder Control** | Correctly identifying and adjusting for confounders via the DAG is essential to unbiased estimation. |
| **DoWhy Framework** | Formalizes causal identification, estimation, and robustness checks through refutation tests. |
| **Interpretation** | Causal estimates (ATEs) quantify *how much* a treatment changes an outcome — beyond correlation. |
| **Ethical & Historical Context** | Real-world data, like the Titanic or crash statistics, remind us that each datapoint represents human consequences. |

---

## 📊 Tools and Libraries
- **Python 3.12+**
- [Seaborn](https://seaborn.pydata.org/) — built-in datasets (Titanic, Tips, Car Crashes)  
- [scikit-learn](https://scikit-learn.org/) — preprocessing, pipelines, and models  
- [DoWhy](https://microsoft.github.io/dowhy/) — causal modeling and refutation  
- [Graphviz](https://graphviz.org/) — DAG visualization  

---

## 🧩 Repository Structure

Crash_Course_in_Causality/
│
├── causality_titanic.ipynb # Titanic dataset analysis
├── causality_tips.ipynb # Tips dataset causal analysis
├── causality_car_crashes.ipynb # Car crashes dataset causal analysis
├── quizzes/
│ ├── titanic_quiz.md
│ ├── tips_quiz.md
│ └── car_crashes_quiz.md
└── README.md

## 🧩 Reflections

This project bridges **machine learning** and **causal reasoning**, showing that:
> “Better data cleaning doesn’t just improve accuracy — it changes the story we tell.”

Across datasets:
- *Titanic* reminded us how social class and gender shaped survival.  
- *Tips* highlighted behavioral economics in everyday interactions.  
- *Car Crashes* demonstrated the power of causal modeling in real-world policymaking.

Each case shows that **causal inference turns statistics into understanding** — transforming data from numbers into narratives of cause, effect, and consequence.

---

## 📚 References
- Pearl, J. (2009). *Causality: Models, Reasoning, and Inference.* Cambridge University Press.  
- Hernán, M. A., & Robins, J. M. (2020). *Causal Inference: What If.* Chapman & Hall/CRC.  
- Peters, J., Janzing, D., & Schölkopf, B. (2017). *Elements of Causal Inference.* MIT Press.  
- Microsoft Research. *DoWhy: A Python Library for Causal Inference.*  
- Seaborn Documentation. *Built-in Datasets.*  

---

## 🪪 License

This repository and its contents are licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.  

You are free to:  
- **Share** — copy and redistribute the material in any medium or format  
- **Adapt** — remix, transform, and build upon the material for any purpose, even commercially  

Under the following terms:  
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.  

Full License: [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
