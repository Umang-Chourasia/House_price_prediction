# 🏠 California Housing Price Prediction

A Machine Learning project that predicts California housing prices using the California Housing dataset.  
This project demonstrates an end-to-end ML workflow including data preprocessing, feature engineering, model training, serialization, and prediction generation using Scikit-learn pipelines.

---

## 🚀 Project Overview

The goal of this project is to build a regression model capable of predicting median house values based on various housing-related features such as:

- Median income
- Housing age
- Total rooms
- Population
- Geographic location
- Ocean proximity

The project follows a production-style workflow with reusable preprocessing pipelines and saved trained models.

---

## ✨ Key Features

- End-to-end Machine Learning pipeline
- Data preprocessing using Scikit-learn pipelines
- Missing value handling
- Feature scaling and categorical encoding
- Stratified train-test splitting
- Random Forest Regression model
- Model persistence using Joblib
- Batch prediction support using CSV input
- Clean and modular workflow

---

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- Joblib

---

## 📂 Project Structure

```bash
California-House-Price-Prediction/
│
├── main.py              # Main training & prediction script
├── housing.csv          # California housing dataset
├── input_data.csv       # Input file for predictions
├── output_data.csv      # Generated predictions
├── model.pkl            # Saved trained model
├── pipeline.pkl         # Saved preprocessing pipeline
└── README.md
```

---

## ⚙️ Machine Learning Workflow

### 1. Data Loading
The dataset is loaded using Pandas for preprocessing and analysis.

### 2. Data Preprocessing
The preprocessing pipeline includes:
- Median imputation for missing values
- Feature scaling using StandardScaler
- One-hot encoding for categorical features

### 3. Stratified Sampling
Income categories are used to perform stratified sampling for better train-test distribution.

### 4. Model Training
A `RandomForestRegressor` is trained on the processed dataset.

### 5. Model Serialization
The trained model and preprocessing pipeline are saved using Joblib for future inference.

### 6. Prediction Pipeline
New housing data can be passed through `input_data.csv` to generate predictions automatically.

---

## ▶️ How to Run the Project

### Clone the Repository

```bash
git clone https://github.com/yourusername/California-House-Price-Prediction.git
cd California-House-Price-Prediction
```

---

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

### Run the Project

```bash
python main.py
```

---

## 🔁 Training Mode

If saved model files are not available:
- The model will train automatically
- `model.pkl` and `pipeline.pkl` will be generated

---

## 🔮 Prediction Mode

If model files already exist:
- Existing model and pipeline are loaded
- Input data is read from `input_data.csv`
- Predictions are generated
- Results are saved to `output_data.csv`

---

## 📊 Output

Predictions are stored in:

```text
output_data.csv
```

Predicted values are generated under the column:

```text
median_house_value
```

---

## 📈 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Model evaluation metrics dashboard
- XGBoost/LightGBM integration
- Streamlit or Flask deployment
- Interactive data visualization
- Docker containerization

---

## 🎯 Learning Outcomes

This project helped in understanding:
- Machine Learning pipelines
- Data preprocessing workflows
- Regression modeling
- Model persistence
- Production-style ML structure

---

## 👨‍💻 Author

Umang Chourasia

---

## ⭐ Acknowledgment

This project uses the California Housing dataset available through Scikit-learn.
