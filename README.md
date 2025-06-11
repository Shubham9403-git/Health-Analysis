# 🫀 Heart Disease Prediction using Logistic Regression

This project is a machine learning-based approach to predict the presence of heart disease using a dataset of clinical attributes. The goal is to explore, visualize, and train a model that can help identify high-risk patients using key health indicators.

---

## 📁 Dataset

The dataset used is the **Heart Disease UCI dataset** commonly used in ML classification tasks. It contains 14 features such as age, sex, chest pain type, resting blood pressure, cholesterol, etc.

- 📌 **Target Variable:** `target` (1 = presence of heart disease, 0 = absence)

### Sample Features:
| Feature | Description |
|---------|-------------|
| age     | Age in years |
| cp      | Chest pain type (0–3) |
| trestbps| Resting blood pressure |
| chol    | Serum cholesterol in mg/dl |
| thal    | Thalassemia (0–2) |
| target  | Target (0 or 1) |

---

## ⚙️ Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn (for EDA and visualization)
- Scikit-learn (for model building)

---

## 🔍 Steps Performed

1. **Data Loading & Inspection**
   - Loaded the CSV using Pandas.
   - Checked for missing values, data types, and statistical summary.

2. **Exploratory Data Analysis (EDA)**
   - Correlation heatmap of all features.
   - Count plots for target distribution and chest pain types.

3. **Data Preprocessing**
   - Feature scaling using `StandardScaler`.
   - Train-test split (80/20).

4. **Model Training**
   - Trained a Logistic Regression model using `sklearn.linear_model`.

5. **Evaluation Metrics**
   - Confusion matrix
   - Classification report
   - Accuracy score

---

## 📊 Output Visualizations

- 🔥 Correlation Heatmap
- 📉 Star rating distribution (countplot)
- 💔 Chest pain type vs Heart Disease (grouped countplot)
- ✅ Confusion Matrix, Accuracy Score, and Classification Report

---

## 🧪 How to Run

// bash
# Step 1: Clone the repository
git clone https://github.com/Shubham9403-git/Health-Analysis.git
cd heart-disease-prediction

# Step 2: Install required packages
pip install -r requirements.txt

# Step 3: Run the main Python script
python heart_disease_predict.py

// Confusion Matrix:
[[23  4]
 [ 3 31]]

Classification Report:
              precision    recall  f1-score   support
           0       0.88      0.85      0.86        27
           1       0.89      0.91      0.90        34

Accuracy Score: 0.88


# 📌 Future Work
  * Add support for other models (Random Forest, SVM, etc.)

  * Hyperparameter tuning and cross-validation

  * Web deployment using Streamlit or Flask

  * Model interpretation (SHAP values or feature importance)
