# AI-Driven Loyalty Program Optimization for Retail Supermarkets in Kenya

**Capstone Group 2:** Sylvia, Clive, Ezekiel, Brenda, Isaiah  
**Date:** June 2025

---
## Overview
This project leverages AI to optimize loyalty programs for Kenyan supermarkets by analyzing customer data to boost retention, increase repeat purchases, and personalize promotions

## Business Context & Problem

- Traditional loyalty programs are generic and poorly targeted.
- Result in low engagement, inefficient promotions, and declining retention.
- Goal: Use AI to personalize loyalty strategies for Kenyan supermarkets.

---

## Project Objectives

1. Segment customers using behavioral data.
2. Predict customer churn.
3. Identify high-value customers to prioritize in retention strategies.

---
## Success Metrics
- Churn prediction accuracy ≥ 80%
- Clustering silhouette score > 0.45
- ROC-AUC score ≥ 90%

---

## Data Overview

Two main datasets were used:
- `customer_info.csv`: Demographics and customer metadata.
- `POS_Transactions.csv`: Transaction details including basket size and spend.
- Combined and engineered into RFM features and churn labels.

---

## Methodology

- Data cleaning and preprocessing.
- RFM analysis (Recency, Frequency, Monetary).
- Churn prediction with classification models.
- Customer segmentation with KMeans clustering.

---

## Deployment
A Streamlit dashboard that:
- Predicts customer churn using XGBoost
- Segments customers using KMeans clustering
- Uses RFM features (Recency, Frequency, Monetary)
- Provides evaluation plots (Confusion Matrix, ROC, Elbow, Silhouette)

### App Structure
```
loyalty_app/
├── app.py                # Main Streamlit app
├── utils.py              # Preprocessing, training, evaluation
├── xgboost_model.joblib  # Trained churn model
├── kmeans_model.joblib   # Trained segmenter
├── scaler.joblib         # Preprocessing scaler
```
Upload customer and transaction CSVs to generate insights.

---

## Churn Prediction Results

### Confusion Matrix
![Confusion Matrix](confusion_matrix.png)

> Interpretation: High true positives and negatives indicate strong model performance.

### ROC Curve
![ROC Curve](roc_curve.png)

> ROC-AUC score of 0.92 shows excellent discriminatory ability.

---

## Customer Segmentation

### Cluster Visualization
![Customer Segments](customer_segments.png)

> KMeans clustering identified 4 distinct groups, enabling targeted strategies.

---

## Business Insights

- Identify and prioritize high-value segments for tailored offers.
- Intervene early with customers predicted to churn.
- Allocate marketing budget efficiently using customer tiers.

---

## Recommendations

- Deploy churn model for regular customer monitoring.
- Personalize rewards based on customer segments.
- Conduct A/B testing on targeted promotions.

---

## Next Steps & Limitations

- Implement model feedback loop.
- Monitor and retrain on new data regularly.
- Consider additional features like in-store activity.
- Address potential model bias and data privacy concerns.

---

## More Information
Find the full analysis in the [Capstone jupyter notebook](./Group_2_Phase_5_Project_Capstone.ipynb) or this [presentation](./AI_Loyalty_Program_Presentation.pdf) and [project report](./Loyalty_Program_Project_Report.pdf).

For additional info, contact Capstone Group 2 Team
