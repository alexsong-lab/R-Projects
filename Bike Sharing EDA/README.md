# Exploratory Analysis of Bike Sharing Usage — DATA 5321 Project (Part 1 of 4 Phases)

This project is the first phase of a four‑part analysis focused on understanding how various factors influence daily bike‑sharing usage. Using the bike‑sharing dataset provided for the course, this phase centers on exploratory data analysis and initial regression modeling to uncover relationships between daily usage counts and key predictor variables.

The work in this phase uses **2011 data as the training set** and **2012 data as the test set**, following the project’s longitudinal structure.

---

## **Purpose**

Over the course of the quarter, this project will progress through exploratory analysis, model development, model evaluation, and communication of results. Part 1 establishes the foundation by:

- Exploring the structure and behavior of the dataset  
- Understanding how individual predictors relate to daily usage  
- Building and evaluating simple and interaction‑based regression models  
- Preparing for model selection and validation in later phases  

This phase emphasizes clear, interpretable analysis that informs future modeling decisions.

---

## **Dataset Description**

The dataset contains daily bike‑sharing usage information for **2011 and 2012**. For this phase, analysis focuses on the **daily counts** variable:

- **cnt** — total daily bike‑sharing usage (response variable)

Predictor variables include:

- **season**  
- **mnth**  
- **holiday**  
- **weekday**  
- **workingday**  
- **weathersit**  
- **temp**  
- **atemp**  
- **hum**  
- **windspeed**

Descriptions for each variable are available in the dataset documentation.

---

## **Report Requirements**

## **1. Exploratory Data Analysis (2011 Data)**

Conduct a thorough exploratory analysis of the 2011 training dataset, including:

- Numerical summaries for each variable  
- Visual summaries (histograms, boxplots, scatterplots, etc.)  
- Observations about distributions, patterns, and potential issues  

This section establishes an understanding of the data before modeling.

---

## **2. Individual Regression Models (2011 Data)**

Fit **separate simple linear regression models** predicting **cnt** using each predictor variable individually.

For each model:

- Evaluate model fit  
- Assess regression assumptions (linearity, residual behavior, etc.)  
- Comment on the usefulness and limitations of each predictor  

---

## **3. Two‑Variable Models with Interaction Effects**

Fit **at least three** regression models that include:

- Two predictor variables  
- An interaction term between them  

Discuss:

- Why each interaction was chosen  
- Whether the interaction appears meaningful  
- How the interaction changes interpretation of the predictors  

---

## **4. Backward Selection for a Final Model**

Starting with:

- All predictor variables  
- The interaction terms explored in Section 3  

Use **backward selection** to determine a final model based on the 2011 data.

Then:

- Interpret the final model  
- Explain how each included predictor relates to daily usage  
- Discuss why certain variables or interactions were removed  

---

## **5. Model Evaluation on 2012 Data**

Apply the final model from Section 4 to the **2012 test dataset**.

Discuss:

- How well the model generalizes  
- Whether predictive performance is consistent across years  
- What this suggests about the model’s reliability  

This step sets the stage for more advanced modeling in later phases.

---

## **Project Structure**

```
├── data/                 # 2011 and 2012 bike-sharing datasets
├── rmd/                  # R Markdown files for analysis and reporting
├── reports/              # Rendered reports (HTML/PDF)
├── scripts/              # Supporting R scripts (optional)
└── README.md             # Project documentation
```

---

## **Tools and Libraries**

This phase uses R and common data analysis packages, including:

- dplyr / tidyr — data wrangling  
- ggplot2 — visualization  
- stats — regression modeling  
- broom — model tidying (optional)  
- R Markdown — report generation  

---

## **Learning Outcomes**

By completing Part 1, students will learn to:

- Conduct exploratory analysis on real‑world datasets  
- Build and interpret simple and interaction‑based regression models  
- Evaluate regression assumptions  
- Apply model selection techniques  
- Assess model generalization using a test dataset  
- Communicate findings clearly and effectively  
