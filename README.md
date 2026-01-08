# Analyzing Telco Usage Patterns to Predict Subscription Type with Machine Learning

**Course:** Special Topic in Computer Science (CSC649)  
**Institution:** Universiti Teknologi MARA (UiTM)  
**Status:** Completed (July 2025)

## 📌 Project Overview
[cite_start]This project aims to develop a machine learning model to automatically categorize mobile plans as either **Prepaid** or **Postpaid** based on key user attributes such as pricing, data limits, and digital behavior[cite: 16]. 

In Malaysia's competitive telecommunications industry, understanding customer preferences is critical. [cite_start]This project utilizes the **K-Nearest Neighbors (KNN)** algorithm and **K-Fold Cross Validation** to predict subscription types, helping telcos align their product offerings with actual user behavior[cite: 17, 70, 81].

## 👥 Team Members
| Name | Student ID |
| :--- | :--- |
| Aisya Hanim Binti Basri | 2023126685 |
| Nurin Qurratu' Aini Binti Razali | 2023103525 |
| Muhammad Ashim Bin Mohd Arif | 2023119039 |
| Ahmad Luthfi Bin Hassan | 2023115999 |
[cite_start][cite: 12]

## 🎯 Objectives
1. [cite_start]**Analyze** Malaysian telco user data to extract meaningful features indicating subscription behavior[cite: 80].
2. [cite_start]**Develop** a predictive classification model using K-Nearest Neighbors (KNN) to differentiate between prepaid and postpaid users[cite: 81].
3. [cite_start]**Evaluate** classification accuracy and consistency using K-Fold Cross Validation[cite: 85].

## 📂 Repository Structure
Based on the project files, the repository is organized as follows:
- **`DATASETS/`**: Contains the raw survey data collected via Google Forms.
- **`JUPYTER-PYTHON CODE/`**: The main `.ipynb` notebooks containing data cleaning, EDA, and model training.
- **`REPORT/`**: The full project documentation (PDF).
- **`SPLIT DATASET/`**: Training and testing splits used for the model.
- **`K-FOLD DATASETS/`**: Datasets divided for the 4-fold cross-validation process.

## ⚙️ Methodology & Tech Stack
* **Language:** Python
* [cite_start]**Libraries:** Pandas, Scikit-Learn, Matplotlib, Seaborn[cite: 285].
* **Algorithm:** K-Nearest Neighbors (KNN).
* [cite_start]**Validation:** K-Fold Cross Validation ($K=4$)[cite: 936].

### Data Pipeline:
1.  [cite_start]**Data Collection:** Survey of 681 participants with 23 features (e.g., Age, Income, Monthly Data Usage, Gaming/Streaming habits)[cite: 109, 263].
2.  [cite_start]**Preprocessing:** Data cleaning, label encoding for categorical variables, and Z-score normalization[cite: 374, 497].
3.  **Modeling:** * Initial KNN model ($k=9$, distance weights).
    * Optimization using K-Fold Cross Validation.
    * [cite_start]Final Model parameters: $k=7$, Metric=`distance`[cite: 976, 1765].

## 📊 Key Results & Insights
* [cite_start]**Model Accuracy:** The final remodeled classifier achieved **100% accuracy** on both training and testing sets after hyperparameter tuning[cite: 1765].
* **Behavioral Insights:**
    * [cite_start]**Marital Status:** Married individuals predominantly prefer **Postpaid** plans, while Single users lean towards **Prepaid**[cite: 1202].
    * [cite_start]**Location:** Urban areas have the highest Wi-Fi availability (56.5%), correlating with different data consumption patterns compared to rural areas[cite: 1230].
    * [cite_start]**Spending:** Postpaid users exhibit a wider spread and higher median monthly expenses compared to prepaid users[cite: 1563].

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone [https://github.com/ashimarif/Telco-Prediction-Project.git](https://github.com/ashimarif/Telco-Prediction-Project.git)
