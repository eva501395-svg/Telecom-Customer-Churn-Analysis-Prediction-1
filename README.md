# Telecom-Customer-Churn-Analysis-Prediction-1
Great question — your GitHub repo is what recruiters and the Codveda team will actually look at, so it needs a clear **README**, organized **folders per level** (the task list explicitly says "maintain a separate file for each level"), and visible results. Here's a complete blueprint based on your task list and the churn dataset you have.

## 1. First, pick tasks that fit your dataset

Your `churn-bigml-80/20.csv` files (telecom churn data, ~3,333 customers) are perfect for these:

| Level | Recommended Tasks | Why |
|---|---|---|
| **Level 1 (Basic)** | Task 2 (Data Cleaning) + Task 3 (EDA) | Churn data works directly |
| **Level 2 (Intermediate)** | Task 2 (Logistic Regression) + Task 3 (Clustering) | Churn prediction is the classic use case; clustering = customer segmentation |
| **Level 3 (Advanced)** | Task 3 (Neural Networks) | Feed-forward NN on the churn data; Tasks 1 & 2 need time-series/text data you don't have |

*(If you prefer Level 2 Task 1 (Regression), you could predict `Total day charge` from the other numeric features.)*

## 2. Repository structure

```
telecom-churn-analysis-codveda/
├── data/
│   ├── churn-bigml-80.csv
│   └── churn-bigml-20.csv
├── Level_1_Basic/
│   ├── Task2_Data_Cleaning_and_Preprocessing.ipynb
│   └── Task3_Exploratory_Data_Analysis.ipynb
├── Level_2_Intermediate/
│   ├── Task2_Classification_Logistic_Regression.ipynb
│   └── Task3_KMeans_Clustering.ipynb
├── Level_3_Advanced/
│   └── Task3_Neural_Network_TensorFlow_Keras.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## 3. README.md template (copy, then fill in your actual numbers)

````markdown
# 📞 Telecom Customer Churn — Analysis & Prediction
**Data Science Internship Projects | Codveda Technology**

End-to-end data science workflow on a real telecom churn dataset — from data
cleaning and exploratory analysis to classification, clustering, and deep
learning — completed as part of my 1-month Data Science internship at
Codveda Technology (2 tasks per level, Levels 1–3).

## 📊 Dataset
Two CSV files (`churn-bigml-80.csv` = 80% train, `churn-bigml-20.csv` = 20% test)
containing **3,333 customers × 20 features**:

- **Demographics:** State, Area code, Account length
- **Services:** International plan, Voice mail plan, Number vmail messages
- **Usage:** Total day / evening / night / international minutes, calls, charges
- **Support:** Customer service calls
- **Target:** `Churn` (True/False) — ~14.5% churn rate (imbalanced classes)

## 🛠️ Tech Stack
`Python` · `pandas` · `NumPy` · `scikit-learn` · `matplotlib` · `seaborn` · `TensorFlow/Keras` · `Jupyter`

## 🗂️ Repository Structure
| Folder | Contents |
|---|---|
| `Level_1_Basic/` | Data Cleaning & Preprocessing, EDA |
| `Level_2_Intermediate/` | Logistic Regression Classification, K-Means Clustering |
| `Level_3_Advanced/` | Neural Network with TensorFlow/Keras |

---

## Level 1 — Basic Tasks

### Task 2: Data Cleaning & Preprocessing
- Handled missing values and duplicates
- Outlier detection and treatment (IQR method)
- Encoded categorical features (`International plan`, `Voice mail plan` → binary;
  `State` → one-hot encoding)
- Scaled numerical features with `StandardScaler`
- Documented class imbalance (~85.5% loyal vs ~14.5% churned)

### Task 3: Exploratory Data Analysis (EDA)
- Summary statistics (mean, median, variance) per feature
- Histograms, box plots, and churn-rate comparisons
- Correlation matrix — minutes and charge columns are near-perfectly correlated
- **Key findings:**
  - Customers with an **International plan churn ~4× more often**
  - Churn rate rises sharply after **3–4 customer service calls**
  - High day-time usage correlates with churn

---

## Level 2 — Intermediate Tasks

### Task 2: Classification — Logistic Regression
- Natural train/test split using the 80/20 dataset files
- Baseline Logistic Regression vs Random Forest and SVM
- Evaluation: Accuracy, Precision, Recall, F1-score, ROC-AUC, confusion matrix

| Model | Accuracy | Precision | Recall | F1 | ROC-AUC |
|---|---|---|---|---|---|
| Logistic Regression | — | — | — | — | — |
| Random Forest | — | — | — | — | — |
| SVM | — | — | — | — | — |

### Task 3: Clustering — K-Means (Customer Segmentation)
- Optimal k selected via **elbow method + silhouette score**
- Clusters visualized in 2D using **PCA**
- Segment profiles interpreted (e.g., high-usage/international-plan cluster
  aligned with high churn)

---

## Level 3 — Advanced Task

### Task 3: Neural Network with TensorFlow/Keras
- Feed-forward architecture: input → Dense(64) → Dense(32) → Dense(1, sigmoid)
- Dropout + early stopping to prevent overfitting
- Handled class imbalance with class weights
- Trained with backpropagation; plotted accuracy/loss curves
- Tuned learning rate and batch size

| Metric | Value |
|---|---|
| Test Accuracy | — |
| ROC-AUC | — |
| Recall (churn class) | — |

---

## 🚀 How to Run
```bash
git clone https://github.com/<your-username>/telecom-churn-analysis-codveda.git
cd telecom-churn-analysis-codveda
pip install -r requirements.txt
# open notebooks in Jupyter and run top to bottom
```

## 🙏 Acknowledgments
Thank you to **Codveda Technology** for the internship opportunity and guidance.

#CodvedaJourney #CodvedaExperience #FutureWithCodveda #CodvedaProjects
````

## 4. Supporting files

**`requirements.txt`** (example):
```
pandas
numpy
scikit-learn
matplotlib
seaborn
tensorflow
jupyter
```

**`.gitignore`**: include `.ipynb_checkpoints/`, `venv/`, `__pycache__/`

## 5. Pro tips

- **Save notebooks with outputs visible** — recruiters want to see your plots, confusion matrices, and metrics without running anything.
- **Write real conclusions** in each notebook (2–3 sentences of "what did we learn") — this is what separates you from copy-paste repos.
- **Use meaningful commit messages** (`Add EDA on churn drivers`, not `update`) — it shows your process.
- **Pin the repository** on your GitHub profile, then link it in your LinkedIn video post as the internship instructions require.
- Fill in the `—` placeholders in the tables with your **actual results** after running your models — never leave fake numbers.

Want me to help you next with the actual notebook code for any specific task (e.g., the Logistic Regression churn classifier or the EDA)?
