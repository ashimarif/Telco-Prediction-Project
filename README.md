# Analyzing Telco Usage Patterns to Predict Subscription Type with Machine Learning


## 📌 Project Overview
This project aims to develop a machine learning model to automatically categorize mobile plans as either **Prepaid** or **Postpaid** based on key user attributes such as pricing, data limits, and digital behavior. 

In Malaysia's competitive telecommunications industry, understanding customer preferences is critical. This project utilizes the **K-Nearest Neighbors (KNN)** algorithm and **K-Fold Cross Validation** to predict subscription types, helping telcos align their product offerings with actual user behavior.

## 🎯 Objectives
1. **Analyze** Malaysian telco user data to extract meaningful features indicating subscription behavior.
2. **Develop** a predictive classification model using K-Nearest Neighbors (KNN) to differentiate between prepaid and postpaid users.
3. **Evaluate** classification accuracy and consistency using K-Fold Cross Validation.

## 📂 Repository Structure
Based on the project files, the repository is organized as follows:
- **`DATASETS/`**: Contains the raw survey data collected via Google Forms.
- **`JUPYTER-PYTHON CODE/`**: The main `.ipynb` notebooks containing data cleaning, EDA, and model training.
- **`REPORT/`**: The full project documentation (PDF).
- **`SPLIT DATASET/`**: Training and testing splits used for the model.
- **`K-FOLD DATASETS/`**: Datasets divided for the 4-fold cross-validation process.

## ⚙️ Methodology & Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Scikit-Learn, Matplotlib, Seaborn.
* **Algorithm:** K-Nearest Neighbors (KNN).
* **Validation:** K-Fold Cross Validation ($K=4$).

### Data Pipeline:
1.  **Data Collection:** Survey of 681 participants with 23 features (e.g., Age, Income, Monthly Data Usage, Gaming/Streaming habits).
2.  **Preprocessing:** Data cleaning, label encoding for categorical variables, and Z-score normalization.
3.  **Modeling:** * Initial KNN model ($k=9$, distance weights).
    * Optimization using K-Fold Cross Validation.
    * Final Model parameters: $k=7$, Metric=`distance`.

## 📊 Key Results & Insights
* **Model Accuracy:** The final remodeled classifier achieved **100% accuracy** on both training and testing sets after hyperparameter tuning.
* **Behavioral Insights:**
    * **Marital Status:** Married individuals predominantly prefer **Postpaid** plans, while Single users lean towards **Prepaid**.
    * **Location:** Urban areas have the highest Wi-Fi availability (56.5%), correlating with different data consumption patterns compared to rural areas.
    * **Spending:** Postpaid users exhibit a wider spread and higher median monthly expenses compared to prepaid users.

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/ashimarif/Telco-Prediction-Project.git](https://github.com/ashimarif/Telco-Prediction-Project.git)
