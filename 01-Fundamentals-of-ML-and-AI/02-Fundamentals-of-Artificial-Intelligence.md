
# Fundamentals of Artificial Intelligence

# 1. Machine Learning Fundamentals

## 1.1 What Is Machine Learning?

Machine Learning (ML) is a type of Artificial Intelligence that enables computers to learn patterns from data and improve their performance on specific tasks.

Instead of explicitly programming every rule, developers train ML algorithms using data. The trained model can then use what it has learned to make predictions or decisions on new data.

## 1.2 Machine Learning Model Development Process

Building a machine learning model involves several stages:

1. Data collection and preparation
2. Algorithm selection
3. Model training
4. Model evaluation and testing
5. Iteration and improvement
6. Inferencing using the trained model

The process may be repeated to improve model performance.

### Importance of Training Data

The ML process starts with collecting and processing training data.

The quality of an ML model depends heavily on the quality of the data used to train it.

**Garbage in, garbage out:** Poor-quality, incorrect, incomplete, or unsuitable data can lead to poor model performance.

Data preparation is one of the most critical stages of ML development because it can significantly affect the model's ability to learn useful patterns.

## 1.3 Types of Training Data

### A. Labeled Data

Labeled data is a dataset in which each instance or example is associated with a label or target variable representing the desired output.

Labels may be provided by human experts or obtained through a reliable process.

**Example:** An image dataset containing images labeled as cat, dog, or car.

Labeled data is commonly used in supervised learning.

### B. Unlabeled Data

Unlabeled data consists of examples without associated labels or target variables.

The dataset contains input features but does not provide the desired output for each example.

**Example:** A collection of images without labels or annotations.

Unlabeled data is commonly used in unsupervised learning and self-supervised pre-training.

### Labeled vs. Unlabeled Data

| Feature | Labeled Data | Unlabeled Data |
|---|---|---|
| Labels | Present | Absent |
| Desired output | Provided for each example | Not provided |
| Common use | Supervised learning | Unsupervised learning |
| Example | Images labeled cat or dog | Images without labels |

## 1.4 Types of Data

Training data can be broadly classified into structured and unstructured data.

### A. Structured Data

Structured data is organised and formatted according to a predefined structure, typically using rows and columns.

It is commonly stored in spreadsheets, databases, and tabular files.

**Types of structured data:**

**1. Tabular Data**
- Organised into rows and columns.
- Rows represent individual records or instances.
- Columns represent features or attributes.
- Examples include spreadsheets, CSV files, and database tables.

**2. Time-Series Data**
- Consists of values measured at successive points in time.
- Examples include stock prices, sensor readings, and weather measurements.

### B. Unstructured Data

Unstructured data does not follow a predefined tabular format.

It often requires specialised techniques to extract meaningful information.

Examples include:

- **Text data:** Documents, articles, and social media posts.
- **Image data:** Photographs, digital images, and video frames.
- **Audio data:** Speech recordings and sound files.
- **Video data:** Recorded video content.

### Structured vs. Unstructured Data

| Feature | Structured Data | Unstructured Data |
|---|---|---|
| Organisation | Predefined format | No fixed tabular structure |
| Typical representation | Rows and columns | Text, images, audio, video |
| Examples | CSV files and databases | Photographs and documents |
| Processing | Often suitable for traditional tabular ML | May require specialised processing techniques |

## 1.5 Types of Machine Learning

The three main categories of machine learning introduced in the course are supervised learning, unsupervised learning, and reinforcement learning.

### A. Supervised Learning

Supervised learning trains algorithms using labeled data.

The objective is to learn a mapping between input features and known outputs so the model can predict outputs for new, unseen inputs.

**Example:** Training a model using historical property data with known prices to predict the prices of new properties.

**Key points:**
- Uses labeled data.
- Learns from known input-output examples.
- Commonly used for prediction and classification tasks.

### B. Unsupervised Learning

Unsupervised learning uses unlabeled data.

The objective is to discover patterns, structures, or relationships within the data without predefined target labels.

**Example:** Grouping customers according to their purchasing behaviour.

**Key points:**
- Uses unlabeled data.
- Identifies hidden patterns or structures.
- Does not require predefined output labels.

### C. Reinforcement Learning

