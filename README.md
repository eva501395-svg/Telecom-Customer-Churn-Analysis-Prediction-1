
````markdown
# Telecom Customer Churn — Analysis & Prediction

**Data Science Internship | Codveda Technology**

End-to-end data science workflow on telecom customer data: cleaning, EDA, machine learning, and deep learning — 2 tasks per level, Levels 1–3.

---

## 📁 Repository Structure

```
├── data/                        # churn-bigml-80.csv, churn-bigml-20.csv
├── Level_1_Basic/               # Data Cleaning, EDA
├── Level_2_Intermediate/        # Logistic Regression, K-Means
├── Level_3_Advanced/            # Neural Network (Keras)
└── README.md
```

## 📊 Dataset

3,333 telecom customers × 20 features (call usage, plans, service calls). Target: `Churn` (~14.5% positive — imbalanced classes). The 80/20 train-test split is provided as two CSV files in `data/`.

## ✅ Tasks Completed

| Level | Task | Notebook | What Was Done |
|---|---|---|---|
| 1 | Data Cleaning & Preprocessing | `Level_1_Basic/Task2_...ipynb` | Missing values, outlier removal (IQR), one-hot encoding, scaling |
| 1 | Exploratory Data Analysis | `Level_1_Basic/Task3_...ipynb` | Summary stats, distributions, correlation matrix, churn drivers |
| 2 | Classification | `Level_2_Intermediate/Task2_...ipynb` | Logistic Regression vs Random Forest & SVM; accuracy, precision, recall, ROC |
| 2 | Clustering | `Level_2_Intermediate/Task3_...ipynb` | K-Means, elbow + silhouette, PCA visualization, segment interpretation |
| 3 | Neural Network | `Level_3_Advanced/Task3_...ipynb` | Feed-forward net (Keras), dropout, class weights, hyperparameter tuning |

## 🏆 Results

| Model | Accuracy | F1 (churn) | ROC-AUC |
|---|---|---|---|
| Logistic Regression | — | — | — |
| Random Forest | — | — | — |
| Neural Network | — | — | — |

## 💡 Key Insights

- Customers with an **International plan churn ~4× more** than those without
- Churn rate jumps sharply after **3+ customer service calls**
- Minutes and charge columns are almost perfectly correlated (redundant features)

## 🛠️ Tech Stack

`Python` `pandas` `scikit-learn` `matplotlib` `seaborn` `TensorFlow/Keras`

## 🚀 How to Run

```bash
git clone https://github.com/<your-username>/telecom-churn-analysis-codveda.git
cd telecom-churn-analysis-codveda
pip install -r requirements.txt
```
Then open the notebooks in Jupyter and run top to bottom.

---

Made during my Data Science internship at **Codveda Technology**.

#CodvedaJourney #CodvedaExperience #FutureWithCodveda
````

