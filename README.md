# Essay-Scoring-Model
A light AI model to grade and assess student essays as well as a full exploration of what makes an essay "good" semantically.

---

## Data


This project uses the **ASAP Automated Student Assessment Prize dataset**, which contains:

• 24,000+ student essays
• Human grading scores
• Essay prompts and source texts
• Demographic indicators

The dataset is commonly used for research in **automated essay scoring (AES)**.

You may view the dataset here: [Kaggle Dataset](https://www.kaggle.com/datasets/lburleigh/asap-2-0).

---

# AI Essay Grading Analysis: Can Machine Learning Approximate Teacher Evaluation?

This project explores whether machine learning can approximate human essay grading and what features of student writing influence scoring. Using the **ASAP Automated Essay Scoring dataset**, we perform semantic exploratory data analysis, build predictive models, and analyze where AI grading succeeds and fails.

The project was developed as part of a series on **AI in Education**, focusing on how data science can help us understand learning outcomes in the classroom.

---

# Project Overview

Teachers spend significant time grading written assignments. With the rise of AI tools in education, automated essay scoring has become an area of increasing interest.

This project investigates three key questions:

• What characteristics of essays correlate with higher scores?
• Can machine learning approximate human grading patterns?
• Where does AI grading perform poorly or introduce bias?

To answer these questions, we analyze over **24,000 student essays**, extract linguistic features, train predictive models, and evaluate AI grading behavior.

---

# Notebook 1: Semantic Exploratory Data Analysis

The first notebook explores patterns in student writing and grading.

### Feature Engineering

We extract interpretable linguistic features including:

* Word count
* Sentence count
* Average sentence length
* Vocabulary richness
* Readability score

We also perform **semantic analysis** using:

* Topic modeling (LDA)
* Sentence embeddings
* UMAP semantic visualization
* Essay clustering

### Key Questions Explored

• Do longer essays receive higher scores?
• Does vocabulary diversity impact grading?
• What topics appear most frequently in essays?
• Can we visualize essay meaning in semantic space?

### Example Visualizations

* Score distribution
* Essay length vs score
* Vocabulary richness vs score
* Topic cluster distribution
* Semantic map of essays

---

# Notebook 2: Predicting Essay Scores

In the second notebook, we train machine learning models to predict essay scores using engineered features.

### Models Used

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor

The goal is not to build a production model, but to examine **how well simple interpretable features approximate teacher grading**.

### Evaluation Metrics

* RMSE (Root Mean Squared Error)
* R² Score

### Key Insight

Even simple models can approximate grading patterns surprisingly well when using basic writing features.

---

# Notebook 3: AI Grading Behavior & Fairness

The final notebook evaluates how the AI grading model behaves compared to human graders.

We analyze:

• Prediction error distribution
• Error by essay score
• Error by essay length
• Error by essay topic

### Key Questions

• Does AI overgrade or undergrade certain essays?
• Are short essays harder to evaluate?
• Are certain essay topics more difficult for the model?

---

# Key Findings

Some of the main observations from the analysis include:

• **Essay length strongly correlates with score**
• **Vocabulary diversity is associated with higher scoring essays**
• Machine learning models can approximate teacher grading within about **one point on average**
• AI grading errors tend to increase for **very short essays and extreme scores**

These findings highlight both the **potential and limitations of automated grading systems**.

---

# Technologies Used

Python
Pandas
Scikit-learn
Sentence Transformers
UMAP
Seaborn
Matplotlib

The analysis was developed using **Google Colab notebooks**.

---

# Educational Context

This project was developed as part of a broader exploration of **AI applications in education**, including:

* Automated assessment
* AI-assisted teaching tools
* Data-driven learning analysis

While automated grading can assist educators, this project emphasizes the importance of **transparency, interpretability, and fairness** in educational AI systems.

---

Key Results

• AI predicted essay scores within ~1 point of human graders
• Essay length and vocabulary richness were the strongest predictors
• Short essays and extreme scores produced the largest errors
• Semantic clusters revealed distinct writing styles among essays

---
