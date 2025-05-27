# 🛡️ Phishing Detection Model Performance Tracking with MLflow

This project implements a **phishing website detection system** using supervised machine learning algorithms and **MLflow** to track experiments, metrics, and artifacts. It applies effective **feature selection**, evaluates multiple models, and logs everything for **performance comparison and reproducibility**.

---

## 📌 Project Overview

- Built a phishing detection system using a dataset with ~11,000 samples.
- Evaluated **Random Forest**, **Decision Tree**, and **Logistic Regression** classifiers.
- Applied feature selection and standard preprocessing steps.
- Achieved **95% accuracy** on the best-performing model.
- Used **MLflow** to log:
  - Model hyperparameters
  - Accuracy, precision, and recall
  - Trained models and other artifacts for reproducibility

---

## 🔍 Dataset

The dataset consists of ~11,000 samples, each containing features indicative of phishing attempts, such as:

- Presence of IP Address in URL
- Length of URL
- Use of HTTPS
- Domain registration length
- Number of redirects
- Mouseover behavior, etc.

---

## ⚙️ Tools & Technologies

- **Python 3**
- **Jupyter Notebook**
- **Pandas, NumPy, Scikit-learn**
- **Matplotlib, Seaborn**
- **MLflow** for experiment tracking

---

## 📈 Models Evaluated

| Model               | Accuracy |
|--------------------|----------|
| Random Forest       | 95%      | 
| Decision Tree       | ~91%     | 
| Logistic Regression | ~89%     | 

Each model was trained with hyperparameter tuning, and all evaluation metrics and artifacts were logged to MLflow for comparison.

---

## 🧪 MLflow Integration

- Set up a local MLflow tracking server.
- Logged parameters (`max_depth`, `n_estimators`, etc.)
- Logged evaluation metrics (`accuracy`, `precision`, `recall`)
- Logged model artifacts (pickle/MLlib files)

📸 **Example MLflow UI Output:**

![MLflow UI Screenshot](https://github.com/user-attachments/assets/79e4dc2b-cd0e-41d9-8f56-24cbc7e18e42)

![Experiment Result Screenshot](https://github.com/user-attachments/assets/9c64c059-0f58-4f83-86f9-264633b2508d)

![Confusion Matrix Output](https://github.com/user-attachments/assets/bd92b0eb-e90b-4d8b-bd2b-8ec873c95aac)


> You can launch MLflow using:
> ```bash
> mlflow ui
> ```
> and access it at `http://localhost:5000`.


