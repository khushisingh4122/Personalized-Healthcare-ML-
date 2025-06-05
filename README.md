# Personalized Healthcare Recommendations - ML Project 

This project builds a **Machine Learning-based system** that provides **personalized healthcare recommendations** based on patient health data. It uses blood donation history (like Recency, Frequency, etc.) to predict whether a patient needs medical attention or is likely healthy.

-----------

##  What This Project Does

- Loads and processes patient data from `blood.csv`
- Uses **feature scaling** to prepare numerical features
- Trains and compares multiple ML models:
  - Random Forest
  - Logistic Regression
  - Gradient Boosting
  - Support Vector Machine (SVM)
- Tunes the best model using **GridSearchCV**
- Visualizes class distribution using bar and pie charts
- Generates a personalized recommendation for a new patient
- Prints prediction confidence and model accuracy reports
- Times the full program execution ⏱

---

##  Example Data Fields

| Feature   | Description                                      |
|-----------|--------------------------------------------------|
| Recency   | Months since the last blood donation             |
| Frequency | Total number of donations                        |
| Monetary  | Blood volume donated                             |
| Time      | Months since the first donation                  |
| Class     | 0 = Healthy, 1 = Requires Attention (Label)      |

---

## ✅ Sample Output

Best Hyperparameters: {'classifier__max_depth': 5, 'classifier__min_samples_split': 5, 'classifier__n_estimators': 100}

Prediction Confidence (Probabilities): [[0.17 0.83]]
Personalized Recommendation: Requires attention

Total time taken to run the program: 2.35 seconds



## 📁 Files Included

- `blood.csv` – dataset file
- `personalized_healthcare.ipynb` – main notebook
- `health_model.pkl` – saved model for reuse

---

## 📌 Requirements

- Python 3.x
- Libraries:
  - `pandas`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`
  - `joblib`

You can install dependencies using: 
pip install pandas scikit-learn matplotlib seaborn joblib
 
 💡 How to Use
Clone the repo or upload the files to your own project

Run the notebook in Jupyter

Modify the example_patient_data to simulate other patients

View recommendation and model performance

########🧠 Future Ideas #######
Add login for doctors and patients

Use Streamlit to build a simple web app

Expand the dataset for deeper insights

✍️ Author
Khushi Singh
