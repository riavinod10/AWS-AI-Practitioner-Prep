
# Machine Learning Development Lifecycle

## Introduction

The machine learning (ML) development lifecycle is the end-to-end process of developing, deploying, monitoring, and maintaining machine learning models.

The main phases are business goal identification, ML problem framing, data processing, model development, model deployment, model monitoring, and model retraining.

## 1. Business Goal Identification

The process begins with a business objective. Stakeholders identify the expected value, budget, and success criteria for the ML workload.

Key Performance Indicators (KPIs) help determine whether the solution meets the business requirements.

## 2. ML Problem Framing

Problem framing converts a business problem into a machine learning problem.

Data scientists, data engineers, ML architects, and subject matter experts work together to determine whether ML is suitable, whether sufficient data is available, and what resources are required.

## 3. Data Processing

Data processing converts raw data into a usable format.

### Data Collection and Integration
Collects data from different sources and makes it accessible in a central location.

### Data Preprocessing and Visualization
Cleans and transforms raw data. Visualization helps identify patterns, understand distributions, and detect issues.

### Feature Engineering
Creates, transforms, extracts, and selects variables that help the model learn useful patterns.

## 4. Model Development

Model development includes model training, tuning, and evaluation.

It is an iterative process. Developers may modify features, adjust hyperparameters, try different approaches, and retrain the model to improve performance.

## 5. Model Retraining

If a model does not meet the required business goals, developers revisit the data, features, and training parameters to improve it.

Retraining may also be required when new data becomes available or data patterns change.

## 6. Model Deployment

When the model achieves satisfactory results, it is deployed into production to generate predictions, also called inferences.

## 7. Model Monitoring

Monitoring checks whether the deployed model maintains the required performance.

It helps identify declining model quality, data changes, and issues that require investigation or corrective action.

## 8. Iterations

The ML lifecycle is iterative. Models are continuously improved as new data becomes available and business requirements change.

Successful ML development requires collaboration between product managers, developers, data scientists, and engineers.

## Use Case: Amazon Call Center

### Business Goals
Amazon wanted to improve customer service call routing. Its traditional menu-based system could direct customers to the wrong agents, increasing call transfers, costs, and waiting time.

### Problem Formulation
The goal was to predict which agent skill would best resolve a customer's issue. This was framed as a multiclass classification problem.

### Data Collection and Integration
Historical customer service data was used for supervised learning. Features included recent orders, Kindle ownership, and Prime membership.

### Data Preprocessing and Visualization
The team examined labels, combined similar categories where appropriate, and analyzed the distribution of calls.

### Model Training
The data was divided into training, validation, and testing subsets. Common splits include 80/10/10 and 70/15/15.

### Model Evaluation
The model was evaluated using unseen data to estimate how well it would generalize to future customer calls.

### Model Tuning and Feature Engineering
Hyperparameters and input features were adjusted to improve predictions.

### Model Deployment
The model helped customers reach the appropriate agent on their first attempt, reducing call transfers and improving customer experience.

## Key Takeaways

- Define business objectives before developing an ML model.
- Frame the business problem as an appropriate ML task.
- Prepare data and engineer useful features.
- Train, evaluate, and tune models iteratively.
- Deploy models only after satisfactory evaluation.
- Monitor production models and retrain when necessary.
