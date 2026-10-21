
# Model Deployment

## Introduction

Model deployment integrates a trained machine learning model and its resources into a production environment so that it can generate predictions.

## 1. Deployment Types

### Self-hosted API

A self-hosted API runs a model on infrastructure managed by the organization, either on premises or in the cloud.

The organization manages the required infrastructure, such as servers, containers, load balancers, and databases.

Advantages:
- Greater control over infrastructure.
- Flexibility to customize the environment.
- Potential cost savings depending on usage.

Disadvantages:
- More operational overhead.
- Responsibility for infrastructure maintenance.
- Additional management and scaling requirements.

### Managed API

A managed API service provides a managed environment for hosting ML models.

Amazon SageMaker AI is an example of a managed service that reduces the need to manage underlying infrastructure directly.

The choice between managed and self-hosted APIs depends on cost, control, customization, expertise, and workload requirements.

## 2. Amazon SageMaker AI Deployment

SageMaker AI supports model deployment through a single action or API call.

Its deployment capabilities include:
- Automatic scaling.
- Model hosting services.
- HTTPS endpoints.
- Support for hosting multiple models.

## 3. Inference Options

### Real-time Inference

Real-time inference is appropriate for interactive workloads requiring low-latency predictions.

Example: A customer-facing application that needs an immediate prediction.

### Batch Transform

Batch transform processes large datasets when predictions do not need to be returned immediately through a persistent endpoint.

It can also be used for certain dataset preprocessing tasks.

### Asynchronous Inference

Asynchronous inference queues incoming requests and processes them asynchronously.

It is useful for workloads involving large payloads, long processing times, or near-real-time requirements where an immediate response is unnecessary.

### Serverless Inference

Serverless inference allows models to run without configuring or managing the underlying inference infrastructure.

It is suitable for workloads with idle periods between traffic spikes that can tolerate cold starts.

## 4. Choosing a Deployment Method

Consider the following factors when choosing a deployment method:

- Required response time.
- Request size and processing duration.
- Expected traffic and scaling needs.
- Infrastructure management requirements.
- Cost and available technical expertise.
- Whether predictions are needed individually or in batches.

## Key Takeaways

- Deployment makes a trained model available in a production environment.
- Self-hosted APIs provide control but require infrastructure management.
- Managed APIs reduce operational responsibilities.
- Real-time inference supports low-latency applications.
- Batch transform handles large datasets without a persistent inference endpoint.
- Asynchronous inference supports queued, long-running requests.
- Serverless inference suits intermittent workloads that can tolerate cold starts.