Reinforcement learning is an ML technique in which an agent learns through interaction and feedback.

The agent receives rewards or penalties for its actions and learns to improve its decisions over time.

The objective is to maximise cumulative reward or achieve a longer-term goal.

**Example:** A simulated racing car learning which actions help it complete a track effectively.

**Key points:**
- Learns through interaction.
- Receives rewards or penalties.
- Improves decision-making over time.
- Does not rely on labeled examples in the same way as supervised learning.

### D. Semi-Supervised Learning

Semi-supervised learning uses a combination of labeled and unlabeled data.

Only a portion of the training examples have labels, while the remaining examples are unlabeled.

### Comparison of Learning Types

| Feature | Supervised Learning | Unsupervised Learning | Reinforcement Learning | Semi-Supervised Learning |
|---|---|---|---|---|
| Learning signal | Labeled examples | Patterns in data | Rewards and penalties | Labeled and unlabeled examples |
| Main objective | Predict outputs | Discover structure | Learn effective actions | Learn with limited labels |
| Example | Spam classification | Customer clustering | Autonomous racing | Image classification with limited labels |

## 1.6 Training and Inferencing

### Training

Training is the process through which an ML algorithm learns patterns and relationships from training data.

During training, model parameters are adjusted to improve performance on the learning task.

### Inferencing

Inferencing is the process of using a trained model to make predictions or decisions on input data.

After training, the model can process new inputs and generate outputs.

**Example:**
- Training: A model learns from historical customer purchasing data.
- Inferencing: The trained model predicts whether a new customer may purchase a product.

### Types of Inferencing

#### A. Batch Inferencing

Batch inferencing processes a large amount of data together and produces a set of results.

Characteristics:
- Processes data in batches.
- Suitable when an immediate response is not essential.
- Useful for large-scale data analysis and processing.

**Example:** Analysing a large collection of images overnight.

#### B. Real-Time Inferencing

Real-time inferencing processes new inputs and produces responses quickly as they arrive.

Characteristics:
- Responds to incoming data with low latency.
- Suitable for applications requiring immediate decisions.
- Processes inputs as they become available.

**Example:** A chatbot responding to a user query.

### Batch vs. Real-Time Inferencing

| Feature | Batch Inferencing | Real-Time Inferencing |
|---|---|---|
| Processing | Large groups of data | Incoming inputs as they arrive |
| Response | Results produced for a batch | Rapid response to each input |
| Latency requirement | Immediate response usually unnecessary | Low latency is important |
| Example | Overnight document analysis | Interactive chatbot |

---

# 2. Deep Learning Fundamentals

## 2.1 What Is Deep Learning?

Deep Learning (DL) is a branch of machine learning inspired by the structure and function of the human brain.

It uses artificial neural networks, which are computational models designed to learn patterns from data through interconnected processing units.

Deep learning is particularly useful for learning complex patterns from large amounts of data.

## 2.2 Artificial Neural Networks

Neural networks form the foundation of deep learning.

They consist of interconnected units called nodes or artificial neurons. These nodes are arranged in layers.

### A. Input Layer

The input layer receives the input features provided to the network.

For example, in a customer prediction model, the input features might include age, purchase history, and browsing activity.

### B. Hidden Layers

Hidden layers process information received from earlier layers.

They learn useful patterns and representations from the input data.

A network may contain one or more hidden layers. Deep neural networks generally contain multiple hidden layers.

### C. Output Layer

The output layer produces the final result of the neural network.

Depending on the task, the output may be a class, a numerical prediction, or another result.

### Connections and Weights

Nodes are connected through weighted connections.

During training, the network adjusts its weights to learn patterns that improve its predictions.

After training, the network can apply the learned patterns to previously unseen inputs.

## 2.3 Applications of Deep Learning

### A. Computer Vision

Computer vision is a field of AI that enables computers to interpret and understand digital images and videos.

Deep learning supports several computer vision tasks:

1. **Image Classification:** Assigning a category to an image.
2. **Object Detection:** Identifying objects and their locations in an image.
3. **Image Segmentation:** Identifying regions or pixels belonging to particular objects or classes.

**AWS example:** Amazon Rekognition provides image and video analysis capabilities.

### B. Natural Language Processing (NLP)

Natural Language Processing is a branch of AI concerned with interactions between computers and human languages.

