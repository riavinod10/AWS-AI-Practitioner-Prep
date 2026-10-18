
# AWS Infrastructure and Technologies

## 1. Introduction to AWS AI/ML Services

Amazon Web Services (AWS) offers a wide range of services that help developers and organisations build, train, deploy, and integrate AI and ML capabilities into applications.

These services include:
- Tools for building custom machine learning models.
- Ready-to-use AI services for text, documents, speech, vision, search, and recommendations.
- Services for accessing and using foundation models.
- Generative AI assistants and developer tools.

The appropriate service depends on the application's requirements, the desired level of customisation, the available infrastructure, and the cost.

---

## 2. AWS AI/ML Services Stack

AWS groups its AI and ML capabilities into three broad layers.

### 2.1 ML Frameworks Layer

This layer provides tools and infrastructure for developing and deploying machine learning models.

#### Amazon SageMaker AI

Amazon SageMaker AI is a fully managed service that enables developers to build, train, and deploy ML models.

Key capabilities:
- Provides managed infrastructure for ML development.
- Supports model building, training, and deployment.
- Provides tools and workflows for the ML lifecycle.
- Helps reduce the effort involved in managing ML infrastructure.
- Supports development and deployment of models, including large language models and other foundation models.

**Example:** A developer can use SageMaker AI to train and deploy a custom model that predicts customer demand.

**Remember:** SageMaker AI is primarily associated with building, training, and deploying custom ML models.

### 2.2 AI/ML Services Layer

This layer provides specialised, ready-to-use AI capabilities for specific tasks.

The services include:
- Natural language processing
- Language translation
- Document text extraction
- Conversational interfaces
- Speech synthesis and recognition
- Image and video analysis
- Intelligent search
- Personalised recommendations
- Reinforcement learning education and experimentation

These services allow developers to incorporate AI capabilities into applications without necessarily building every underlying model from scratch.

### 2.3 Generative AI Layer

This layer provides services and tools for working with foundation models and building generative AI applications.

Important services include:
- Amazon SageMaker JumpStart
- Amazon Bedrock
- Amazon Q
- Amazon Q Developer
- PartyRock

---

## 3. AWS AI/ML Services

### 3.1 Amazon Comprehend

**Purpose:** Natural language processing and text analysis.

Amazon Comprehend uses ML and NLP to identify insights and relationships in unstructured text.

Capabilities:
- Identifies the language of a text.
- Extracts key phrases.
- Identifies entities such as people, places, brands, and events.
- Analyses sentiment to determine whether text expresses positive or negative sentiment.
- Analyses text using tokenisation and parts of speech.
- Organises collections of text by topic.

**Example:** A company can analyse customer reviews to identify sentiment and recurring themes.

**Exam keyword:** Text analysis, sentiment analysis, key phrases, and entity extraction.

### 3.2 Amazon Translate

**Purpose:** Neural machine translation.

Amazon Translate converts text from one language to another using deep learning-based translation technology.

Applications:
- Translating website and application content.
- Localising content for different audiences.
- Translating large volumes of text for analysis.
- Supporting communication between users speaking different languages.

Neural machine translation can produce more natural translations than traditional rule-based and statistical translation approaches.

**Example:** Translating a website into several languages for international users.

**Exam keyword:** Language translation.

### 3.3 Amazon Textract

**Purpose:** Extracting text and structured information from documents.

Amazon Textract automatically extracts text and data from scanned documents.

It goes beyond basic optical character recognition (OCR) by identifying:
- Text in scanned documents.
- Fields in forms.
- Information stored in tables.

**Example:** Extracting invoice numbers, amounts, and table entries from scanned invoices.

**Exam keyword:** Document processing, OCR, forms, and tables.

### 3.4 Amazon Lex

**Purpose:** Building conversational interfaces.

Amazon Lex is a fully managed AI service used to design, build, test, and deploy conversational interfaces using text and voice.

It supports:
- Automatic speech recognition (ASR), which converts speech into text.
- Natural language understanding (NLU), which helps identify the intent of a user's message.
- Conversational bots.
- Voice-enabled interactive voice response (IVR) systems.

Amazon Lex makes conversational technologies similar to those used by Amazon Alexa available to developers.

**Example:** Building a customer-support chatbot that understands user requests.

**Exam keyword:** Chatbots, conversational interfaces, and user intent.

### 3.5 Amazon Polly

**Purpose:** Text-to-speech conversion.

Amazon Polly converts text into lifelike speech using deep learning technologies.

Capabilities:
- Produces synthetic speech from text.
- Provides voices across multiple languages.
- Supports speech-enabled applications.

Applications:
- Virtual assistants.
- Audiobooks.
- Spoken content.
- Applications that read text aloud.

