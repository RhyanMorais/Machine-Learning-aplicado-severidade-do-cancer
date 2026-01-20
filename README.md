Machine Learning Applied to Cancer Severity Analysis (2015–2024)

This project applies classical machine learning techniques to analyze factors associated with cancer severity using patient-level data from 2015 to 2024.

Objective

Identify and evaluate how demographic, behavioral, environmental and clinical variables relate to cancer severity, using supervised machine learning models for both classification and regression tasks.

Dataset

The dataset contains patient information such as:

Age and gender

Country and year

Genetic risk indicators

Lifestyle factors such as smoking, alcohol use and obesity

Environmental factors such as air pollution

Cancer type and stage

Survival time

The target variable represents cancer severity, originally defined as a continuous severity score. This variable was used directly for regression models and discretized into three severity levels (low, moderate and severe) for classification tasks.

Approach

The analysis follows these steps:

Data loading using relative paths for reproducibility

Data cleaning and preprocessing

Removal of non-informative identifiers

Encoding of categorical variables

Creation of dummy variables for selected features

Feature scaling

Train-test split

Feature selection using Spearman correlation

Training and evaluation of classical machine learning models

Performance comparison using task-appropriate metrics

Models

The following classical machine learning models were explored.

Classification models

Logistic Regression

Decision Tree Classifier

Random Forest Classifier

SGDClassifier

Regression models

Linear Regression

Decision Tree Regressor

Random Forest Regressor

SGD Regressor

Evaluation Metrics

Different metrics were used according to the problem type.

For classification:

Accuracy

Precision

Recall

F1-score

For regression:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

R² score

The F1-score was especially important in classification due to the multiclass nature of the problem. In regression, MAE and R² were prioritized for interpretability and explanatory power.

Results and Analysis

In the classification task, Logistic Regression achieved the highest overall accuracy, around 70 percent, with balanced performance across classes. Random Forest produced similar results, while Decision Tree and SGDClassifier showed lower performance. The close performance among classifiers suggests that the discretized severity patterns are well captured by linear decision boundaries.

In the regression task, Linear Regression achieved the best overall performance, with the lowest prediction error and the highest R² score, explaining approximately 79 percent of the variance in cancer severity. This result indicates a strong linear relationship between the selected features and the severity score. Tree-based regression models showed slightly lower performance, possibly due to unnecessary complexity for the underlying data structure.

Feature selection analysis identified smoking, genetic risk, air pollution, alcohol use and obesity level as the most relevant variables associated with cancer severity.

Conclusion

The results indicate that regression-based approaches were more effective than classification models for predicting cancer severity in this dataset. Linear Regression stood out as the best-performing model due to its simplicity, stability and interpretability.

The proposed approach demonstrates potential applicability in clinical triage scenarios, supporting severity estimation and treatment prioritization. A key limitation is the inclusion of treatment cost as a feature, which occurs after severity assessment and may introduce bias. Future work should address this issue and explore additional validation strategies.

How to Run

Install dependencies:

pip install -r requirements.txt

Open the notebook:

02_machine_learning_cancer_severity_analysis_2015_2024.ipynb

You can run it locally or directly in Google Colab using the Open in Colab button.
