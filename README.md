# Churn Experiment 1 --- MLOps Churn Prediction

## 📌 Project Overview

This project implements an end-to-end **MLOps workflow for customer
churn prediction**.

The goal is to build a reproducible machine learning pipeline that takes
customer data, validates and preprocesses it, trains a churn prediction
model, evaluates the model, and tracks the experiment using MLOps
practices.

## 🎯 Objectives

-   Prepare and validate customer churn data.
-   Perform preprocessing and feature transformation.
-   Train a machine learning model for churn prediction.
-   Evaluate model performance using suitable metrics.
-   Track experiments and model runs using MLflow.
-   Validate outputs and reproducibility.
-   Organize the project using a structured MLOps directory layout.

## 🗂️ Project Structure

``` text
Churn-Experiment1/
│
├── configs/                    # Configuration files
├── data/
│   ├── raw/                    # Original/raw dataset
│   └── processed/              # Processed dataset
│
├── logs/                       # Logs generated during experiments
├── models/                     # Saved trained models and preprocessing objects
├── notebooks/
│   └── project_implementation.ipynb
│
├── outputs/                    # Generated prediction/results files
├── pipelines/                  # End-to-end and experiment pipeline scripts
│   ├── run_lab3_baseline.py
│   ├── run_lab4_tracking.py
│   └── run_lab5_pipeline.py
│
├── reports/                    # Reports and evaluation results
├── src/                        # Main source code
│   ├── evaluate.py
│   ├── preprocess_pipeline.py
│   ├── preprocess.py
│   ├── train_mlflow.py
│   ├── train.py
│   ├── validate_data.py
│   ├── validate_outputs.py
│   └── validate_reproducibility.py
│
├── .gitignore                  # Files/folders excluded from Git
└── requirements.txt            # Python dependencies
```

## 🔄 MLOps Workflow

``` text
Raw Data
   ↓
Data Validation
   ↓
Preprocessing
   ↓
Feature Transformation
   ↓
Model Training
   ↓
Experiment Tracking
   ↓
Model Evaluation
   ↓
Output Validation
   ↓
Reproducibility Validation
```

## 🛠️ Technologies Used

-   Python
-   Pandas
-   NumPy
-   Scikit-learn
-   MLflow
-   Jupyter Notebook
-   Git
-   GitHub

## 📊 Dataset

The project uses a **customer churn dataset** containing customer
information and a churn target.

The raw dataset should be placed inside:

``` text
data/raw/
```

Processed data is stored in:

``` text
data/processed/
```

## ▶️ How to Run

### 1. Clone the repository

``` bash
git clone https://github.com/saisribhavitha-arch/MlopsProject_Churndata.git
cd MlopsProject_Churndata
```

### 2. Create a virtual environment

``` bash
python -m venv .venv
```

### 3. Activate the environment on Windows

``` powershell
.venv\Scripts\Activate.ps1
```

### 4. Install dependencies

``` bash
pip install -r requirements.txt
```

### 5. Run the preprocessing step

``` bash
python src/preprocess.py
```

### 6. Train the model

``` bash
python src/train.py
```

### 7. Evaluate the model

``` bash
python src/evaluate.py
```

## 🧪 Experiment Pipelines

The `pipelines/` directory contains scripts for different stages of the
MLOps experiment:

-   `run_lab3_baseline.py` --- baseline experiment
-   `run_lab4_tracking.py` --- experiment tracking
-   `run_lab5_pipeline.py` --- complete pipeline execution

Run a pipeline using:

``` bash
python pipelines/run_lab5_pipeline.py
```

## 📈 Experiment Tracking

MLflow is used to track machine learning experiments, including model
runs and relevant parameters and metrics.

The tracking workflow is implemented in:

``` text
src/train_mlflow.py
```

## ✅ Validation

The project includes separate validation scripts for:

-   Input data validation
-   Output validation
-   Reproducibility validation

These are located in:

``` text
src/
```

## 👩‍💻 Author

**Bhavitha Sai Sri**

GitHub: `saisribhavitha-arch`

## 📄 License

This project is created for educational and academic purposes.
