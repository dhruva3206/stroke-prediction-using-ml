# Stroke Prediction Using Machine Learning

## Overview

This project explores the application of machine learning classification algorithms to predict stroke occurrence using demographic, medical, and lifestyle related features.

The project involves data cleaning, exploratory data analysis, feature preprocessing, model development, and performance evaluation to understand how different machine learning algorithms perform on a binary classification problem.

## Objectives

* Perform data cleaning and exploratory data analysis.
* Investigate relationships between patient characteristics and stroke occurrence.
* Prepare numerical and categorical features for machine learning.
* Develop and compare machine learning classification models.
* Evaluate model performance using appropriate classification metrics.
* Identify limitations and potential improvements.

## Dataset

The project uses the **Stroke Prediction Dataset** available on Kaggle.

The dataset contains demographic, medical, and lifestyle related information, including age, gender, hypertension, heart disease, average glucose level, BMI, smoking status, and stroke occurrence.

**Dataset source:** [Stroke Prediction Dataset — Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

## Methodology

### 1. Data Cleaning

* Examined the dataset structure and data types.
* Identified and handled missing values where necessary.
* Checked for data quality issues and prepared the dataset for analysis.

### 2. Exploratory Data Analysis (EDA)

* Analysed feature distributions and relationships with the target variable.
* Investigated the distribution of stroke and non-stroke cases.
* Examined potential patterns in demographic and medical characteristics.

### 3. Data Preprocessing

* Prepared numerical and categorical features for modelling.
* Applied appropriate encoding and preprocessing techniques.
* Split the data into training and testing sets to evaluate model performance on unseen observations.

### 4. Model Development

* Implemented the machine learning classification algorithms explored in the notebook.
* Trained the models using the prepared training data.
* Compared their predictive performance using a consistent evaluation approach.

### 5. Model Evaluation

Model performance was assessed using the evaluation metrics implemented in the project, which may include:

* **Accuracy:** Proportion of correctly classified observations.
* **Precision:** Proportion of predicted stroke cases that were actual stroke cases.
* **Recall:** Proportion of actual stroke cases correctly identified.
* **F1-score:** Balance between precision and recall.

Since stroke cases are relatively uncommon in this dataset, accuracy alone may provide a misleading impression of model performance. Recall and precision are particularly important when assessing the identification of positive cases.

## Results and Interpretation

The models were compared to evaluate their ability to predict stroke occurrence.

**Key findings:** 
* The original Decision Tree achieved a recall of 20% and an F1 score of
* 17.86%, providing a better balance between identifying stroke cases and avoiding false-positive predictions than the other models
* Hyperparameter tuning of the Decision Tree improved recall to 72%.
* However, precision decreased to 8.63%, while accuracy fell to 61.35%
* This illustrates the trade-off between identifying more actual stroke cases and generating more false-positive predictions
* Overall, no model demonstrated consistently strong performance across all evaluation metrics

<img width="438" height="170" alt="image" src="https://github.com/user-attachments/assets/245b21da-b750-485d-9754-a8f90263e177" />

## Limitations

* The dataset may not be representative of all populations or healthcare settings.
* Class imbalance can affect the ability of models to identify stroke cases.
* Performance on a held-out test set does not guarantee similar results on new populations.
* The models have not been established as clinically validated diagnostic or screening tools.

## Future Improvements

Potential improvements include:

* Hyperparameter tuning using GridSearchCV.
* Exploring additional classification algorithms and ensemble methods.
* Investigating appropriate class-weighting or resampling techniques.
* Comparing models using precision-recall curves and ROC-AUC.
* Evaluating probability calibration and classification thresholds.
* Validating the final model on an independent dataset.

## Libraries Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib and Seaborn
* Jupyter Notebook

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries.
3. Download the dataset from the Kaggle source provided above.
4. Place the dataset in the location specified in the notebook.
5. Open the notebook in Jupyter Notebook, JupyterLab, or VS Code.
6. Execute the notebook cells in order.

## Acknowledgments & Data Source

This project utilizes the **Stroke Prediction Dataset**.

* **Dataset source:** [Kaggle — Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)
* **Dataset curator/uploader:** [fedesoriano](https://www.kaggle.com/fedesoriano)

