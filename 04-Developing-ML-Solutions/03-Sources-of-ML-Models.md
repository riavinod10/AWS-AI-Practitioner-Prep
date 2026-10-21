
# Sources of ML Models

## Introduction

Amazon SageMaker AI supports pretrained models, built-in algorithms, and custom Docker images. The appropriate implementation depends on the problem, available data, required customization, and resources.

## 1. Pretrained Models

Pretrained models require relatively little development effort because they have already been trained on existing data.

They can be deployed directly when suitable or fine-tuned for a specific use case.

Amazon SageMaker JumpStart provides access to pretrained models.

## 2. Built-in Algorithms

SageMaker AI provides built-in algorithms for common machine learning problems.

These algorithms can be useful when an existing solution meets the requirements and the workload needs to scale to large datasets.

## 3. ML Frameworks

When built-in algorithms do not meet the requirements, developers can use supported machine learning and deep learning frameworks.

Examples include:

- scikit-learn
- TensorFlow
- PyTorch
- MXNet
- Chainer

These frameworks allow developers to create and train custom models.

## 4. Custom Docker Images

Developers can build custom Docker images containing the packages, libraries, and software required for a particular ML workload.

This option provides flexibility when standard images or existing solutions are insufficient.

## 5. SageMaker AI Supported Algorithms

### Supervised Learning

Supervised learning uses labeled data and supports classification and regression problems.

### Unsupervised Learning

Unsupervised learning identifies patterns in unlabeled data.

Applications include clustering, dimensionality reduction, topic modeling, and anomaly detection.

### Image Processing

Image-processing algorithms support image classification, object detection, computer vision, and related tasks.

### Text Analysis

Text-analysis algorithms support natural language processing tasks, including document classification, summarization, topic modeling, transcription, and translation.

## 6. Amazon SageMaker JumpStart

SageMaker JumpStart provides pretrained open-source models from different providers.

It supports:
- Deploying pretrained models.
- Fine-tuning models.
- Evaluating models.
- Using solution templates for common use cases.
- Exploring runnable example notebooks.

JumpStart helps developers get started with ML solutions without building every model from scratch.

## Key Takeaways

- Pretrained models are suitable when an existing model can meet the requirements.
- Built-in algorithms provide ready-made solutions for common ML problems.
- Frameworks enable custom model development.
- Custom Docker images support specialized software requirements.
- SageMaker JumpStart simplifies access to pretrained models and example solutions.
