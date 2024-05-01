## Exploring-Tree-Based-Algorithms-for-Data-Analysis

## Project Overview
This project leverages tree-based machine learning algorithms, including Decision Trees and Random Forests, to analyze loan repayment data. The goal is to identify factors influencing loan repayment abilities and predict loan default risks.

## Contents
- Introduction to tree-based models
- Data preprocessing
- Implementation of Decision Tree Classifier
- Implementation of Random Forest Classifier
- Implementation of Gradient Boosting Machine
- Comparison of model performance
- Conclusion and future work

## Objective
The primary goal is to understand the predictive power of tree-based models in assessing loan repayment risks and to compare the performance and variable importance identified by Decision Trees and Random Forests.

## Tools Used
-Python
-Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

## How to Run the Notebook
- Clone the repository to your local machine.
- Ensure Python and the necessary libraries are installed.
- Run the Jupyter notebook through Jupyter Lab or Jupyter Notebook environment.
Analysis of Outputs
For each model implemented:

## Analysis of Outputs
# Decision Tree Model
- Model Performance: The initial unpruned Decision Tree model achieved a training accuracy of 93.87% and a testing accuracy of 89.95%. This indicates a potential overfitting issue as seen by the discrepancy between training and testing performance.
- Visualization: The decision tree was visualized to show the classification rules with Education Type at the top, indicating its primary importance in predicting outcomes.
# Decision Tree Pruning
- Improved Generalization: After pruning to a maximum depth of 3, both training and testing accuracies converged to around 92%, reducing overfitting and improving the model's generalization to unseen data.
- Simplified Model: The pruned tree focuses on the most significant predictors and is easier to interpret.
# Random Forest Model
- Robust Performance: The Random Forest model showed no overfitting, with both training and testing accuracies around 91.99%. This consistency suggests that Random Forests manage bias and variance more effectively than a single Decision Tree.
- Visualization of Ensemble: The first five trees of the Random Forest were plotted to demonstrate the diversity within the ensemble, which helps in averaging out errors and improving accuracy.
# Model Comparison and Insights
- Variable Importance: Correlation analysis highlighted the most significant variables related to the target variable. Variables like DAYS_BIRTH, REGION_RATING_CLIENT, and DAYS_LAST_PHONE_CHANGE showed strong positive correlations with the target, indicating higher importance in predicting loan defaults.
- Negative Correlations: Variables like EXT_SOURCE_1, EXT_SOURCE_2, and EXT_SOURCE_3 showed strong negative correlations, suggesting that higher values of these external sources are associated with lower chances of default.

Model Description: Provide a brief overview of the model.
Key Observations: Discuss the accuracy, precision, recall, and other relevant metrics.
Visualizations: Analyze any plots comparing model performances or showing important features.
Conclusions: What can be inferred from the comparisons? Which model performs best and under what conditions?
Future Work
Suggestions on how the models might be improved, potential data to include, or other algorithms to explore.
