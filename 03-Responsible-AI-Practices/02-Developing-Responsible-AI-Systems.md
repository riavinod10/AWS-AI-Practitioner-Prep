# Developing Responsible AI Systems

## 1. Amazon Services and Tools for Responsible AI

AWS provides services and tools for foundation model evaluation, generative AI safeguards, bias detection, prediction explanations, monitoring, human review, governance, and transparency.

### 1.1 Amazon SageMaker AI

Amazon SageMaker AI is a fully managed ML service for building, training, and deploying models in a production-ready hosted environment.

Key capabilities include:

- ML workflows through integrated development environments.
- Managed storage and sharing of data.
- Managed algorithms for large datasets and distributed environments.
- Support for custom algorithms and ML frameworks.
- Flexible distributed training.
- Secure and scalable model deployment.

SageMaker AI also integrates with tools for model evaluation, bias analysis, explainability, monitoring, human review, and governance.

### 1.2 Amazon Bedrock

Amazon Bedrock is a fully managed service that provides access to foundation models from Amazon and other AI providers through a unified API.

It enables organizations to select suitable models, build generative AI applications with security and privacy capabilities, privately customize models with organizational data, and integrate them into applications without managing the underlying infrastructure directly.

### 1.3 Foundation Model Evaluation

A foundation model should be evaluated to determine whether it suits the intended use case.

**Model Evaluation on Amazon Bedrock**
- **Automatic evaluation:** uses predefined metrics such as accuracy, robustness, and toxicity.
- **Human evaluation:** supports subjective or custom criteria such as friendliness, style, and alignment with a brand voice. Reviewers may be internal employees or an AWS-managed team.

**Amazon SageMaker AI Clarify**
- Supports automatic evaluation of foundation models for metrics such as accuracy, robustness, and toxicity.
- Human reviewers can assess nuanced content that requires judgment.

### 1.4 Guardrails for Amazon Bedrock

Guardrails for Amazon Bedrock helps apply safeguards based on an application's use case and responsible AI policies.

Capabilities include:
- Filtering undesirable or harmful content.
- Detecting and redacting personally identifiable information (PII).
- Defining topics the application should avoid.
- Evaluating both user inputs and model responses.
- Monitoring interactions that violate configured policies.
- Creating different guardrail configurations for different applications.
- Integrating with Agents for Amazon Bedrock.

#### Blocking undesirable topics

Organizations can define topics that the application should avoid. Guardrails can detect and block inputs or responses involving restricted topics. For example, a banking assistant could be configured to avoid investment advice if it is outside the assistant's intended scope.

#### Filtering harmful content

Configurable content filters can help detect content in categories such as hate, insults, sexual content, and violence. These filters add another layer of protection alongside safeguards in the underlying model.

#### Redacting PII

Guardrails can detect personal information in user inputs and model responses. Depending on the use case, an application can reject inputs containing PII or redact it from outputs. For example, personal details can be redacted when summarizing customer-service conversations.

### 1.5 Bias Detection and Dataset Balancing

**SageMaker AI Clarify** helps identify potential bias in datasets and ML models. Users can specify features such as age or gender for analysis. Clarify produces a visual report describing bias metrics and measurements that can inform remediation.

**Amazon SageMaker Data Wrangler** provides data-preparation tools and balancing operators:
- **Random undersampling:** reduces examples from an overrepresented group or class.
- **Random oversampling:** increases the representation of an underrepresented group or class by sampling existing examples.
- **SMOTE (Synthetic Minority Oversampling Technique):** generates synthetic examples for an underrepresented class.

Balancing decisions should be based on the use case and careful evaluation of the data.

### 1.6 Model Prediction Explanation

SageMaker AI Clarify can identify features that contributed to a prediction for tabular, natural language processing (NLP), and computer vision models. For tabular data, it can also produce an aggregated feature-importance chart showing which features influence the model overall.