Deep learning supports tasks such as:
- Text classification
- Sentiment analysis
- Machine translation
- Language generation

**Example:** Analysing customer reviews to identify whether the expressed sentiment is positive or negative.

### Computer Vision vs. NLP

| Feature | Computer Vision | NLP |
|---|---|---|
| Primary data | Images and videos | Human language |
| Main purpose | Interpret visual information | Process and understand language |
| Example tasks | Image classification and object detection | Sentiment analysis and translation |

---

# 3. Generative AI Fundamentals

## 3.1 What Is Generative AI?

Generative AI is a field of AI focused on generating new content based on patterns learned from existing data.

It can produce text, images, audio, code, and other forms of content.

The course highlights large-scale investment in computing resources, specialised teams, and model development as contributors to the rapid emergence of generative AI.

## 3.2 Foundation Models

Foundation Models (FMs) are models pre-trained on large, diverse datasets that can serve as a starting point for many downstream tasks.

Rather than training a separate model from scratch for every task, a single foundation model can be adapted for multiple applications.

Examples of tasks include:
- Text generation
- Text summarisation
- Information extraction
- Image generation
- Chatbot interactions
- Question answering

Foundation models can also be adapted to specialised tasks or domains.

## 3.3 Foundation Model Lifecycle

The foundation model lifecycle involves several stages, from selecting training data to deploying and improving the model.

### A. Data Selection

Foundation models require large datasets from diverse sources.

Unlabeled data can be used at scale because it is often easier to obtain than manually labeled data.

Examples include raw text files, images, and videos without informative labels.

### B. Pre-Training

Pre-training allows a foundation model to learn general patterns and relationships from large datasets.

Foundation models are typically pre-trained through **self-supervised learning**.

Self-supervised learning uses the structure of the data to generate training targets automatically, reducing the need for manually labeled examples.

For example, a language model can learn relationships between words and how their meanings depend on context.

**Continuous pre-training** involves further pre-training a model on additional data to expand its knowledge and improve its ability to generalise across domains or tasks.

### C. Optimisation

Optimisation improves the usefulness of a pre-trained foundation model for a specific task.

Techniques include:
- Prompt engineering
- Retrieval-augmented generation (RAG)
- Fine-tuning

These techniques differ in their complexity, cost, and effect on model weights.

### D. Evaluation

Evaluation measures whether a model meets the desired performance criteria.

It can involve:
- Appropriate evaluation metrics
- Benchmarks
- Task-specific performance requirements
- Business requirements

A model should be evaluated before deployment to determine whether it is suitable for its intended purpose.

### E. Deployment

Deployment involves integrating the model into a production environment.

This may include integrating it into:
- Applications
- APIs
- Software systems

### F. Feedback and Continuous Improvement

After deployment, model performance is monitored and feedback is collected from users, domain experts, and other stakeholders.

Feedback and monitoring can help identify:
- Performance problems
- Potential biases
- Data or model drift
- Areas requiring improvement

The model may then be further optimised, continuously pre-trained, or retrained when needed.

**Important:** The foundation model lifecycle is iterative. Feedback from one stage can influence later stages.

## 3.4 Large Language Models (LLMs)

Large Language Models are foundation models designed to understand and generate human-like text.

Modern LLMs commonly use the transformer architecture.

They are trained on large text datasets and learn patterns and relationships between words and phrases.

Applications include:
- Answering questions
- Summarising information
- Generating content
- Assisting with programming
- Conversational interactions

## 3.5 Tokens

Tokens are the basic units of text processed by a language model.

A token may represent:
- A complete word
- Part of a word
- A punctuation mark
- Another unit of text

For example, the sentence:

"A puppy is to dog as a kitten is to cat."

may be divided into tokens such as:

"A", "puppy", "is", "to", "dog", "as", "a", "kitten", "is", "to", "cat".

The exact tokenisation depends on the tokenizer used by the model.

Tokenisation provides a standardised representation of text for processing.

## 3.6 Embeddings and Vectors

Embeddings are numerical representations of tokens or other data items.

A vector is an ordered list of numerical values.

Embeddings are learned during training and capture useful semantic relationships between items.

For example, the embeddings for "cat", "feline", and "kitten" may be close together in an embedding space because the concepts are related.

