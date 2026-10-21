
# Developing ML Solutions with Amazon SageMaker AI

## Introduction

Amazon SageMaker AI is a fully managed machine learning service that supports data preparation, model building, training, evaluation, deployment, and monitoring.

## 1. Collecting, Analyzing, and Preparing Data

### Amazon SageMaker Data Wrangler
A low-code/no-code tool for importing, preparing, transforming, featurizing, and analyzing data through a web interface. Python scripts and custom transformations can be added when required.

### SageMaker Studio Classic
Integrates with Amazon EMR and AWS Glue interactive sessions to support large-scale data preparation and ML workflows.

### SageMaker Processing API
Runs scripts and notebooks for data preprocessing, transformation, analysis, feature engineering, and evaluation using supported ML frameworks.

## 2. Managing Features

### Amazon SageMaker Feature Store

Feature Store helps data scientists and ML engineers create, share, store, and manage features used in machine learning.

Stored features can be retrieved and enriched before being supplied to models for inference.

## 3. Model Training and Evaluation

### SageMaker AI Training Jobs
Training jobs use training code and datasets on managed compute instances. Models can use built-in or custom algorithms, and resulting model artifacts can be stored in Amazon S3.

### Amazon SageMaker Canvas
A no-code tool that allows users to generate predictions without writing code.

### Amazon SageMaker JumpStart
Provides pretrained models, solution templates, and example notebooks. Models can be deployed, fine-tuned, and evaluated for different use cases.

### Amazon SageMaker Experiments
Helps compare datasets, algorithms, and parameters to understand their effects on model performance.

### Automatic Model Tuning
Runs training jobs with different hyperparameter combinations and evaluates them using a selected metric to identify suitable configurations.

## 4. Sources of ML Models

### Pretrained Models
Models already trained on existing data. They can be deployed directly when appropriate or fine-tuned for a specific task.

### Built-in Algorithms
Algorithms provided by SageMaker AI for common ML problems.

### ML Frameworks
Supported frameworks include scikit-learn, TensorFlow, PyTorch, MXNet, and Chainer.

### Custom Docker Images
Custom images can be created with the packages and software required for specialized ML workloads.

## 5. SageMaker AI Supported Algorithms

### Supervised Learning
Supports classification and regression using labeled data.

### Unsupervised Learning
Supports clustering, dimensionality reduction, topic modeling, and anomaly detection.

### Image Processing
Supports image classification, object detection, computer vision, and related tasks.

### Text Analysis
Supports natural language processing, document classification, summarization, topic modeling, transcription, and translation.

## 6. Machine Learning Model Performance Evaluation

### Training, Validation, and Test Sets

- Training set: Used to train the model.
- Validation set: Used to assess intermediate performance and guide improvements.
- Test set: Used for final evaluation on held-out data.

### Overfitting
Occurs when a model performs well on training data but poorly on evaluation data because it has learned patterns specific to the training examples.

### Underfitting
Occurs when a model performs poorly on training data because it cannot adequately capture the relationships between inputs and target values.

### Balanced Model
A balanced model avoids excessive overfitting and underfitting and generalizes effectively to unseen data.

### Bias and Variance
Bias describes systematic prediction error, while variance describes how sensitive predictions are to changes in the training data. Good generalization requires an appropriate balance.

## 7. Classification Metrics

### Confusion Matrix
Compares actual and predicted labels.

- True Positive (TP): Actual positive, predicted positive.
- True Negative (TN): Actual negative, predicted negative.
- False Positive (FP): Actual negative, predicted positive.
- False Negative (FN): Actual positive, predicted negative.

### Accuracy
Measures the proportion of all predictions that are correct.

Accuracy = (TP + TN) / (TP + TN + FP + FN)

### Precision
Measures the proportion of positive predictions that are correct.

Precision = TP / (TP + FP)

Useful when false positives are costly, such as incorrectly classifying legitimate emails as spam.

### Recall
Measures the proportion of actual positive cases correctly identified.

Recall = TP / (TP + FN)

Useful when false negatives are costly.

### F1 Score
Combines precision and recall using their harmonic mean.

F1 = 2 × (Precision × Recall) / (Precision + Recall)

### AUC-ROC
Area Under the Receiver Operating Characteristic Curve measures how well a classifier separates classes across different thresholds.

An AUC near 1 indicates strong separation, while an AUC near 0.5 indicates performance similar to random guessing.

## 8. Regression Metrics

### Mean Squared Error (MSE)
Measures the average squared difference between predicted and actual values.

MSE = Sum of squared prediction errors / Number of observations

A smaller MSE generally indicates better predictive accuracy.

### R-squared
Measures the fraction of variance in target values explained by the model. A value closer to 1 often indicates a better fit.

## 9. Business Metrics

Model evaluation should align with business goals such as increasing sales, reducing costs, or decreasing customer churn.

Custom cost functions can assign costs or values to correct predictions and errors. A/B testing and canary deployments help compare model versions and evaluate business impact.

## 10. Model Deployment

### Self-hosted API
The organization deploys and manages the model on its own infrastructure, either on premises or in the cloud.

Advantages include greater infrastructure control and customization, but this approach requires more operational effort.

### Managed API
A managed service, such as SageMaker AI, handles much of the infrastructure management involved in hosting models.

The choice depends on control, customization, cost, available expertise, and use-case requirements.

## 11. SageMaker AI Inference Options

### Real-time Inference
Suitable for interactive applications requiring low-latency responses.

### Batch Transform
Processes large datasets when predictions do not need to be returned through a persistent endpoint.

### Asynchronous Inference
Queues incoming requests and processes them asynchronously. Suitable for large payloads and long processing times.

### Serverless Inference
Runs inference without requiring users to configure or manage the underlying infrastructure. Suitable for workloads with idle periods that can tolerate cold starts.

## Key Takeaways

- SageMaker AI supports the ML lifecycle through managed tools.
- Pretrained models, built-in algorithms, frameworks, and custom images offer different development options.
- Classification and regression require different evaluation metrics.
- Model evaluation should consider business costs and requirements.
- Deployment and inference choices depend on latency, workload size, traffic patterns, and operational needs.
