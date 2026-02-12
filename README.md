# 📡 Sonar Mine vs Rock Classification

This project builds and compares multiple machine learning classification models to predict whether a sonar signal corresponds to a **mine** or a **rock**.

The dataset contains 60 numerical features representing sonar energy measurements at different frequencies. The task is a **binary classification problem**:

- `M` → Mine
- `R` → Rock

The goal of this project is to evaluate and compare different classification algorithms on this dataset.

---

## 📁 Dataset

- **Source:** [Kaggle – Connectionist Bench Sonar Mines vs Rocks](https://www.kaggle.com/datasets/armanakbari/connectionist-bench-sonar-mines-vs-rocks)
- **Total Samples:** 208
- **Number of Features:** 60 (continuous numerical values)
- **Target Variable:** `M` (Mine) or `R` (Rock)

The dataset represents sonar returns bouncing off metal cylinders (mines) or rocks at various frequencies.

> Note: The dataset is not included in this repository. Please download it from Kaggle and place it in the project directory as `sonar.csv`.

---

## 🧠 Models Implemented

The following classification models were trained and evaluated:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest Classifier
- Support Vector Classifier (SVC)

An 80/20 train-test split was used for evaluation.

Feature scaling was applied using **StandardScaler**, which is important for distance-based models like KNN and SVC.

---

## 📊 Results

Below are the model accuracies on the test set:

Logistic Regression Accuracy: 80.95%
KNN Accuracy: 90.48%
Random Forest Accuracy: 85.71%
SVC Accuracy: 88.10%

**Best Performing Model:** [KNeighborsClassifier]

---

## ⚙️ How to Run

### 1️⃣ Clone the Repository

bash
git clone https://github.com/uraza116/SONAR-Rock-vs-Mine-Prediction-
cd your-repo-name

### 2️⃣ Create a Virtual Environment

python -m venv .venv
source .venv/bin/activate # Mac/Linux
.venv\Scripts\activate # Windows

### 3️⃣ Install Dependencies

pip install -r requirements.txt

### 4️⃣ Run the Notebook

### Open the notebook file:

sonar_mine_vs_rock.ipynb

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

## Key Takeaways

- Comparison of multiple classification algorithms on the same dataset
- Understanding model performance evaluation using accuracy
- Practical implementation of binary classification