- Cat and feline have related meanings.
- Kitten refers to a young cat.
- Dog and canine have related meanings.
- Puppy refers to a young dog.
- Old and young express contrasting concepts.

### Tokens vs. Embeddings

| Feature | Tokens | Embeddings |
|---|---|---|
| Representation | Units of text | Numerical vectors |
| Main purpose | Standardise text for model processing | Represent learned semantic relationships |
| Example | The token "cat" | A vector representing the meaning and relationships of "cat" |

LLMs use tokens, embeddings, and learned relationships to generate coherent and contextually appropriate text.

## 3.7 Diffusion Models

Diffusion models are generative models that learn to generate new data by reversing a process that gradually introduces noise.

They are commonly associated with image generation.

### A. Forward Diffusion

Forward diffusion gradually introduces noise into an input image until its original structure becomes obscured.

### B. Reverse Diffusion

Reverse diffusion progressively removes noise to generate a new, coherent sample.

Diffusion models can be used for text-to-image generation and other generative tasks.

## 3.8 Multimodal Models

Multimodal models can process or generate multiple types of data, such as text, images, audio, and video.

They learn relationships between different modalities and can combine them to perform more complex tasks.

Examples:
- Answering questions about an image.
- Generating graphics from text instructions.
- Creating video captions.
- Combining text and visual information to answer questions.

## 3.9 Generative Adversarial Networks (GANs)

Generative Adversarial Networks consist of two neural networks that compete with each other during training.

### A. Generator

The generator creates synthetic data using random noise or another input.

Its objective is to generate samples that resemble the real training data.

### B. Discriminator

The discriminator receives real and generated data and attempts to distinguish between them.

Its objective is to identify whether a sample is real or generated.

### How GANs Work

1. The generator creates synthetic samples.
2. The discriminator evaluates real and generated samples.
3. The generator attempts to fool the discriminator.
4. The discriminator attempts to identify generated samples correctly.
5. The adversarial training process continues to improve generation quality.

GANs are used to generate realistic synthetic data.

## 3.10 Variational Autoencoders (VAEs)

Variational Autoencoders are generative models that combine ideas from autoencoders and variational inference.

A VAE contains two main components.

### A. Encoder

The encoder maps input data, such as an image, into a lower-dimensional latent representation.

The latent representation captures essential information about the input.

### B. Decoder

The decoder uses the latent representation to reconstruct the original input or generate new data.

### Latent Space

The latent space is encouraged to follow a probability distribution, commonly a Gaussian distribution.

New samples can be generated by sampling from the latent space and passing the samples through the decoder.

## 3.11 Comparison of Generative Models

| Model | Main Components or Process | Key Idea |
|---|---|---|
| Large Language Model | Commonly transformer-based | Understands and generates text |
| Diffusion Model | Forward and reverse diffusion | Generates samples by learning to reverse a noise process |
| Multimodal Model | Processes multiple data modalities | Combines or generates different types of data |
| GAN | Generator and discriminator | Uses adversarial training to generate realistic data |
| VAE | Encoder and decoder | Learns a probabilistic latent representation for reconstruction and generation |

---

# 4. Optimising Foundation Model Outputs

A foundation model can be optimised to improve its outputs for a particular task or application.

The three techniques covered in this course are prompt engineering, fine-tuning, and retrieval-augmented generation.

## 4.1 Prompt Engineering

Prompt engineering involves designing and refining prompts to guide a foundation model towards a desired output.

A prompt provides instructions and information that help the model understand the task.

### Elements of a Prompt

**A. Instructions**

Describe the task the model should perform.

Example: "Summarise the following article."

**B. Context**

Provides background information that helps guide the model.

Example: "You are an experienced journalist."

**C. Input Data**

Provides the information the model must process.

Example: The article to be summarised.

**D. Output Indicator**

Specifies the expected response format or type.

Example: "Write the summary in 2–3 sentences."

### Example Prompt

"You are an experienced journalist. Summarise the following text in 2–3 sentences. Text: [Long article text goes here]."

In this example:
- Instructions: Summarise the text.
- Context: Experienced journalist.
- Input data: The article.
- Output indicator: 2–3 sentences.

Prompt engineering is generally the quickest and lowest-cost optimisation option introduced in this course because it does not require additional model training.

