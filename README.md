# DevelopersHub-Co.-Advanced-Tasks

This repository contains solutions for three core data science tasks, demonstrating proficiency in classification, unsupervised clustering, and time-series forecasting. Each project focuses on end-to-end implementation—from data preprocessing to model interpretability and evaluation.

***

## Task 1: Term Deposit Subscription Prediction (Bank Marketing)

| Section | Description |
| :--- | :--- |
| **Dataset** | Bank Marketing Dataset (UCI Machine Learning Repository) |
| **Skills Used** | Classification, Random Forest, SHAP (Explainable AI), Feature Engineering. |

### 🎯 Objective
To build a machine learning model that predicts whether a bank customer will subscribe to a term deposit. This helps financial institutions focus their marketing efforts on high-probability leads to reduce costs.

### 💡 Approach
1.  **Modeling:** Developed and compared **Logistic Regression** and **Random Forest** classifiers.
2.  **Efficiency:** Due to the large dataset size, a representative subset was utilized for training and evaluation.
3.  **Explainability:** Implemented **SHAP (SHapley Additive exPlanations)** to provide transparency by visualizing exactly which features drove the model's "Yes/No" predictions for individual customers.



### 📊 Results and Insights
* **Top Model:** **Random Forest** showed superior performance over Logistic Regression in handling the complex relationships in the dataset.
* **Key Influencers:** Analysis revealed that **call duration**, **campaign frequency**, and **previous campaign outcomes** were the most critical factors for success.
* **Impact:** The inclusion of SHAP values ensures the model is not a "black box," allowing bank managers to understand the reasoning behind every prediction.

***

## Task 2: Customer Segmentation Using Unsupervised Learning

| Section | Description |
| :--- | :--- |
| **Dataset** | Mall Customers Dataset |
| **Skills Used** | K-Means Clustering, PCA, t-SNE, Elbow Method, Silhouette Analysis. |

### 🎯 Objective
To segment a retail customer base into distinct groups based on annual income and spending behavior to enable data-driven, targeted marketing strategies.

### 💡 Approach
1.  **Clustering:** Applied the **K-Means algorithm** to group customers based on "Annual Income" and "Spending Score."
2.  **Optimization:** Used the **Elbow Method** and **Silhouette Analysis** to confirm that 5 clusters provided the most mathematically sound grouping.
3.  **Visualization:** Utilized **PCA** and **t-SNE** to reduce high-dimensional data, allowing for clear visual validation of the segments in 2D and 3D space.



### 📊 Results and Insights
* **Cluster Identification:**
    * **Target Group:** High Income, High Spenders (Focus for luxury products).
    * **Budget Group:** Low Income, Low Spenders (Focus for value bundles).
    * **Potential Group:** High Income, Low Spenders (Target for brand engagement).
* **Business Conclusion:** Identified 5 actionable customer personas, allowing for highly personalized marketing campaigns that maximize engagement and ROI.

***

## Task 3: Energy Consumption Time Series Forecasting

| Section | Description |
| :--- | :--- |
| **Dataset** | Household Power Consumption Dataset |
| **Skills Used** | Time Series Analysis, ARIMA, Facebook Prophet, XGBoost, Lag Engineering. |

### 🎯 Objective
To predict **Global Active Power** (total household electricity usage) by comparing traditional statistical methods, additive seasonal models, and machine learning regressors.

### 💡 Approach
1.  **Model Benchmarking:** Evaluated three distinct approaches: **ARIMA** (Statistical), **Facebook Prophet** (Seasonal Trend), and **XGBoost** (Feature-based ML).
2.  **Feature Engineering:** Created time-based features (hour, day of week) and lag variables to capture temporal dependencies.
3.  **Short-term Analysis:** Conducted a "Zoom-in" forecast comparison on a 168-hour window (1 week) to visualize how well each model tracked actual hourly usage.



### 📊 Results and Insights
* **Model Comparison:**
    * **Prophet:** Best at capturing the natural "rhythm" of daily household life (e.g., peak usage at 7 AM).
    * **XGBoost:** Most responsive to sudden, sharp spikes in energy consumption.
    * **ARIMA:** Provided a stable baseline but struggled with the high volatility of real-time usage.
* **Conclusion:** For energy providers, hybrid models combining seasonal trends (Prophet) with reactive lag features (XGBoost) offer the most robust forecasting for load management.

***
