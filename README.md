# Advanced Credit Risk Prediction: Beyond Traditional Scoring

[![Author](https://img.shields.io/badge/Author-Prakash%20Ukhalkar-blue.svg)](https://github.com/prakash-ukhalkar)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-Latest-red)](https://xgboost.readthedocs.io/)
[![SHAP](https://img.shields.io/badge/SHAP-Latest-blue)](https://shap.readthedocs.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview

This project implements a comprehensive **Dual-Track** credit risk prediction pipeline, designed to handle the distinct financial behaviors of **Individual (Retail)** borrowers and **Corporate** entities. By integrating traditional metrics (like CIBIL scores) with demographic data and corporate health indicators, the system provides a robust framework for financial risk assessment.

A key highlight of this repository is the integration of **Explainable AI (XAI)** using SHAP, ensuring that model decisions are transparent, justifiable, and compliant with regulatory standards.

## Key Features

- **Dual-Track Methodology**: Separate ingestion and modeling pipelines for Retail and Corporate datasets.
- **Automated Profiling & EDA**: Deep statistical analysis and visualization of financial features.
- **Advanced Feature Engineering**: Strategic preprocessing tailored to credit risk indicators.
- **Ensemble Modeling**: Implementation of Random Forest and XGBoost for high-accuracy predictions.
- **XAI Interpretability**: SHAP-based auditing to extract actionable financial insights from "black box" models.

## Project Structure

```text
.
├── data/
│   ├── raw/                # Original source datasets
│   └── processed/          # Cleaned and engineered features
├── models/                 # Serialized model artifacts
├── notebooks/
│   ├── 01_Data_Acquisition_and_Profiling.ipynb
│   ├── 02_Exploratory_Data_Analysis.ipynb
│   ├── 03_Feature_Engineering_and_Preprocessing.ipynb
│   ├── 04_Individual_Risk_Modeling.ipynb
│   ├── 05_Corporate_Risk_Modeling.ipynb
│   └── 06_Model_Interpretability.ipynb
├── reports/                # Generated figures and analysis results
├── requirements.txt        # Project dependencies
└── LICENSE                 # MIT License
```

## Notebook Pipeline Guide

1.  **[01_Data_Acquisition_and_Profiling](notebooks/01_Data_Acquisition_and_Profiling.ipynb)**: Establishes the dual-track ingestion pipeline and performs initial statistical profiling.
2.  **[02_Exploratory_Data_Analysis](notebooks/02_Exploratory_Data_Analysis.ipynb)**: Deep dive into feature distributions, correlations, and risk drivers.
3.  **[03_Feature_Engineering_and_Preprocessing](notebooks/03_Feature_Engineering_and_Preprocessing.ipynb)**: Handles missing values, encoding, and creates specialized financial features.
4.  **[04_Individual_Risk_Modeling](notebooks/04_Individual_Risk_Modeling.ipynb)**: Trains and evaluates models specifically for individual/retail credit risk.
5.  **[05_Corporate_Risk_Modeling](notebooks/05_Corporate_Risk_Modeling.ipynb)**: Develops high-performance models for corporate health and default prediction.
6.  **[06_Model_Interpretability](notebooks/06_Model_Interpretability.ipynb)**: Uses SHAP for XAI auditing, extracting global and local feature importance.

## Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/prakash-ukhalkar/Advanced-Credit-Risk-Prediction.git
   cd Advanced-Credit-Risk-Prediction
   ```

2. **Create a Virtual Environment**:
   ```bash
   python -m venv credit-risk-venv
   source credit-risk-venv/bin/activate  # On Windows: credit-risk-venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
**Maintained by**: [Prakash Ukhalkar](https://github.com/prakash-ukhalkar)
