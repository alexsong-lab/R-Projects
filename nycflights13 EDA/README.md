# Analysis of United Airlines Flight Delays and Flight Gains Using nycflights13

This project uses data from the **nycflights13** package to analyze two major operational metrics for United Airlines (carrier code **UA**):  
1. Departure delays  
2. Net flight gains (how much time a flight makes up or loses relative to schedule)

The work is presented through two R Markdown reports written for a **general, non‑technical audience**, focusing on clear explanations, accessible visualizations, and interpretable statistical results. The analysis incorporates exploratory data analysis, permutation tests, confidence intervals, and hypothesis testing.

---

## **Purpose**

This combined project develops skills in:

- Exploratory data analysis  
- Communicating results to non‑technical stakeholders  
- Working with real flight and weather data  
- Creating new variables to measure operational performance  
- Applying permutation tests, confidence intervals, and hypothesis tests  
- Producing clear, accessible visualizations in R  

The goal is to provide insights that could help United Airlines improve efficiency and customer satisfaction.

---

# Part 1 — Departure Delay Analysis

---

## **Overview**

The first part of the project investigates **departure delays** for United Airlines flights departing from New York City. The analysis examines how delays relate to:

1. Time of day  
2. Time of year  
3. Temperature  
4. Wind speed  
5. Precipitation  
6. Visibility  

The report uses exploratory data analysis and permutation tests to evaluate these relationships.

---

## **1. Introduction**

This section explains:

- The motivation for studying departure delays  
- The data sources used (flights and weather from nycflights13)  
- Why delays matter for airline operations and customer satisfaction  
- The overall goals of the analysis  

The introduction is written for a general audience without technical terminology.

---

## **2. Data Methodology**

Describe how the data was prepared:

- Loading flights and weather data in R  
- Filtering for United Airlines flights  
- Cleaning and merging datasets  
- Creating any new variables (e.g., late, very_late)  
- Handling missing values  

All steps are explained clearly and without assuming prior knowledge.

---

## **3. Results**

For each factor (time of day, time of year, temperature, wind speed, precipitation, visibility):

- Present exploratory visualizations created in R (ggplot2)  
- Use descriptive labels rather than variable names  
- Include permutation tests where appropriate  
- Interpret the results in plain language  

The focus is on what the patterns mean, not on technical details.

---

## **4. Discussion**

Summarize:

- The main findings  
- Which factors appear most strongly related to delays  
- Limitations of the analysis  
- Ideas for future follow‑up work  

---

# Part 2 — Flight Gain Analysis

---

## **Overview**

The second part of the project investigates **flight gains**, defined as how much time a flight makes up (or loses) relative to its schedule. The key variable is:

**Net Gain = Departure Delay − Arrival Delay**

A positive value means the flight arrived earlier than expected relative to its delayed departure; a negative value means it lost additional time.

The analysis uses exploratory data analysis, confidence intervals, and hypothesis tests to answer several operational questions.

---

## **1. Introduction**

Explain:

- The concept of flight gain and why it matters  
- The data used (flights and weather from nycflights13)  
- The purpose of creating a new variable for net gain  
- The operational context for United Airlines  

This section is written for a general audience.

---

## **2. Data Methodology**

Describe:

- How the net gain variable was created in R  
- Any additional variables (e.g., gain per hour)  
- How flights were filtered and cleaned  
- How missing or inconsistent data was handled  

---

## **3. Results**
### **A. Does the average gain differ for flights that departed late versus those that did not?**  
Use confidence intervals or hypothesis tests.

### **B. What about flights that departed more than 30 minutes late?**  
Analyze whether these flights make up more time.

### **C. What are the five most common destination airports for United Airlines flights?**  
For each of the top five destinations:

- Describe the distribution of gains  
- Report the average gain  
- Include appropriate visualizations  

### **D. Gain per hour**  
Create a new variable:

**Gain per Hour = Net Gain ÷ (Flight Duration in Hours)**

Then analyze:

- Whether gain per hour differs for late vs. on‑time departures  
- Whether gain per hour differs for flights delayed more than 30 minutes  
- Whether gain per hour differs for longer vs. shorter flights  

Each subsection includes:

- Graphs  
- Numerical summaries  
- Confidence intervals and/or hypothesis tests  
- Clear interpretations  

---

## **4. Discussion**

Summarize:

- The main takeaways from the flight gain analysis  
- Operational insights for United Airlines  
- Limitations of the study  
- Potential follow‑up analyses (e.g., aircraft type, route distance, weather interactions)  

---

# Project Structure

```
├── data/                 # nycflights13 data (if exported)
├── rmd/                  # R Markdown files for both analyses
├── reports/              # Rendered HTML/PDF reports and visualizations
├── scripts/              # Supporting R scripts (optional)
└── README.md             # Project documentation
```

---

## **Tools and Libraries**

- R  
- nycflights13  
- dplyr / tidyr for data manipulation  
- ggplot2 for visualization  
- infer or similar packages for permutation tests  
- broom, stats, or custom functions for confidence intervals and hypothesis tests  
- R Markdown for reporting  

---

## **Learning Outcomes**

By completing this combined project, students will learn to:

- Analyze real‑world flight and weather data in R  
- Communicate findings clearly to non‑technical audiences  
- Apply exploratory data analysis techniques  
- Use permutation tests, confidence intervals, and hypothesis tests  
- Create and interpret new operational metrics such as net gain and gain per hour  
- Produce polished, accessible reports using R Markdown  