**SageMaker AI Experiments** is a capability used to create, manage, analyze, and compare ML experiments. Clarify can integrate with Experiments to support prediction explanations.

### 1.7 Monitoring and Human Review

**Amazon SageMaker Model Monitor**
- Monitors the quality of SageMaker ML models in production.
- Supports continuous monitoring of real-time endpoints or regularly running batch jobs, as well as scheduled monitoring for asynchronous batch jobs.
- Can issue alerts when model quality deviates from expected behavior, allowing teams to take corrective action.

**Amazon Augmented AI (Amazon A2I)**
- Helps developers build workflows for human review of ML predictions.
- Reduces the effort involved in building review systems and managing reviewers.
- Supports human judgment for uncertain, sensitive, or complex outputs.

### 1.8 Governance Tools

- **SageMaker Role Manager:** helps administrators define minimum permissions for users and teams.
- **SageMaker Model Cards:** records intended uses, risk ratings, training details, and other essential model information.
- **SageMaker Model Dashboard:** helps teams view and monitor model behavior in production.

These tools improve visibility and support governance across the model lifecycle.

### 1.9 AWS AI Service Cards

AWS AI Service Cards document AWS AI services and support responsible use. They cover:
1. Basic concepts about a service or its features.
2. Intended use cases and limitations.
3. Responsible AI design considerations.
4. Deployment and performance-optimization guidance.

## 2. Responsible Considerations for Selecting a Model

Model selection affects performance, user experience, deployment, costs, and business outcomes. Amazon Bedrock model evaluation and SageMaker AI Clarify can help assess accuracy, robustness, toxicity, and qualities requiring human judgment.

### 2.1 Define the Use Case Narrowly

The use case should be defined precisely rather than described only by the technology.

**Traditional AI example: face recognition**
- **Gallery retrieval:** a missing-person search may favor recall so that more potentially relevant matches are returned.
- **Celebrity recognition:** may favor precision to reduce incorrect matches.
- **Virtual proctoring:** may also prioritize precision because false matches can be disruptive.

The consequences of false positives and false negatives should determine the required balance.

**Generative AI example: online shopping**

A model that catalogs products has a different purpose from one intended to persuade customers to purchase products.

| Consideration | Product catalog | Persuade to buy |
|---|---|---|
| Target audience | Broad demographic | Narrower, defined demographic |
| Possible issues | Veracity and accuracy | Veracity, unwanted bias, toxicity, excessive or unsuitable detail |
| Possible consequences | Brand damage, lost sales, returns | Representative harm, brand damage, lost sales, returns |
| Tuning focus | Neutrality, clarity, completeness | Relevant benefits and problems for the intended group |

### 2.2 Choose Based on Performance Requirements

Important factors include:

- **Customization:** from prompt-based approaches to full retraining.
- **Model size:** amount of information learned, commonly represented by parameter count.
- **Inference options:** self-managed deployment or API access.
- **Licensing:** agreements may restrict or prohibit commercial use.
- **Context window:** how much information can fit into a prompt.
- **Latency:** time required to generate an output.

### 2.3 Evaluate Against Test Datasets

A model is not universally good or bad independently of the data used to evaluate it. Performance depends on both the model and the test dataset. A model may perform well on dataset A, better on dataset B, and worse on dataset C.

Teams should consider:
1. **Model development trajectory:** how the model changes as it is developed or updated.
2. **Dataset development trajectory:** how data changes over time.

Datasets can evolve as user behavior, environments, or data distributions change. Models should be evaluated on relevant, representative datasets over time.

### 2.4 Sustainability Considerations

Sustainability means developing and deploying AI in ways that are socially, environmentally, and economically sustainable over time.

**Energy consumption**
- **Challenge:** training large models and running them at scale can use significant energy and contribute to greenhouse-gas emissions.
- **Possible responses:** improve energy efficiency, consider renewable energy where possible, and assess the carbon footprint of AI operations.

