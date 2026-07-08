# Forecasting-Spare-parts-inventory
 AI-powered Spare Parts Inventory Forecasting system using MySQL &amp; Python to predict vehicle service demand and achieve Just-In-Time (JIT) management.

## 📖 Introduction

Inventory management is one of the most critical functions in vehicle service centers. Service centers must maintain a delicate balance: sustaining a sufficient spare parts inventory to meet instant customer repair demands while simultaneously minimizing warehouse storage and long-term operational costs. 

### ⚠️ The Core Challenge
Predicting the exact demand for automotive spare parts is uniquely challenging because it depends on an intertwined matrix of highly variable factors:
*   **Vehicle Specifications:** Different makes and models require highly specialized replacement components.
*   **Service Frequency:** Variations in how often individual clients visit the repair bays.
*   **Vehicle Mileage & Lifecycle:** Odometer progression dictates when specific parts naturally reach their mechanical wear thresholds.
*   **Erratic Maintenance Patterns:** Unpredictable emergency breakdowns versus routine scheduled tune-ups.

Poor inventory planning triggers severe operational risks on both ends of the spectrum. **Excess stock** ties up vital capital and inflates overhead holding costs. Conversely, **insufficient stock** creates severe service delays, gridlocks repair bays, and drives customer dissatisfaction.

### 💡 The Data-Driven Solution
With the growth of data-driven technologies, **Data Science** and **Machine Learning** have emerged as exceptionally powerful tools for solving modern supply chain bottlenecks. By mining historical maintenance footprints, organizations can replace human guesswork with predictive analytics to optimize their stock levels automatically. This system enables service centers to:
1.  Uncover deep, underlying components usage patterns.
2.  Instantly flag high-demand, fast-moving spare parts.
3.  Accurately forecast future consumption trends across multiple horizons.

### 🎯 Project Scope & Ultimate Goal
This project focuses on developing an intelligent **Spare Parts Inventory Forecasting System** that hooks directly into historical service center operational records securely housed in a **MySQL database**. 

By applying robust, Python-based data science workflows—including detailed data preprocessing, multi-variable Exploratory Data Analysis (EDA), regression machine learning models, and statistical time-series forecasting—the pipeline translates raw transactional text into actionable supply chain metrics. 

The ultimate goal of this system is to transition automotive service centers into a strict **Just-In-Time (JIT) Inventory Management** standard. This protocol ensures that critical spare parts appear seamlessly in the workshop exactly when needed, without forcing the business to maintain expensive, excessive physical stock.


# 🚗 Vehicle Service Center: Spare Parts Inventory Forecasting System

An end-to-end data science and machine learning pipeline designed to optimize spare parts inventory management in automotive service centers. By extracting and analyzing **28,484 historical service transaction records** from a central **MySQL database**, this system predicts future component demand. 

The ultimate objective of this system is to transition service operations toward a **Just-In-Time (JIT)** inventory framework—ensuring critical replacement parts are exactly where they need to be, right when a customer pulls into the service bay, while minimizing warehouse storage costs.

---

## 🎯 Project Objectives

*   **Database Ingestion:** Securely extract operational service center data directly from a relational MySQL database.
*   **Data Sanitation:** Perform rigorous preprocessing and cleaning to resolve data inconsistencies and handle missing values across transaction blocks.
*   **Exploratory Data Analysis (EDA):** Conduct deep analytical visualizations to identify hidden seasonal patterns and usage trends in spare parts consumption.
*   **Machine Learning Modeling:** Develop predictive machine learning models to map parts demand against mileage and vehicle behavior.
*   **Time-Series Forecasting:** Implement statistical time-series forecasting techniques to analyze and project future long-term demand trends.
*   **JIT Implementation:** Support service centers in achieving Just-In-Time (JIT) standards to reduce inventory holding and storage costs while ensuring parts availability.

---

## 📊 Dataset & Feature Description

The system processes a dataset containing **28,484 operational records** consisting of 7 core engineering attributes:

| # | Feature Name | Data Type | Structural Description |
|---|---|---|---|
| **1** | `invoice_date` | Object (Date/Time) | The date when the service invoice was generated after maintenance completion. Tracks when parts were officially billed. |
| **2** | `job_card_date` | Object (Date/Time) | The date when the service request or job card was created. Indicates when the servicing process began. |
| **3** | `business_partner_name` | Object (Categorical) | The name of the customer or organization that owns the vehicle being serviced. |
| **4** | `vehicle_no` | Object (Identifier) | Unique vehicle registration number used as a core key for tracking lifetime maintenance history. |
| **5** | `vehicle_model` | Object (Categorical) | The specific model of the vehicle. Dictates the specialized spare parts and maintenance procedures required. |
| **6** | `current_km_reading` | Integer (Numerical) | Odometer reading of the vehicle at the time of servicing. Crucial for correlation against component wear thresholds. |
| **7** | `invoice_line_text` | Object (Text/Cat) | Detailed description of the specific spare parts or service items consumed during the vehicle servicing. |

---

## 🧠 Importance of Inventory Forecasting

Maintaining an un-optimized warehouse layout causes severe operational bottlenecks. Implementing predictive data analytics yields major supply chain advantages:
*   📉 **Cost Containment:** Dramatically reduces inventory holding, depreciation, and warehouse storage costs.
*   🚫 **Shortage Prevention:** Eliminates service bay bottlenecks and part stockouts.
*   ⚡ **Operational Productivity:** Boosts technician efficiency by ensuring components are available on demand.
*   🤝 **Customer Satisfaction:** Enhances customer retention rates by mitigating vehicle repair and turnaround delays.

---

.  **Extraction:** Designing optimized SQL queries to fetch clean relational records across service tables.
2.  **Feature Engineering:** Converting object datetime strings into computational index intervals and restructuring text descriptions into uniform part categories.
3.  **Visual Analytics:** Mapping consumption frequency histograms, tracking mileage-to-wear ratios, and running structural seasonality checks.
4.  **Predictive Pipelines:** Training regression frameworks and time-series forecasting models to compute demand limits.
5.  **Statistical Diagnostics:** Assessing model reliability through error metrics (MAE, RMSE) to guarantee safe deployment profiles inside active service centers.


## 🔭 Scope of Work

1.  **Extraction:** Designing optimized SQL queries to fetch clean relational records across service tables.
2.  **Feature Engineering:** Converting object datetime strings into computational index intervals and restructuring text descriptions into uniform part categories.
3.  **Visual Analytics:** Mapping consumption frequency histograms, tracking mileage-to-wear ratios, and running structural seasonality checks.
4.  **Predictive Pipelines:** Training regression frameworks and time-series forecasting models to compute demand limits.
5.  **Statistical Diagnostics:** Assessing model reliability through error metrics (MAE, RMSE) to guarantee safe deployment profiles inside active service centers.
