# ShinyApp_python_ML_prediction

---

```markdown
# 📊 Loan Default Risk Prediction Dashboard

This project is a web-based dashboard built with **Python Shiny** to predict the probability of loan default using trained machine learning models: **AdaBoost, CatBoost, and Random Forest**.

## 🚀 Features

- ✅ Predict loan default risk with a few user inputs.
- 📊 Visualize model-specific feature importance.
- 📈 Display loan statistics & dataset insights.
- 🔄 Interactive UI with model switching.
- 📥 Download the full dataset in **CSV/XLSX** format.

---

## 🛠️ Setup Instructions

### 1️⃣ Create a Virtual Environment (Recommended)

```bash
python -m venv venv
```

### 2️⃣ Activate the Environment

- **Windows**
  ```bash
  venv\Scripts\activate
  ```

- **macOS/Linux**
  ```bash
  source venv/bin/activate
  ```

### 3️⃣ Install Required Libraries

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the App

Once your environment is ready, **run the following command**:

```bash
shiny run --reload app.py
```

Then, **open your browser** and visit:

```
http://127.0.0.1:8000
```

---

## 📁 Project Structure

```
LOAN_DEFAULT_PROJECT/
│
├── __pycache__/            # Compiled Python files
├── .venv/                  # Virtual environment (hidden)
├── data/                   # Processed dataset storage
│   ├── processed_loan_data.csv
│
├── models/                 # Trained models (saved as .pkl files)
│
├── notebook/               # Jupyter notebooks for analysis
│
├── static/                 # Static plots & images
│   ├── default_rate_by_dti.png
│   ├── static_line_dti_default.png
│   ├── catboost.png
│   ├── adaboost.png
│   ├── randomforest.png
│
├── venv/                   # Python virtual environment
│
├── app.py                  # Main Shiny dashboard script
├── README.md               # Project documentation
├── requirements.txt        # Dependencies list
```

---

## 📌 Notes

- 🔹 The dashboard **only takes 4 primary inputs** from the user; other features are **filled with realistic median values**.
- 🔹 **Trained models** must be stored in the `models/` directory.
- 🔹 **Static plots** must be pre-generated and saved in the `static/` directory.

---

## ✅ Machine Learning Models Used

- **AdaBoost Classifier**
- **CatBoost Classifier**
- **Random Forest Classifier**

📌 **All models are trained on engineered features (`f_` columns), with `Default` as the target variable.**

---

## 💡 Future Improvements

- 🔄 Add real-time feature engineering before prediction.
- 📊 Improve UI with better visualizations.
- ⚡ Optimize model inference speed.

---