**Example:** Converting a written article into spoken audio.

**Exam keyword:** Text to speech (TTS).

### 3.6 Amazon Transcribe

**Purpose:** Automatic speech recognition (ASR).

Amazon Transcribe converts speech into text.

Capabilities:
- Transcribes stored audio files.
- Supports common audio formats such as WAV and MP3.
- Can provide timestamps for words.
- Supports real-time transcription of live audio streams.

Applications:
- Transcribing customer service calls.
- Generating subtitles.
- Analysing audio and video content using text.

**Example:** Converting a recorded customer-support call into searchable text.

**Exam keyword:** Speech to text.

### 3.7 Amazon Rekognition

**Purpose:** Image and video analysis.

Amazon Rekognition uses deep learning to analyse images and videos.

Capabilities include:
- Identifying objects.
- Detecting people and text.
- Recognising scenes and activities.
- Detecting inappropriate content.
- Performing facial analysis and facial comparison.

Applications:
- Image and video analysis.
- People counting.
- User verification.
- Content moderation.
- Public safety use cases.

**Example:** Analysing images to identify objects or detecting inappropriate visual content.

**Exam keyword:** Computer vision, image analysis, and video analysis.

### 3.8 Amazon Kendra

**Purpose:** Intelligent enterprise search.

Amazon Kendra uses ML to help users find information across organisational content repositories.

Applications:
- Searching internal company documents.
- Helping employees find organisational information.
- Enabling intelligent search in websites and applications.

**Example:** An employee searches a company's internal knowledge base to find a policy document.

**Exam keyword:** Intelligent enterprise search.

### 3.9 Amazon Personalize

**Purpose:** Personalised recommendations.

Amazon Personalize enables developers to build recommendation systems tailored to individual users.

Input data can include:
- Application activity, such as page views, sign-ups, and purchases.
- Items to recommend, such as articles, products, videos, and music.
- Optional demographic information, such as age or geographic location.

The service analyses the data, identifies useful patterns, and trains and optimises a personalised recommendation model.

**Example:** A shopping application recommends products based on a user's previous activity.

**Exam keyword:** Recommendation systems and personalisation.

### 3.10 AWS DeepRacer

**Purpose:** Hands-on experience with reinforcement learning.

AWS DeepRacer is a 1/18th-scale autonomous racing car designed to help users learn reinforcement learning.

Reinforcement learning trains an agent through rewards and penalties rather than relying on labeled training examples in the same way as supervised learning.

It helps users explore how an agent can learn complex behaviours and optimise decisions towards longer-term goals.

**Example:** Training a racing agent to complete a track effectively.

**Exam keyword:** Reinforcement learning.

---

## 4. AWS AI/ML Services Comparison

| Service | Primary Function | Example Use Case |
|---|---|---|
| Amazon SageMaker AI | Build, train, and deploy ML models | Custom prediction model |
| Amazon Comprehend | Analyse text and extract insights | Sentiment analysis |
| Amazon Translate | Translate languages | Multilingual website |
| Amazon Textract | Extract text and structured data from documents | Invoice processing |
| Amazon Lex | Build conversational interfaces | Chatbot |
| Amazon Polly | Convert text into speech | Spoken articles |
| Amazon Transcribe | Convert speech into text | Call transcription |
| Amazon Rekognition | Analyse images and videos | Object detection |
| Amazon Kendra | Intelligent search | Internal knowledge search |
| Amazon Personalize | Generate personalised recommendations | Product recommendations |
| AWS DeepRacer | Learn reinforcement learning | Autonomous racing |

### 4.1 Frequently Confused Services

#### Amazon Polly vs. Amazon Transcribe

- **Polly:** Text to speech.
- **Transcribe:** Speech to text.

#### Amazon Comprehend vs. Amazon Translate

- **Comprehend:** Extracts information and insights from text.
- **Translate:** Converts text from one language to another.

#### Amazon Textract vs. Amazon Rekognition

- **Textract:** Extracts text, form fields, and tables from documents.
- **Rekognition:** Analyses images and videos for objects, people, scenes, and activities.

#### Amazon Lex vs. Amazon Polly

- **Lex:** Builds conversational interfaces and recognises user intent.
- **Polly:** Generates spoken audio from text.

#### Amazon Kendra vs. Amazon Personalize

- **Kendra:** Helps users find relevant information.
- **Personalize:** Recommends items based on user activity and other available data.

---

## 5. Generative AI Services on AWS

### 5.1 Amazon SageMaker JumpStart

Amazon SageMaker JumpStart helps users get started with machine learning through pre-built solutions and supported models.

