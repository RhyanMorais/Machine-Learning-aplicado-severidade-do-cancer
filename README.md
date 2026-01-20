# Machine Learning Applied to Cancer Severity Analysis (2015–2024)

This project applies classical machine learning techniques to analyze factors associated with cancer severity using patient-level data from 2015 to 2024.

## Objective
Identify and evaluate how demographic, behavioral, environmental and clinical variables relate to cancer severity, using supervised machine learning models.

## Dataset
The dataset contains patient information such as:
- Age and gender
- Country and year
- Genetic risk indicators
- Lifestyle factors (smoking, alcohol use, obesity)
- Environmental factors (air pollution)
- Cancer type and stage
- Survival time

The target variable represents cancer severity, derived from a severity score and discretized for classification tasks.

## Approach
The analysis follows these steps:
- Data loading using relative paths for reproducibility
- Data cleaning and preprocessing
- Encoding of categorical variables
- Feature scaling
- Train-test split
- Training and evaluation of classical machine learning models
- Performance comparison using appropriate metrics

## Models
Examples of models explored include:
- Decision Tree
- Random Forest
- Other classical regression and classification algorithms

## Results
The project evaluates model performance and discusses which features contribute most to cancer severity, highlighting the strengths and limitations of classical machine learning approaches for this problem.

## How to Run
Install dependencies:
```bash
pip install -r requirements.txt
```
Open the notebook:

02_machine_learning_cancer_severity_analysis_2015_2024.ipynb

You can run it locally or directly in Google Colab using the Open in Colab button.
