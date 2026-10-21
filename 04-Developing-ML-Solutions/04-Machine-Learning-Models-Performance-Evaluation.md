
# Machine Learning Models Performance Evaluation

## Introduction

Model evaluation measures how effectively a trained machine learning model makes predictions on data it has not seen during training.

The appropriate evaluation method depends on whether the problem involves classification or regression.

## 1. Model Evaluation Datasets

### Training Set
Used to train the model.

### Validation Set
Used to evaluate intermediate performance and guide improvements before the final test.

### Test Set
Used for the final assessment of predictive quality on held-out data.

## 2. Model Fit

### Overfitting
A model performs well on training data but poorly on evaluation data because it has learned patterns specific to the training examples.

### Underfitting
A model performs poorly on training data because it cannot adequately capture the relationships between input features and target values.

### Balanced Model
A balanced model avoids excessive overfitting and underfitting and generalizes effectively to unseen examples.

## 3. Bias and Variance

Bias describes the difference between expected predictions and actual target values.

Variance describes the degree to which predictions change when the training data changes.

A model should balance bias and variance to achieve good generalization.

## 4. Classification Metrics

### Confusion Matrix

A confusion matrix compares predicted classes with actual classes.

- True Positive (TP): Actual positive and predicted positive.
- True Negative (TN): Actual negative and predicted negative.
- False Positive (FP): Actual negative but predicted positive.
- False Negative (FN): Actual positive but predicted negative.

### Accuracy

Accuracy measures the proportion of correct predictions.

Accuracy = (TP + TN) / (TP + TN + FP + FN)

Accuracy can be less useful when classes are highly imbalanced.

### Precision

Precision measures the proportion of positive predictions that are actually positive.

Precision = TP / (TP + FP)

Precision is useful when false positives are costly.

### Recall

Recall measures the proportion of actual positive cases correctly identified.

Recall = TP / (TP + FN)

Recall is useful when false negatives are costly.

### F1 Score

The F1 score combines precision and recall using their harmonic mean.

F1 = 2 × (Precision × Recall) / (Precision + Recall)

### AUC-ROC

AUC-ROC evaluates how well a classifier separates classes across different thresholds.

- An AUC near 1 indicates strong separation.
- An AUC near 0.5 indicates performance similar to random guessing.

The appropriate classification threshold depends on the business use case and the costs of errors.

## 5. Regression Metrics

### Mean Squared Error (MSE)

MSE measures the average squared difference between predicted values and actual values.

MSE = Sum of squared prediction errors / Number of observations

A smaller MSE generally indicates better predictive accuracy.

### R-squared

R-squared measures the proportion of variance in target values explained by the model.

A value closer to 1 often indicates a better fit, although it should be interpreted alongside other metrics.

## 6. Business Metrics

Technical metrics should align with the business objectives defined at the beginning of the project.

Examples include:
- Increasing sales.
- Reducing costs.
- Decreasing customer churn.
- Reducing unnecessary maintenance.
- Improving customer experience.

A custom cost function can represent the economic impact of correct predictions and errors.

A/B testing and canary deployments can compare model variants and help determine whether changes improve business outcomes.

## Key Takeaways

- Use separate training, validation, and test datasets.
- Overfitting and underfitting indicate different model problems.
- Classification metrics measure different aspects of predictive performance.
- MSE and R-squared provide different perspectives on regression.
- The most appropriate metric depends on the model and business requirements.