## 4.2 Fine-Tuning

Fine-tuning involves taking a pre-trained model and training it further on a more specific dataset.

The purpose is to improve the model's performance on a particular task or domain.

Fine-tuning modifies the model's learned weights.

**Example:** Further training a general foundation model on specialised medical material to adapt its behaviour to a medical research task.

### A. Instruction Fine-Tuning

Instruction fine-tuning uses examples of how a model should respond to specific instructions.

The course identifies prompt tuning as a type of instruction fine-tuning.

### B. Reinforcement Learning from Human Feedback (RLHF)

RLHF uses human feedback to help align a model's responses with human preferences.

## 4.3 Retrieval-Augmented Generation (RAG)

Retrieval-augmented generation improves responses by retrieving relevant external information and providing it as context to a foundation model.

Instead of training the model on a small set of domain-specific examples, RAG retrieves relevant documents at answer time.

### RAG Process

1. A user submits a question.
2. The system retrieves relevant documents.
3. The retrieved information is supplied to the foundation model as context.
4. The model generates a response informed by that context.

### Advantages of RAG

- Provides relevant external information to guide responses.
- Helps incorporate domain-specific documents.
- Does not require fine-tuning the foundation model on those documents.
- Does not change the foundation model's weights.

## 4.4 Prompt Engineering vs. Fine-Tuning vs. RAG

| Feature | Prompt Engineering | Fine-Tuning | RAG |
|---|---|---|---|
| Main approach | Improve instructions | Train further on specific data | Retrieve relevant documents |
| Changes model weights? | No | Yes | No |
| Requires additional model training? | No | Yes | Not required |
| Main benefit | Guides output | Adapts model behaviour | Supplies external knowledge |
| Cost and complexity | Generally lowest | Can be higher | Depends on retrieval infrastructure |

### Selecting the Appropriate Technique

- Use **prompt engineering** when better instructions can improve the output.
- Use **fine-tuning** when additional training is needed to adapt model behaviour to a specific task.
- Use **RAG** when a model needs relevant external documents as context without changing its weights.

---

# 5. Key Revision Points

1. AI is the broad field; ML is a subset of AI.
2. Deep learning uses artificial neural networks with multiple layers.
3. Generative AI produces new content based on learned patterns.
4. Supervised learning uses labeled data.
5. Unsupervised learning discovers patterns in unlabeled data.
6. Reinforcement learning uses rewards and penalties.
7. Training teaches a model; inferencing uses the trained model.
8. Batch inferencing processes groups of data; real-time inferencing responds quickly to incoming data.
9. Foundation models are pre-trained on large datasets and can support multiple tasks.
10. Foundation models are typically pre-trained using self-supervised learning.
11. Tokens are units of text; embeddings are learned numerical representations.
12. GANs use a generator and discriminator.
13. VAEs use an encoder and decoder.
14. Prompt engineering changes instructions, not model weights.
15. Fine-tuning changes model weights through additional training.
16. RAG retrieves external information and supplies it as context without fine-tuning the model.

## Important Terms

| Term | Definition |
|---|---|
| Training Data | Data used to teach a model patterns or relationships. |
| Labeled Data | Data with associated labels or target values. |
| Unlabeled Data | Data without associated labels or target values. |
| Supervised Learning | Learning from labeled examples. |
| Unsupervised Learning | Discovering patterns in unlabeled data. |
| Reinforcement Learning | Learning through rewards and penalties. |
| Inferencing | Using a trained model to produce predictions or decisions. |
| Neural Network | A computational model consisting of interconnected nodes organised into layers. |
| Foundation Model | A broadly pre-trained model that can be adapted for multiple tasks. |
| Self-Supervised Learning | Learning using training targets generated from the structure of data. |
| Token | A basic unit of text processed by a model. |
| Embedding | A learned numerical representation of a token or data item. |
| Diffusion Model | A generative model that learns to reverse a noise process. |
| GAN | A generative model with a competing generator and discriminator. |
| VAE | A generative model with an encoder and decoder operating through a probabilistic latent space. |
| Prompt Engineering | Designing and refining prompts to guide model outputs. |
| Fine-Tuning | Further training a pre-trained model on specific data. |
| RAG | Retrieving relevant external information to provide context for a model response. |
