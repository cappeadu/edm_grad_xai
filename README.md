# Graduation-Rate-Prediction-Using-Machine-Learning-and-XAI

This repository contains the code, data, metadata, and visualizations for the research paper titled "Harnessing XAI to Inform Educational Decision-Making: A Machine Learning Study on Graduation Rates". The study uses U.S. institutional-level data from IPEDS (2012–2017) to build predictive models of graduation rates and applies eXplainable AI (XAI) tools to interpret the results.

## 📁 Repository Structure
```
graduation-rate-prediction-using-machine-learning-and-XAI/
├── Data from IPEDS/
│ ├── 2012/ # Raw IPEDS data and metadata
│ ├── ..../ # Raw IPEDS data and metadata
│ ├── ..../ # Raw IPEDS data and metadata
│ └── merged_dataset_for_imputation_and_ML/ # Cleaned and preprocessed data from grad_rate_preprocess.ipynb. Used in grad_rate_training_predict.ipynb for predictions and XAI.
│
├── grad_rate_preprocess.ipynb # Data cleaning & feature engineering
├── grad_rate_training_predict.ipynb # Model training and explainability
│
├── plots/ # SHAP plots, PDPs, and visuals
│
├── requirements.txt # List of Python dependencies
├── README.md # Project overview
└── LICENSE # License information
```

## 🔍 Project Overview
This research explores how machine learning and explainable AI can be used to predict and interpret institutional graduation rates. It:
- Trains six machine learning models including Linear Regression, SVR, Decision Tree, Random Forest, XGBoost, and LightGBM.
- Selects the best model using cross-validation and test set evaluation.
- Applies SHAP, Permutation Importance, PDPs, and ICE plots for feature interpretation.
- Analyzes institutional-level variables like retention rates, tuition, test scores, and demographic disparities.

## 📊 Key Findings

- **SVR** performed best with an R² of 0.8112, followed closely by XGBoost and Random Forest.
- **Retention rate (previous year)** was the strongest predictor of graduation rates.
- Gender and racial disparities in graduation rates also proved critical.
- SHAP and PDPs revealed how individual features and interactions influence predictions.
- Local explanations (force and waterfall plots) demonstrated practical interpretability for individual institutions.

## 📚 Dataset
- Source: Integrated Postsecondary Education Data System (IPEDS)
- Years Covered: 2012–2017
- Level: Institutional-level features

⚠️ Note: Due to size, the final merged dataset has been provided in the Data from IPEDS directory. The file name is merged_dataset_for_imputation_and_ML

## 🛠 How to Run
To run any of the experiments, execute the .ipynb files in notebooks folder.
```
grad_rate_preprocess.ipynb #this contains the processes for data cleaning, feature selection etc

grad_rate_training_predict.ipynb #contains the codes for machine learning and XAI

```
## 📄 Paper Link
[Link to paper: https://zenodo.org/records/18238053](https://zenodo.org/records/18238053)

## 🧠 Author
Clement Appeadu  
MSc Data Science, University of South Wales  
[LinkedIn](https://www.linkedin.com/in/clement-appeadu-9b6a2b148)

## 📃 License
MIT License – see LICENSE file for details.
