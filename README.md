# heart-disease--prediction-machine-learning
Here’s a complete **README.md** file tailored for your GitHub repository based on the provided project details:

---

# Heart Disease Prediction Using Machine Learning Classification Models

## Project Overview
Heart disease is one of the leading causes of death, requiring early detection to mitigate its impact. This project explores the use of **machine learning classification models** to predict heart disease. The dataset is sourced from the **Behavioural Risk Factor Surveillance System (BRFSS)** and includes lifestyle and health-related factors. Seven machine learning models are implemented, compared, and evaluated based on performance metrics such as **Accuracy, Precision, Recall, F1-score, ROC-AUC**, and **Specificity**.

---

## Dataset
- **Source**: Behavioural Risk Factor Surveillance System (BRFSS)
- **Records**: 319,795 entries
- **Columns**: 18 features, including:
    - `HeartDisease` (Target)
    - `BMI` - Body Mass Index
    - `Smoking` - Smoking status
    - `AlcoholDrinking` - Alcohol consumption
    - `PhysicalActivity` - Exercise habits
    - `GenHealth` - General health rating
    - `AgeCategory`, `Sex`, `Race`, etc.

---

## Project Objectives
- Analyze and visualize key factors affecting heart disease:
   - Impact of **age**, **gender**, **smoking**, **alcohol consumption**, and **physical activity**.
- Handle class imbalance using techniques like **under-sampling** and **SMOTE**.
- Train and evaluate seven machine learning models:
   1. Logistic Regression
   2. Decision Tree
   3. Random Forest
   4. K-Nearest Neighbors
   5. Gradient Boosting
   6. XGBoost
   7. AdaBoost
- Identify the best-performing model for **heart disease prediction**.

---

## Tools and Libraries
- **Python**: pandas, numpy, matplotlib, seaborn, scikit-learn
- **Visualization**: Tableau (for dashboards)
- **Model Evaluation**: ROC-AUC, F1-score, Precision, Recall, Accuracy

---

## Methodology

### 1. **Data Preprocessing**
   - Duplicate removal (18,078 records)
   - Outlier handling (SleepTime outliers removed)
   - Encoding:
     - Binary features → Label Encoding
     - Ordinal features → Ordinal Encoding
     - Nominal features → One-Hot Encoding
   - Scaling: `StandardScaler`

### 2. **Exploratory Data Analysis (EDA)**
- Insights from visualizations:
   - Heart disease rates based on **age**, **gender**, **physical activity**, etc.
   - Correlation analysis to identify relationships between features.

### 3. **Modeling**
- Resampling to handle class imbalance.
- Seven classification models trained and evaluated:
   - Gradient Boosting outperformed others with **80% Recall** and **0.84 ROC-AUC**.

### 4. **Model Evaluation**
- Key metrics:
   - Accuracy
   - Precision
   - Recall
   - Specificity
   - F1-score
   - ROC-AUC

---

## Results
| **Model**              | **Accuracy** | **Precision** | **Recall** | **F1-Score** | **ROC-AUC** |
|------------------------|--------------|---------------|------------|--------------|-------------|
| Logistic Regression    | 0.74         | 0.22          | 0.77       | 0.35         | 0.84        |
| Decision Tree          | 0.67         | 0.17          | 0.65       | 0.26         | 0.67        |
| Random Forest          | 0.71         | 0.20          | 0.76       | 0.32         | 0.81        |
| K-Nearest Neighbors    | 0.71         | 0.20          | 0.74       | 0.31         | 0.78        |
| **Gradient Boosting**  | **0.73**     | **0.22**      | **0.80**   | **0.34**     | **0.84**    |
| XGBoost                | 0.73         | 0.22          | 0.78       | 0.34         | 0.83        |
| AdaBoost               | 0.74         | 0.22          | 0.77       | 0.35         | 0.83        |

**Best Performing Model**: Gradient Boosting  
- **Recall**: 80% (minimizes false negatives, critical for healthcare)
- **ROC-AUC**: 0.84

---

## Conclusion
Gradient Boosting achieved the highest **recall** (80%) and **ROC-AUC** (0.84), making it the most suitable model for heart disease prediction. While false positives remain an issue, minimizing false negatives is prioritized in healthcare applications. Further improvements can be explored using additional features and advanced machine learning techniques.

---

## Future Work
- Incorporate additional features (e.g., lab results, ECG data).
- Explore hybrid and deep learning models.
- Optimize thresholds to balance recall and precision.

---


---

This README provides a comprehensive guide for collaborators, users, and stakeholders. Let me know if you'd like further refinements!
