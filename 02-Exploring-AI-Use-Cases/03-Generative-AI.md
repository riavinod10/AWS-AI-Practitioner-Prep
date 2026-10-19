# Generative AI

## 1. Overview of Generative AI

Generative AI is a subset of deep learning that generates new content based on patterns and structures learned from training data.

It can generate conversations, stories, images, videos, music, and code. It can also automate repetitive tasks, analyze information, and support creative work.

## 2. Capabilities of Generative AI

### 2.1 Adaptability

Generative AI models can adapt to different tasks and domains by producing content suited to specific contexts and requirements.

**Example:** A language model can assist with customer support, summarize reports, and generate product descriptions.

### 2.2 Responsiveness

Generative AI models can respond rapidly to incoming prompts. This is useful for chatbots, virtual assistants, and interactive applications.

### 2.3 Simplicity

Generative AI simplifies complex or repetitive tasks by automating content creation.

**Example:** Generating an initial draft of a report reduces manual effort.

### 2.4 Creativity and Exploration

Generative AI can produce new ideas, designs, and possible solutions by combining learned patterns in different ways.

**Example:** A designer can explore multiple product designs before selecting one.

### 2.5 Data Efficiency

Some generative AI models can learn from relatively small amounts of data and generate samples consistent with learned patterns. This is useful when data is scarce or difficult to obtain.

### 2.6 Personalization

Generative AI can create content tailored to individual preferences or characteristics.

**Example:** An e-commerce platform generates personalized product recommendations or marketing messages.

### 2.7 Scalability

Once trained and deployed, generative AI models can produce large amounts of content quickly.

**Example:** Generating descriptions for thousands of product listings.

## 3. Challenges of Generative AI

### 3.1 Regulatory Violations

**Risk:** Models may generate outputs that expose personally identifiable information (PII) or violate privacy regulations.

**Mitigation:**
- Anonymize or pseudonymize sensitive data.
- Use privacy-preserving techniques.
- Audit training data and model behavior.
- Assess compliance with relevant regulations.

### 3.2 Social Risks

**Risk:** Models may generate unwanted or inappropriate content that harms individuals or an organization's reputation.

**Mitigation:**
- Test and evaluate models before production deployment.
- Establish acceptable-use policies.
- Monitor outputs and collect feedback.
- Implement safeguards.

### 3.3 Data Security and Privacy

**Risk:** Information supplied to a model may contain personal or confidential data, potentially resulting in unauthorized exposure.

**Mitigation:**
- Encrypt data in transit and at rest.
- Enforce least-privilege access controls.
- Redact or pseudonymize PII.
- Include only the minimum context required.
- Use system-level instructions to establish behavioral boundaries.
- Configure Amazon Bedrock Guardrails to filter PII, harmful content, and restricted topics.

### 3.4 Toxicity

**Risk:** Models may generate offensive, inflammatory, or inappropriate content.

**Mitigation:**
- Curate training data to reduce harmful content.
- Test models for undesirable outputs.
- Use guardrails and filtering mechanisms.

### 3.5 Hallucinations

**Risk:** A model may generate convincing but inaccurate or unsupported information. These outputs are called hallucinations.

**Mitigation:**
- Verify important claims using independent sources.
- Require human review for high-impact decisions.
- Clearly identify unverified content.
- Do not treat generated outputs as automatically factual.

### 3.6 Interpretability

**Risk:** Users may misunderstand model outputs or be unable to understand how a model arrived at a result.

**Mitigation:**
- Provide relevant domain context.
- Communicate limitations.
- Use suitable explanations and supporting information.
- Evaluate whether outputs are understandable to intended users.

### 3.7 Nondeterminism

**Risk:** A model may produce different outputs for the same input, creating reliability issues.

**Mitigation:**
- Run repeated tests using the same inputs.
- Compare outputs for consistency.
- Identify sources of variation.
- Configure model parameters appropriately.

### Summary of Challenges

| Challenge | Risk | Mitigation |
|---|---|---|
| Regulatory violations | Legal or regulatory breaches | Privacy protection and compliance audits |
| Social risks | Harmful or reputationally damaging content | Testing and evaluation |
| Security and privacy | Exposure of sensitive information | Encryption, access control, and data minimization |
| Toxicity | Offensive or inappropriate outputs | Data curation and guardrails |
| Hallucinations | Incorrect or fabricated information | Independent verification |
| Interpretability | Misunderstanding outputs | Explanations and domain context |
| Nondeterminism | Inconsistent responses | Repeated testing |

## 4. Factors to Consider When Selecting a Generative AI Model

Model selection depends on the intended task, performance requirements, technical constraints, compliance obligations, and cost.

### 4.1 Model Types

Different foundation models are designed or optimized for different tasks.

| Provider | Model | Tasks | Example Use Cases |
|---|---|---|---|
| AI21 Labs | Jurassic-2 | Text generation, summarization, paraphrasing, chat, information extraction | Financial document summaries and product descriptions |
| Amazon | Amazon Titan | Summarization, classification, question answering, information extraction, embeddings, search | Image creation and customer-service summaries |
| Anthropic | Claude | Content generation, translation, question answering, summarization, code explanation and generation | Code generation, debugging, legal document analysis |
| Stability AI | Stable Diffusion | Photorealistic image generation and image-quality improvement | Game environments, advertising assets |
| Cohere | Command | Text generation, information extraction, question answering, summarization | Customer-service chatbots and document summaries |
| Meta | Llama | Question answering, chat, summarization, paraphrasing, sentiment analysis, text generation | Customer-service support |

