# Machine Learning

## 1. Overview of Machine Learning

Machine Learning (ML) is a subset of AI that develops algorithms and statistical models capable of learning from data and making predictions or decisions without being explicitly programmed for every situation.

ML models learn patterns and relationships from data rather than relying only on hard-coded rules.

## 2. When AI and ML Are Appropriate Solutions

AI and ML are appropriate when a problem is difficult to solve using predefined rules or must be handled at a large scale.

### 2.1 Coding the Rules Is a Challenge

Some tasks involve complex relationships, overlapping conditions, and too many variables for humans to define accurate rules manually.

**Example: Spam filtering**

Spam emails differ in wording, format, sender, and content. Creating rules for every possible situation is difficult. ML can learn patterns from existing emails and classify new emails.

### 2.2 Scale of the Project Is a Challenge

Tasks that can be handled manually may become inefficient when the data volume increases.

**Example: Email classification**

A person may inspect hundreds of emails, but examining millions would be time-consuming. An ML-based system can process large volumes automatically.

## 3. Alternative Approaches

AI and ML are not always necessary. Rule-based programming or direct computation may be more appropriate when the problem has a clearly defined solution.

**Example:**

```python
total_price = quantity * unit_price
```

The total price can be calculated directly without training an ML model.

**Key principle:** Choose the solution based on the problem's requirements and constraints rather than using AI simply because it is available.

## 4. Machine Learning Techniques

The three major machine learning techniques are:

1. Supervised learning
2. Unsupervised learning
3. Reinforcement learning

```text
                 ML Techniques
                      |
          +-----------+-----------+
          |           |           |
      Supervised  Unsupervised  Reinforcement
       Learning     Learning      Learning
          |           |
      +---+---+   +---+----------------+
      |       |   |                    |
Classification | Regression      Clustering
                              Dimensionality
                                Reduction
```

| Technique | Training Information | Main Goal |
|---|---|---|
| Supervised learning | Labeled data | Predict outputs for new inputs |
| Unsupervised learning | Unlabeled data | Discover patterns and structures |
| Reinforcement learning | Rewards and penalties | Learn actions that maximize rewards |

## 5. Supervised Learning

Supervised learning uses labeled training data. Each example contains input features and a known output or target.

The algorithm learns the relationship between inputs and outputs to predict results for new, unseen data.

**Example: Car image classification**

1. Provide images labeled as cars.
2. The model learns visual patterns associated with cars.
3. Provide a new, unlabeled image.
4. The model predicts whether the image contains a car.

### 5.1 Classification

Classification assigns labels or categories to new data instances.

**Use cases:**
- Fraud detection
- Image classification
- Customer retention prediction
- Medical diagnostics

**Example:** A model learns from transactions labeled as fraudulent or legitimate and classifies new transactions.

### 5.2 Regression

Regression predicts continuous or numerical values based on one or more input variables.

- **Dependent variable:** The numerical value being predicted.
- **Independent variables:** The input features used for prediction.

**Use cases:**
- Advertising popularity prediction
- Weather forecasting
- Market forecasting
- Estimating life expectancy
- Population growth prediction

**Example:** A model predicts temperature using historical temperature, humidity, and atmospheric measurements.

### Classification vs Regression

| Feature | Classification | Regression |
|---|---|---|
| Output | Category or class | Numerical value |
| Example | Fraudulent or legitimate | Predicted temperature |
| Use case | Image classification | Market forecasting |

## 6. Unsupervised Learning

Unsupervised learning uses unlabeled data. The algorithm discovers hidden patterns, similarities, relationships, or structures without predefined target labels.

### 6.1 Clustering

Clustering groups data points into clusters based on similarities in their features or distances between them.

**Use cases:**
- Customer segmentation
- Targeted marketing
- Recommendation systems

**Example:** An e-commerce company groups customers according to purchasing habits to develop targeted marketing strategies.

### 6.2 Dimensionality Reduction

Dimensionality reduction reduces the number of features in a dataset while preserving its most important information or patterns.

**Use cases:**
- Big data visualization
- Meaningful compression
- Structure discovery
- Feature extraction

**Example:** A dataset containing hundreds of features can be transformed into fewer dimensions to make visualization and analysis easier.

## 7. Reinforcement Learning

Reinforcement learning is a technique in which an agent learns by interacting with an environment and receiving rewards or penalties for its actions.

The agent improves its decisions through repeated interactions and trial and error.

### 7.1 Key Components

- **Agent:** The entity that learns and takes actions.
- **Environment:** The surroundings in which the agent operates.
- **Action:** A decision or operation performed by the agent.
- **Reward:** Feedback indicating how desirable an outcome is.
- **Policy:** The strategy used to select actions.

### 7.2 Working

1. The agent observes the environment.
2. It selects and performs an action.
3. The environment responds.
4. The agent receives a reward or penalty.
5. The agent updates its behavior.
6. The process repeats to improve decision-making.

### 7.3 Example: AWS DeepRacer

AWS DeepRacer provides a simulator in which a virtual car learns to navigate a racetrack.

| Component | Example |
|---|---|
| Agent | Virtual car |
| Environment | Virtual racetrack |
| Actions | Throttle and steering inputs |
| Reward | Feedback encouraging desired driving behavior |
| Goal | Complete the track quickly without deviating |

## 8. Summary

| Learning Technique | Main Categories | Example Use Cases |
|---|---|---|
| Supervised learning | Classification, regression | Fraud detection, weather forecasting |
| Unsupervised learning | Clustering, dimensionality reduction | Customer segmentation, data visualization |
| Reinforcement learning | Learning through rewards and penalties | Simulated driving, autonomous control |

Supervised learning predicts known categories or numerical values, unsupervised learning discovers hidden structures, and reinforcement learning improves decisions through feedback.
