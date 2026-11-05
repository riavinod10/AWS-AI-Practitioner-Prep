
# Selecting a Foundation Model (FM)

## 1. Introduction

After defining the use case, the next step is selecting an appropriate Foundation Model (FM).

A foundation model is a pretrained model that can be adapted for different tasks and applications.

Models can be selected from existing pretrained models or developed from scratch.

## 2. Pretrained Model Selection Criteria

Pretrained models provide a starting point because they already contain knowledge learned from large amounts of data.

They can be fine-tuned using task-specific data to improve performance.

The following criteria should be considered when selecting a pretrained model:

1. **Cost:** Consider licensing fees, computational resources, inference costs, and customization expenses.

2. **Modality:** Choose a model based on the required output, such as text, images, audio, or multiple formats.

3. **Latency:** Consider the time taken by the model to generate responses, especially for real-time applications.

4. **Multilingual Support:** Check whether the model supports the languages required by the application.

5. **Model Size:** Larger models generally require more computational resources but may perform better on complex tasks.

6. **Model Complexity:** Complex models can handle advanced tasks but may be difficult to deploy and optimize.

7. **Customization:** Check whether the model supports fine-tuning or adaptation for specific tasks.

8. **Input/Output Length:** Consider the maximum input and output length supported by the model.

9. **Responsibility Considerations:** Evaluate possible biases, misinformation, and misuse of the model.

10. **Deployment and Integration:** Consider deployment ease, infrastructure compatibility, and available tools and libraries.

## 3. Examples of Pretrained Models on Amazon Bedrock

Amazon Bedrock provides access to foundation models from different providers.

### 1. AI21 Labs – Jurassic-2

- Large Language Model (LLM).
- Used for text generation, question answering, summarization, and classification.
- Can use organizational data for business applications.

### 2. Amazon – Titan

- Family of pretrained foundation models developed by AWS.
- Can be used directly or customized through fine-tuning.
- Includes embedding, text generation, and image generation models.

### 3. Anthropic – Claude

- Family of text and vision AI models.
- Includes Haiku, Sonnet, and Opus.
- Offers different combinations of intelligence, speed, and cost.

### 4. Cohere – Command XL

- Generative language model for text-based responses.
- Used for summarization, copywriting, dialogue, extraction, and question answering.

### 5. Meta – Llama 3

- Family of Large Language Models.
- Based on the Transformer architecture.
- Generates coherent and contextually relevant text.

### 6. Mistral AI – Mistral Large

- Suitable for complex tasks requiring strong reasoning.
- Used for text generation, code generation, RAG, and agents.

### 7. Stability AI – Stable Diffusion

- Image generation model.
- Generates images from text prompts.

**Note:** The best model depends on the business use case, requirements, available resources, and cost constraints.
