# Customer Segmentation and Churn-Risk Model

## Project Overview

This project develops an explainable customer segmentation and rule-based churn-risk prioritization model.

## Objective

The objective is to move from descriptive customer analytics to transparent customer prioritization using behavioral and account features.

## Dataset

The analysis uses a sample customer churn dataset containing 15 customer records and 11 fields.

## Features Used

The model uses:

* Tenure
* Monthly Charges
* Total Charges
* Contract Type
* Support Tickets

Customer ID is used only as an identifier.

## Customer Segmentation

Customers are grouped using tenure and support-ticket activity into simple, explainable customer segments.

## Churn-Risk Score

The rule-based score uses:

* Short tenure: +2 points
* Month-to-month contract: +2 points
* Higher-than-median support tickets: +1 point

Risk levels:

* 0–1: Low Risk
* 2–3: Medium Risk
* 4–5: High Risk

## Validation

The model was checked for missing values, valid score ranges, missing risk classifications, and correct application of individual scoring rules.

Observed churn was used for validation and interpretation rather than as an input to the risk score.

## Limitations

The dataset contains only 15 customers. Therefore, the results should be treated as a demonstration and decision-support exercise rather than a production churn prediction model.

## Files

* `customer_segmentation_recommendation.ipynb` — Complete analysis notebook
* `customer_segment_risk_table.csv` — Customer segmentation and risk results