Amazon Bedrock provides access to a selection of foundation models from multiple providers.

Resources:
- [Amazon Bedrock](https://aws.amazon.com/bedrock/)
- [What Are Foundation Models?](https://aws.amazon.com/what-is/foundation-models/)

### 4.2 Performance Requirements

Performance requirements determine whether a model meets the application's needs.

Important considerations include:

- **Accuracy:** Correctness of outputs.
- **Reliability:** Consistency of useful results.
- **Response time:** Speed of generating results.
- **Quality:** Whether content meets the required standard.
- **Consistency:** Stability across repeated uses.

Test models with relevant datasets and monitor performance after deployment.

### 4.3 Constraints

Constraints are limitations that affect model selection, deployment, and operation.

- **Computational resources:** Available CPU, GPU, memory, and processing capacity.
- **Data availability:** Size, quality, and availability of training or contextual data.
- **Deployment requirements:** Whether the model must run on premises or in the cloud.
- **Infrastructure limitations:** Whether the environment can support the model.

Larger models may require more resources and have fewer practical deployment options than smaller models.

### 4.4 Capabilities

Capabilities refer to the tasks a model can perform and the quality or degree of control it offers.

- Some models specialize in text generation.
- Some focus on image generation.
- Others support multimodal tasks, such as processing text and images together.

Select a model whose capabilities match the application's functional requirements.

### 4.5 Compliance

Compliance involves ensuring that the model and its use meet legal, regulatory, ethical, and organizational requirements.

Important considerations include:

- Fairness and bias
- Transparency and traceability
- Accountability
- Hallucinations and reliability
- Toxicity and harmful content
- Privacy and data protection
- Applicable regulations and ethical guidelines

Compliance is particularly important in healthcare, finance, and legal services.

### 4.6 Cost

Generative AI models differ in cost, speed, size, and deployment requirements.

- **Larger models:** May provide stronger performance for complex tasks but often require more resources and cost more to operate.
- **Smaller models:** May be faster, cheaper, and easier to deploy, depending on the use case.

Organizations should evaluate the trade-off between model size, speed, quality, and cost.

Total expenses may include deployment, maintenance, hardware, software, and other associated costs.

Using generative AI to automate repetitive content creation can reduce labor costs and improve efficiency.

### Model Selection Summary

| Factor | What to Evaluate |
|---|---|
| Model type | Whether the model supports the required task |
| Performance | Accuracy, reliability, quality, and speed |
| Constraints | Compute, data availability, and deployment environment |
| Capabilities | Text, images, multimodal tasks, and customization |
| Compliance | Fairness, privacy, security, and regulatory requirements |
| Cost | Model usage, deployment, maintenance, and infrastructure |

## 5. Business Metrics for Generative AI

Organizations evaluate generative AI applications by measuring their performance, effectiveness, business impact, and return on investment (ROI).

Business metrics help organizations understand whether an AI initiative meets its objectives and identify areas for improvement.

The appropriate metrics depend on the business problem and the application's intended outcomes.

### 5.1 User Satisfaction

User satisfaction measures user feedback regarding AI-generated content or recommendations.

**Use case:** An e-commerce company monitors user satisfaction to improve customer loyalty, repeat purchases, and positive word-of-mouth.

### 5.2 Average Revenue per User (ARPU)

ARPU calculates the average revenue generated per user or customer attributed to the application.

**Use case:** Marketing and product teams analyze how effectively an e-commerce platform monetizes its users and identify opportunities for improvement.

### 5.3 Cross-Domain Performance

Cross-domain performance measures how effectively a generative AI model performs across different domains or industries.

**Use case:** An e-commerce platform operates across different product categories and geographic regions and monitors performance across these domains.

### 5.4 Conversion Rate

Conversion rate measures the percentage of users who complete a desired action, such as making a purchase, signing up, or engaging with content.

**Use case:** An online clothing store monitors the percentage of visitors who become paying customers.

### 5.5 Efficiency

Efficiency evaluates resource utilization, computation time, and scalability.

**Use case:** A manufacturing company monitors production-line efficiency to reduce costs and increase productivity.

### Business Metrics Summary

| Metric | Purpose | Example |
|---|---|---|
| User satisfaction | Measures user experience | Feedback on AI-generated recommendations |
| ARPU | Measures average revenue per user | Revenue generated per e-commerce customer |
| Cross-domain performance | Measures performance across different domains | Model performance across product categories |
| Conversion rate | Measures desired user actions | Percentage of visitors making purchases |
| Efficiency | Measures resource use and productivity | Manufacturing output relative to resources used |

## 6. Course Summary

This course covers AI use cases, machine learning techniques, generative AI capabilities and challenges, model selection, and business metrics.

Key takeaways:

- AI supports tasks requiring perception, reasoning, learning, and decision-making.
- ML is useful when rules are difficult to define or data must be processed at scale.
- Supervised learning uses labeled data, unsupervised learning discovers patterns, and reinforcement learning learns through rewards and penalties.
- Generative AI creates new content but introduces risks such as hallucinations, toxicity, privacy violations, and inconsistent outputs.
- Model selection requires evaluating model types, performance, capabilities, constraints, compliance, and cost.
- Business metrics such as user satisfaction, ARPU, cross-domain performance, conversion rate, and efficiency help measure business value.
