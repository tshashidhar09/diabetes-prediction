# Diabetes Risk Prediction — BRFSS 2015

## Predictive Analytics Coursework (MSIN0097)

### Overview
End-to-end machine learning pipeline predicting diabetes risk from 21 health indicators using the CDC's Behavioral Risk Factor Surveillance System (BRFSS) 2015 dataset.

### Repository Structure
```
├── diabetes_prediction.ipynb   # Main analysis notebook (run this)
├── requirements.txt            # Python dependencies
├── README.md                   # This file
└── data/
    └── diabetes_binary_health_indicators_BRFSS2015.csv
```

### Quick Start

**1. Clone the repository:**
```bash
git clone <your-repo-url>
cd diabetes-prediction
```

**2. Create a virtual environment (recommended):**
```bash
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows
```

**3. Install dependencies:**
```bash
pip install -r requirements.txt
```

**4. Place the dataset:**
Download the dataset from [Kaggle](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset) and place the CSV file in a `data/` folder, or in the same directory as the notebook.

**5. Run the notebook:**
```bash
jupyter notebook diabetes_prediction.ipynb
```
Run all cells from top to bottom (Cell → Run All).

### Dataset
- **Source:** CDC BRFSS 2015 via Kaggle
- **Size:** 253,680 rows × 22 columns
- **Target:** `Diabetes_binary` (0 = No diabetes, 1 = Diabetes/Prediabetes)
- **License:** Public domain (CDC survey data)

### Methods Used
- Logistic Regression (baseline)
- Random Forest
- XGBoost
- LightGBM
- Neural Network (Keras/TensorFlow)
- SMOTE for class imbalance
- SHAP for model interpretability

### Environment
- Python 3.10+
- See `requirements.txt` for full dependency list
