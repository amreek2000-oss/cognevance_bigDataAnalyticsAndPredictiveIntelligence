# 📊 Big Data Analytics & Predictive Intelligence System
**Cognevance Technologies — Level 3 Advanced Internship Capstone Project**

---

## 📌 Executive Summary
This project delivers a comprehensive, end-to-end **Big Data Analytics & Predictive Intelligence Pipeline** built for large-scale healthcare decision-making. Operating on a dataset of **55,501 patient records** across 15 analytical attributes, the pipeline bridges operational gaps in healthcare administration—including bed availability bottlenecks, clinical capacity constraints, and discharge management.

By integrating **Automated Data Preprocessing**, **In-Memory SQL Warehousing**, **Scikit-Learn Machine Learning Architecture**, and **Executive Visual Dashboards**, this system enables hospital administrators to accurately predict patient **Length of Stay (LOS)** and optimize clinical resource allocation.

---

## 🏗️ End-to-End System Architecture

```text
+-----------------------------------------------------------------------------------+
|                               RAW DATASET                                         |
|                          (55,501 Patient Records)                                 |
+-----------------------------------------------------------------------------------+
                                          │
                                          ▼
+-----------------------------------------------------------------------------------+
|                        DATA CLEANING & FEATURE ENGINEERING                        |
|   • Datetime standardization              • Null values median/mode imputation    |
|   • Duplicate detection & removal          • Length of Stay (LOS) Feature Creation  |
+-----------------------------------------------------------------------------------+
                                          │
                    ┌─────────────────────┴─────────────────────┐
                    ▼                                           ▼
+---------------------------------------+   +---------------------------------------+
|        SQL RELATIONAL ANALYTICS       |   |       MACHINE LEARNING ENGINE         |
|     (SQLite In-Memory Engine)         |   |      (Random Forest Regressor)        |
|  • Macro KPIs (Average Stay, Age)     |   |  • Encoding & Standard Scaling        |
|  • Medical Condition Proportions      |   |  • 80/20 Train-Test Dataset Split     |
|  • Admission Type Breakdown           |   |  • Model Evaluation (MAE, RMSE, R²)   |
+---------------------------------------+   +---------------------------------------+
                    │                                           │
                    └─────────────────────┬─────────────────────┘
                                          ▼
+-----------------------------------------------------------------------------------+
|                       OUTPUT GENERATION & DASHBOARD visual                        |
|   • cleaned_healthcare_data.csv            • ml_predictions.csv                   |
|   • analytics_dashboard_preview.png        • Executive Dashboard Integration      |
+-----------------------------------------------------------------------------------+
