# Self-Hosted GenAI Code with RAG Features

## AI 101

Embarking on a new topic can be daunting. It helps to have some foundational knowledge or pointers to give a sense of belonging and calmness while navigating the complexities. This was my initial approach to AI, and over time, my understanding has evolved, adding new insights and refining the sequence of concepts.

![AI 101](docs/20240312-AI-101.drawio.png)


## Fundamentals

# Large Language Models (LLMs)

## Key Points

- **Processing Text with LLMs**:
  - LLMs use encoders and decoders to convert words into numerical vectors.
  - They capture the semantics of text and generate text token by token.

- **Architectures and Tasks**:
  - LLM architectures include encoder, decoder, and encoder-decoder models.
  - These architectures are suited to various tasks such as translation, summarization, and question-answering.

- **Prompting Techniques**:
  - Techniques like in-context learning and chain-of-thought prompting are used to improve LLM performance.
  - Prompting can introduce issues like prompt injection.

- **Hardware Requirements**:
  - LLMs require substantial hardware resources for training and inference.
  - Advanced models like GPT-4 need high-performance GPUs.

- **Applications**:
  - Code models (e.g., Copilot, Codex) and multi-modal models handle text, image, and audio data.
  - Language agents can reason, plan, and take actions, such as those in ReAct and Toolformer.


![Fundamentals Diagram](docs/20240312-AI-Fundementals.drawio.png)

## Gen AI Services

# Generative AI Services

## Key Points

- **Pre-trained Foundational Models**:
  - Used for text generation, summarization, and embedding.
  - Models like Cohere and Llama are commonly used.

- **Generation and Embedding Services**:
  - Generate vectors for words and sentences to determine semantic similarity.
  - Utilize models for various applications, including semantic similarity.

- **Prompt Engineering**:
  - Essential for refining AI outputs.
  - Techniques like in-context learning and K-shot prompting enhance performance.

- **Customization with User Data**:
  - Involves prompt engineering, retrieval-augmented generation (RAG), and fine-tuning.
  - Allows for tailored AI solutions.

- **Inference Services**:
  - Facilitate deployment of customized models.
  - Provide tailored responses based on specific prompts and data.


![Gen AI Services Diagram](docs/20240312-AI-Generative-AI-Service.drawio.png)

## Retrieval-Augmented Generation (RAG)

Retrieval-Augmented Generation (RAG) is a cutting-edge technique that combines retrieval-based methods with generative models to produce more accurate and contextually relevant outputs. It leverages a database of information to enhance the generative capabilities of AI, leading to better performance in tasks such as question answering and content generation.

![RAG Diagram](docs/20240312-AI-RAG.drawio.png)
