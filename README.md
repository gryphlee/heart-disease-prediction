# heart-disease-prediction

# Heart Disease Prediction using Machine Learning

This project is an end-to-end binary classification model built to predict the presence of heart disease in patients based on a set of medical attributes. An XGBoost Classifier is trained on the well-known UCI Heart Disease dataset to provide an accurate diagnostic prediction.

![Project Banner](https://i.imgur.com/gA32GvT.png)

## 1. Business Problem

Cardiovascular diseases are a leading cause of death globally. Early detection is critical for effective treatment and management. This project leverages machine learning to create a tool that can assist medical professionals by predicting the likelihood of heart disease based on patient data, enabling earlier intervention and potentially improving patient outcomes.

---

## 2. Dataset

The analysis uses the **Heart Disease UCI** dataset, a well-known benchmark in the machine learning community for this classification task.

* **Source:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data)
* **Content:** The dataset contains 14 medical attributes collected from patients, including `age`, `sex`, `cholesterol` (chol), `resting blood pressure` (trestbps), and the target variable.

---

## 3. Methodology

The project follows a standard data science workflow from data cleaning to model evaluation.

1.  **Data Cleaning & Preprocessing:** Handled missing values (represented by `?`) and converted the multi-level target variable (`num`) into a binary target (`0` for no disease, `1` for disease). All text-based columns were converted to a numeric format using one-hot encoding.
2.  **Exploratory Data Analysis (EDA):** Visualized the data to understand feature distributions and their relationships with the target variable using tools like `pairplot` and `countplot`.
3.  **Feature Scaling:** Applied `StandardScaler` from Scikit-learn to normalize the feature set, ensuring that all features contribute equally to the model's performance.
4.  **Model Training & Evaluation:** An **XGBoost Classifier** was trained on the preprocessed data. Its performance was then evaluated on an unseen test set using a classification report and a confusion matrix.

---

## 4. Model Performance

The final **XGBoost Classifier** achieved a strong performance, demonstrating its effectiveness in this diagnostic task.

* **Accuracy:** The model achieved an accuracy of **83%** on the unseen test data.
* **Key Insight:** The confusion matrix below shows the model's predictions. It correctly identified 29 healthy patients and 21 patients with heart disease, showing a balanced ability to detect both classes.

![XGBoost Confusion Matrix for Heart Disease Prediction](https://i.imgur.com/rLdK1rF.png)

---

## 5. Technologies Used

* **Python 3**
* **Pandas & NumPy:** For data manipulation and cleaning.
* **Scikit-learn:** For data preprocessing (`StandardScaler`), splitting, and evaluation.
* **XGBoost:** For training the high-performance classification model.
* **Matplotlib & Seaborn:** For data visualization.
* **Jupyter Notebook / VS Code:** For the development environment.