**Resource utilization**
- **Challenge:** AI may require GPUs, TPUs, data-center infrastructure, and other resources whose manufacture and disposal have environmental impacts.
- **Possible responses:** improve resource efficiency, reuse and recycle hardware, and minimize electronic waste.

**Environmental impact assessment**
- **Challenge:** AI has direct impacts through energy and resource use and indirect impacts through the activities it enables.
- **Possible responses:** assess impacts before deployment and introduce mitigation strategies when needed.

### 2.5 Economic Considerations

Economic considerations include AI's benefits and costs and its effects on employment and the wider economy. AI can automate tasks and improve efficiency, but it can also contribute to job displacement or inequality. Concentration of data and technology among a small number of companies can raise concerns about market power.

### 2.6 Responsible Agency

Responsible agency concerns an AI system's ability to make judgments and act in ways aligned with responsible human values.

- **Value alignment:** system goals and behavior should align with responsible human values, not just maximize a numerical objective.
- **Responsible reasoning:** the system should consider principles and context in complex situations; applying ethical principles to unfamiliar situations remains challenging for current AI.
- **Appropriate autonomy:** independence should have clear boundaries and human oversight, especially in high-stakes areas.
- **Transparency and accountability:** provide enough information for people to oversee and assess the system's actions.

The course notes that sophisticated, human-level moral reasoning remains a major challenge for current AI.

## 3. Responsible Preparation for Datasets

Responsible AI requires datasets that are balanced, inclusive, diverse, relevant, and curated for the intended use case.

### 3.1 Balancing Datasets

Balanced datasets help reduce the risk that a model unfairly discriminates or develops unwanted bias. Relevant groups or data topics should have adequate representation. This is particularly important in hiring, lending, and criminal justice.

Balance does not necessarily mean identical numbers of every possible example. The data should appropriately represent the groups and conditions relevant to the task.

### 3.2 Inclusive and Diverse Data Collection

Data should reflect the range of perspectives, experiences, sources, and demographics needed for the use case.

Example: if an ML model is trained mostly on data from middle-aged people, it may be less accurate for younger or older people. Adequate representation of relevant age groups can help it perform more reliably across those groups.

Diversity matters beyond datasets about people. Data about science, geography, weather, products, and other topics should also represent the relevant range of cases. Poor representation can lead to biased outcomes, social harm, and possible legal consequences.

### 3.3 Data Curation

Data curation is the process of labeling, organizing, and preprocessing data so that it can be used effectively to train and evaluate a model. It helps make data reliable, relevant, and less likely to introduce avoidable bias.

The course highlights three activities:

- **Data preprocessing:** clean and prepare data to improve accuracy and completeness. Examples include data cleaning, normalization, and feature selection.
- **Data augmentation:** generate or obtain additional examples to improve representation of underrepresented groups or cases. New examples should remain suitable for the real use case.
- **Regular auditing:** review datasets for imbalance, bias, and quality problems, and take corrective action when needed.

### 3.4 Balance Data for the Intended Use Case

The intended application determines what data should be collected and how it should be balanced. For example, an AI system intended to analyze childhood cancer should use data appropriate to children and the relevant medical context. Unrelated adult cases may reduce relevance if included without considering their suitability.

## Key Takeaways

- SageMaker AI and Amazon Bedrock provide capabilities that support responsible AI development.
- Bedrock model evaluation and SageMaker AI Clarify help assess model quality and suitability.
- Guardrails for Amazon Bedrock can filter harmful content, restrict topics, and detect or redact PII.
- Clarify supports bias analysis and prediction explanations; Data Wrangler supports dataset balancing.
- Model Monitor supports production monitoring, while Amazon A2I enables human review.
- Model selection should consider the precise use case, performance, test datasets, sustainability, economics, responsible agency, and licensing.
- Responsible datasets should be inclusive, diverse, relevant, curated, and regularly audited.
