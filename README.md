# ❤️ Heart Disease Prediction (Machine Learning Project)

This project builds a **machine learning model** to predict the presence of heart disease using the Heart Disease UCI dataset.

It covers the full pipeline:

> Data Cleaning → Feature Engineering → Visualization → Model Training → Evaluation → Interpretation

---

## 🚀 Features

* 🧹 Data cleaning (handling missing values and invalid entries)
* 🔄 Feature engineering (binary target creation)
* 📊 Exploratory Data Analysis (EDA)
* 🔥 Correlation heatmap
* 📈 Data visualization with Seaborn & Matplotlib
* 🤖 Logistic Regression model
* 📉 Model evaluation:

  * Accuracy
  * Confusion Matrix
  * ROC Curve & AUC
* 📊 Feature importance visualization

---

## 🛠️ Tech Stack

* Python 🐍
* pandas → Data preprocessing
* numpy → Numerical operations
* matplotlib → Visualization
* seaborn → Statistical plots
* scikit-learn → Machine learning

---

## 📂 Dataset

The dataset includes patient health information such as:

* Age
* Sex
* Chest pain type (`cp`)
* Cholesterol
* Blood pressure
* Other medical attributes

### 🎯 Target Variable

The original dataset contains a column `num`:

* `0` → No disease
* `>0` → Disease present

This project converts it into a binary target:

```python
target = 1 if num > 0 else 0
```

---

## 🧹 Data Preprocessing Steps

* Removed missing values (`dropna`)
* Replaced invalid values (`"?" → NaN`)
* Dropped unnecessary column (`id`)
* Converted categorical data into numeric
* Encoded categorical variables using one-hot encoding

---

## 📊 Exploratory Data Analysis

### ✔ Correlation Heatmap

* Shows relationships between features

### ✔ Count Plot

* Visualizes chest pain (`cp`) vs target

---

## 🤖 Model Building

### Algorithm Used:

* Logistic Regression

### Steps:

1. Split dataset (80% training, 20% testing)
2. Train model using training data
3. Predict on test data

---

## 📈 Model Evaluation

### ✔ Accuracy

```text
Accuracy: (printed in output)
```

---

### ✔ Confusion Matrix

* Shows:

  * True Positives
  * True Negatives
  * False Positives
  * False Negatives

---

### ✔ ROC Curve & AUC

* Measures model performance across thresholds
* AUC score indicates model quality

---

## 📊 Feature Importance

* Extracted using model coefficients
* Visualized using bar chart

👉 Helps identify which features most influence predictions

---

## ▶️ How to Run

### 1. Clone repository

```bash
https://github.com/codeTechs965/Heart-Disease-Prediction
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Run the script

```bash
Heart_Disease_Prediction.ipynb
```

---

## ⚠️ Notes

* Dataset file must be named:

```text
heart_disease_uci.csv
```


---

## 🔮 Future Improvements

* Add feature scaling (StandardScaler)
* Try advanced models:

  * Random Forest
  * XGBoost
* Hyperparameter tuning
* Build web app (Streamlit)
* Deploy model

---

## 🎯 Learning Outcomes

* Data cleaning and preprocessing
* Handling categorical variables
* Model training and evaluation
* Visualization techniques
* Interpreting model results

---

## ⚠️ Disclaimer

This project is for **educational purposes only**.
It does NOT provide medical diagnosis. Always consult a healthcare professional.

---

## 🤝 Contributing

Contributions are welcome!
Feel free to fork and submit a pull request.

---

## ⭐ Support

If you found this helpful, give it a ⭐ on GitHub!

---

## 👤 Author

TalhaAmmar

---
