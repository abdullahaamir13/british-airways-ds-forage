# British Airways Data Science Job Simulation (Forage)

This repository contains my completed work for the **British Airways Data Science Virtual Experience Program** hosted on [Forage](https://www.theforage.com/simulations/british-airways/data-science-yqoz).

## Overview

The simulation involved two main tasks aimed at understanding how data science supports strategic decisions at British Airways:

### Task 1: Lounge Eligibility Strategy
- Grouped flights by `ARRIVAL_REGION`, `HAUL`, and `TIME_OF_DAY` to create a tiered lounge eligibility lookup.
- Calculated the **average number of eligible passengers** per lounge tier using historical seat class data.
- Derived lounge eligibility percentages using aggregated **mean values** to provide a scalable and interpretable rule-based system.
- Justified assumptions using real-world airline operations and loyalty program logic.

### Task 2: Booking Completion Prediction
- Objective: Predict whether a customer completes a flight booking.
- Data: 50,000 booking funnel records with class imbalance handled using **SMOTE**.
- Models: Compared **Random Forest** and **LightGBM** with a lowered threshold (0.3) to optimize recall.
- Key Insight: `booking_origin` had the strongest influence on customer conversion.

## Key Results

| Model         | Recall (Class 1) | ROC AUC | Precision (Class 1) |
|---------------|------------------|---------|----------------------|
| Random Forest | 72%              | 0.76    | 29%                  |
| LightGBM      | 74%              | 0.75    | 28%                  |

## Outcome

- Recommended deploying either model at a 0.3 threshold to improve recall.
- Insights support targeted marketing and re-engagement strategies.

## Tools & Techniques
- Python, Jupyter Notebook
- pandas, scikit-learn, LightGBM
- imbalanced-learn (SMOTE), matplotlib, seaborn

## Link to Simulation
[British Airways Data Science Simulation on Forage](https://www.theforage.com/simulations/british-airways/data-science-yqoz)