Capabilities include:
- Providing solutions for common ML use cases.
- Accelerating model development.
- Supporting customisation of solutions.
- Supporting deployment and fine-tuning of supported models.

The course describes JumpStart as providing access to more than 150 popular open-source models, including models for NLP, object detection, and image classification.

**Example:** A developer uses a supported pre-built model to accelerate the development of an image-classification application.

**Remember:** JumpStart accelerates ML development through ready-made solutions and supported models.

### 5.2 Amazon Bedrock

Amazon Bedrock is a fully managed service that provides access to foundation models from Amazon and other leading AI providers through an API.

The course mentions providers such as:
- Amazon
- Anthropic
- AI21 Labs
- Cohere
- Meta
- Mistral AI
- Stability AI

Capabilities include:
- Accessing different foundation models.
- Experimenting with models.
- Customising models with organisational data using supported methods.
- Integrating foundation models into AWS applications.
- Deploying generative AI solutions.

**Example:** A company develops a generative AI application that uses a foundation model through the Bedrock API.

**Exam keyword:** Managed access to foundation models through an API.

### 5.3 Amazon Q

Amazon Q is a generative AI-powered assistant designed to help users with work-related tasks.

It can help users:
- Find relevant information.
- Answer questions.
- Solve problems.
- Generate content.
- Work with information available in organisational repositories and enterprise systems.

**Example:** An employee uses an AI assistant to find information in internal company resources.

### 5.4 Amazon Q Developer

Amazon Q Developer is a generative AI-powered assistant designed to improve developer productivity.

It provides code recommendations and generation capabilities.

It can help developers:
- Generate code.
- Complete code snippets.
- Generate functions and logical blocks.
- Accelerate development in supported programming languages and development environments.

The course mentions languages including C#, Java, JavaScript, Python, and TypeScript.

**Example:** A developer uses an IDE assistant to generate a function based on a natural-language description.

### 5.5 PartyRock

PartyRock is an Amazon Bedrock Playground that allows users to experiment with generative AI and build AI-powered applications.

It provides a way to gain hands-on experience with generative AI applications.

### 5.6 Comparison of Generative AI Services

| Service | Primary Purpose | Best Fit |
|---|---|---|
| Amazon SageMaker AI | Build, train, and deploy ML models | Custom ML workflows |
| Amazon SageMaker JumpStart | Accelerate model development using pre-built solutions | Getting started with supported models |
| Amazon Bedrock | Access foundation models through an API | Building generative AI applications |
| Amazon Q | Assist with work using organisational information | General workplace assistance |
| Amazon Q Developer | Assist with coding and development | Software development |
| PartyRock | Experiment with generative AI applications | Learning and prototyping |

---

## 6. Advantages of AWS AI Solutions

### 6.1 Security and Privacy

AWS provides security features, compliance capabilities, and tools that support the development and deployment of AI applications.

Security and privacy considerations are important when processing organisational data and deploying AI systems.

### 6.2 Managed Infrastructure

Managed services reduce the effort required to provision and maintain infrastructure for supported AI workloads.

This allows developers to focus more on building applications and less on managing the underlying infrastructure.

### 6.3 Ready-to-Use AI Capabilities

Services such as Amazon Comprehend and Amazon Rekognition provide specialised AI capabilities that can be incorporated into applications.

Developers do not always need to build and train their own models for these tasks.

### 6.4 Integration with AWS Services

AWS services, SDKs, and APIs can be integrated to build end-to-end solutions.

For example, an application may combine document extraction, data storage, and a downstream ML workflow.

### 6.5 Choice of Foundation Models

Amazon Bedrock provides access to foundation models from different providers, allowing developers to select models according to application requirements.

### 6.6 Shared Responsibility Model

The AWS shared responsibility model distinguishes between responsibilities managed by AWS and responsibilities managed by the customer.

The exact responsibilities depend on the service and deployment.

Customers must understand their responsibilities for areas such as access controls, data handling, application configuration, and security settings.

---

## 7. Cost Considerations for AWS Generative AI

When selecting AWS AI and ML services, organisations must balance cost with requirements such as responsiveness, availability, redundancy, performance, throughput, and customisation.

### 7.1 Responsiveness and Availability

Responsiveness refers to how quickly a service responds to requests.

Availability refers to the ability of a service to remain accessible and operational.

Services with lower latency and stronger availability guarantees may cost more than alternatives with lower performance or availability guarantees.

**Example:** A business requiring consistently fast responses may need a more expensive deployment configuration than a business that can tolerate delays.

### 7.2 Redundancy and Regional Coverage

Redundancy involves deploying additional resources to improve availability and resilience.

AWS services can be deployed across multiple Availability Zones or Regions, depending on the service and architecture.

This can increase costs because additional resources must be provisioned and data may need to be replicated.

