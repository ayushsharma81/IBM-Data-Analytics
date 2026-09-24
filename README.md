# Customer Churn Prediction using AI-Driven Data Analytics

**IBM SkillsBuild Data Analytics with AI — Academic Internship 2026**
Conducted by **BharatCares** in association with **AICTE**

**Author:** YourName

---

## 📌 Project Description

Customer churn — when a customer stops using a company's service — directly impacts revenue and growth for subscription-based businesses such as telecom providers. This project uses **data analytics and machine learning (AI)** to:

- Explore and visualize the key factors that drive customer churn
- Build and compare predictive models (Logistic Regression and Random Forest) that flag customers likely to churn
- Surface explainable, actionable insights that a business can use to improve customer retention

The notebook covers the full analytics workflow: data generation/loading, cleaning, exploratory data analysis (EDA), preprocessing, model training, evaluation, and feature-importance analysis.

## 📊 Dataset

This project is modeled on the widely used **IBM Telco Customer Churn** dataset:

🔗 **Dataset link:** [Telco Customer Churn — IBM Dataset (Kaggle)](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

The notebook ships with a **synthetic 2,000-row dataset** (generated in Section 3 of the notebook) that mirrors the same columns and realistic churn-risk relationships as the original data (e.g., month-to-month contracts and low tenure increase churn risk). This makes the notebook runnable immediately, with no download or Kaggle account required.

To run the project on the **real dataset** instead:
1. Download `WA_Fn-UseC_-Telco-Customer-Churn.csv` from the Kaggle link above.
2. Place it in the same folder as the notebook.
3. Replace the dataset-generation cell with:
   ```python
   df = pd.read_csv("WA_Fn-UseC_-Telco-Customer-Churn.csv")
   ```
   All later sections use the same column names and will run unchanged.

## 🛠️ Technologies Used

| Category | Tools / Libraries |
|---|---|
| Language | Python 3.11 |
| Data handling | pandas, numpy |
| Visualization | matplotlib, seaborn |
| Machine Learning (AI) | scikit-learn (Logistic Regression, Random Forest) |
| Environment | Jupyter Notebook |

## 📁 Repository Contents

| File | Description |
|---|---|
| `YourName_CustomerChurnPrediction.ipynb` | Full project code — EDA, preprocessing, model training & evaluation |
| `requirements.txt` | Python dependencies required to run the notebook |
| `YourName_ProjectReport.docx` | Full project documentation/report |
| `README.md` | This file |

## ⚙️ Setup & Run Instructions

1. **Clone or download** this project folder.
2. **Create a virtual environment** (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate      # Windows: venv\Scripts\activate
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```
5. Open `YourName_CustomerChurnPrediction.ipynb` and run all cells (**Cell → Run All**).

Running the notebook will:
- Generate/save the dataset as `Telco-Customer-Churn.csv`
- Produce EDA charts (`eda_*.png`)
- Train and evaluate two models, saving `confusion_matrix.png`, `roc_curve.png`, and `feature_importance.png`
- Print accuracy, precision, recall, F1-score, and ROC-AUC for both models

## 🔑 Key Results

- **Best-performing model:** Random Forest (higher ROC-AUC than Logistic Regression)
- **Top churn drivers:** Contract type, total charges, monthly charges, and tenure
- **Business insight:** Customers on month-to-month contracts with short tenure and high monthly charges form the highest-risk segment for churn and should be prioritized for retention campaigns

## 📄 License / Academic Use

This project was created for academic submission under the AICTE | IBM SkillsBuild Data Analytics with AI Internship 2026 (BharatCares). Free to use for learning purposes.