**Example:** A business deploying resources in multiple Regions to improve resilience may incur additional infrastructure and data-transfer costs.

### 7.3 Performance

AWS offers different compute options, including CPUs, GPUs, and specialised hardware accelerators.

Higher-performance options generally cost more but can provide significant performance improvements for suitable workloads.

**Example:** A compute-intensive ML workload may benefit from GPU acceleration, while a less demanding workload may not need it.

### 7.4 Token-Based Pricing

Many generative AI services use token-based pricing models.

A token is a unit of text or code processed by a model.

Depending on the service and pricing model, charges may depend on the number of input and output tokens processed.

Generally, processing or generating more tokens increases costs under token-based pricing.

**Example:** A workload that repeatedly processes long documents may consume more tokens than one that handles short queries.

### 7.5 Provisioned Throughput

Provisioned throughput involves reserving a defined amount of processing capacity in advance.

Higher provisioned throughput can increase costs but may provide more predictable performance for workloads with specific capacity requirements.

**Example:** An application with consistent, high-volume processing requirements may benefit from reserved capacity.

### 7.6 Custom Models

AWS supports the use of pre-trained models and, where available, the customisation or deployment of specialised models.

Training and deploying custom models may incur additional costs related to:
- Model complexity.
- Training data.
- Compute resources.
- Training duration.
- Deployment infrastructure.

**Example:** A company fine-tuning a model for a specialised task must consider the cost of additional training and deployment.

### 7.7 Cost Consideration Summary

| Factor | Potential Benefit | Cost Trade-Off |
|---|---|---|
| Lower latency | Faster responses | May require more expensive configurations |
| Higher availability | Greater service resilience | Additional resources may be required |
| Multi-Region deployment | Improved geographic resilience | Replication and infrastructure costs |
| Higher-performance compute | Faster processing for suitable workloads | Higher compute costs |
| More tokens | Supports more extensive inputs and outputs | Higher token-based charges |
| Provisioned throughput | Predictable processing capacity | Charges for reserved capacity |
| Custom models | Specialised model behaviour | Additional training and deployment costs |

### 7.8 Selecting a Cost-Effective Solution

Organisations should evaluate their workload requirements before selecting a service or deployment configuration.

Important questions include:
- How quickly must the application respond?
- What availability level is required?
- Is multi-Region redundancy necessary?
- What compute performance does the workload need?
- How many tokens will the application process?
- Would provisioned throughput be beneficial?
- Is a pre-trained model sufficient, or is customisation necessary?

The goal is to balance cost, performance, availability, and application requirements.

---

## 8. Final Revision Points

1. Amazon SageMaker AI is used to build, train, and deploy ML models.
2. Amazon SageMaker JumpStart accelerates ML development using supported models and pre-built solutions.
3. Amazon Bedrock provides managed API access to foundation models.
4. Amazon Comprehend analyses text and extracts insights.
5. Amazon Translate performs language translation.
6. Amazon Textract extracts text and structured information from documents.
7. Amazon Lex builds conversational interfaces.
8. Amazon Polly converts text into speech.
9. Amazon Transcribe converts speech into text.
10. Amazon Rekognition analyses images and videos.
11. Amazon Kendra provides intelligent enterprise search.
12. Amazon Personalize creates personalised recommendations.
13. AWS DeepRacer provides hands-on reinforcement learning experience.
14. Amazon Q assists with work-related tasks using organisational information.
15. Amazon Q Developer assists with software development and code generation.
16. PartyRock supports experimentation with generative AI applications.
17. Higher performance and availability can increase costs.
18. Multi-Region deployments may improve resilience but require additional resources.
19. Token-based pricing depends on the applicable pricing model and token usage.
20. Custom model training and deployment may incur additional costs.

## 9. Quick Service Lookup

| If the question asks for... | Consider... |
|---|---|
| Custom model training and deployment | Amazon SageMaker AI |
| Pre-built ML solutions | Amazon SageMaker JumpStart |
| Access to foundation models through an API | Amazon Bedrock |
| Text sentiment and entity analysis | Amazon Comprehend |
| Translation between languages | Amazon Translate |
| Text extraction from scanned forms and tables | Amazon Textract |
| A conversational chatbot | Amazon Lex |
| Text-to-speech | Amazon Polly |
| Speech-to-text | Amazon Transcribe |
| Image or video analysis | Amazon Rekognition |
| Enterprise information search | Amazon Kendra |
| Personalised product recommendations | Amazon Personalize |
| Reinforcement learning experimentation | AWS DeepRacer |
| Workplace AI assistant | Amazon Q |
| AI coding assistant | Amazon Q Developer |
| Generative AI prototyping playground | PartyRock |
