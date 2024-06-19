# Self-Hosted GenAI Code with RAG Features

## Why This Project Exists

As we explore AI and ML concepts, each of us embarks on a unique journey. While some achieve great success, many face challenges and setbacks. This repository is a part of my own journey through the evolving landscape of AI.

Journey began with  reading, listening, and learning. Was fascinated by the creative and operational benefits AI offers, but equally aware of the biases it can introduce. This led me to ponder:

> "Is it not a bias to call AI Artificial Intelligence? Shouldn't we consider it Assistive/Aiding Intelligence instead?"


### Initial Boost

In my context the launch of Oracle Cloud Infrastructure GenAI service provided the first major boost to this exploration:

[Oracle Cloud Infrastructure GenAI Service](https://www.oracle.com/artificial-intelligence/generative-ai/generative-ai-service/)

### Catalyst

The learning and certification program acted as a catalyst for this venture:

[Oracle Cloud Infrastructure 2024 GenAI Professional Certification](https://education.oracle.com/oracle-cloud-infrastructure-2024-generative-ai-professional/pexam_1Z0-1127-24)

### Second Boost

On May 21, 2024, the European Union approved the world's first comprehensive AI legal framework, the AI Act, which balances safety with fostering innovation. This legislation imposes strict regulations on high-risk AI applications and bans certain practices. By enhancing transparency and trust, the AI Act positions the EU as a global leader in AI regulation and may inspire similar laws worldwide.

- [EU AI Act Press Release](https://www.consilium.europa.eu/en/press/press-releases/2024/05/21/artificial-intelligence-ai-act-council-gives-final-green-light-to-the-first-worldwide-rules-on-ai/)
- [Video on the AI Act](https://www.youtube.com/watch?v=DjZptKfGTZ0)

Like earlier regulations such as GDPR and MiFID II, this act will shape the AI ecosystem significantly.

This will obviosly created ripples, and would hear often organizations saying

> "We are working on the EU AI act problem, to get into compliance", or few more would tell the problem as opportunity


## Solution to the problem is within the problem

At this stage, my learning journey gained a purpose beyond mere leaning. The positive news was clear: "Consensus leads to approval." When people are impacted, regulations help streamline activities and bring positive benefits.

As with all regulations, the AI Act comes with extensive documentation. Legal, regulatory, and security experts will form forums to disseminate crucial information within organizations. This led to my objective:

> "Ask the AI, on what AI system's Todos and Not Todos" as per the current document stored locally.

To start small, got a single Document that encapsuates this information in ![AI Act](src/pdf-docs/EPRS_BRI698792_EN.pdf) in the RAG program

The results from this grounded reality were quite impressive, opening up numerous opportunities for further exploration and development.



# AI 101

Embarking on a new journey can be daunting. It helps to have knowledge learnt long time back to give a sense of belonging and calmness while navigating the complexities. Below was my initial approach to AI, and over time, my understanding has evolved, adding new insights and refining the one that existed.

![AI 101](docs/20240312-AI-101.drawio.png)



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


# Retrieval-Augmented Generation (RAG)

RAG (Retrieval-Augmented Generation) is an advanced natural language processing (NLP) model designed to enhance text generation by incorporating relevant information from external sources. This README explains the basics of RAG, its core components, the concepts of RAG Sequence and RAG Token Types, and outlines the RAG pipeline.

## Basics of RAG

RAG improves the quality and relevance of generated responses by combining three main components:
1. **Retriever**
2. **Ranker**
3. **Generator**

## Components of RAG

### 1. Retriever
- **Function:** Searches a large corpus of documents or a knowledge base to find relevant information based on the input query.
- **Implementation:** Utilizes dense retrieval methods (like DPR) or traditional sparse retrieval methods (like BM25).

### 2. Ranker
- **Function:** Ranks the retrieved documents or passages based on their relevance to the query.
- **Purpose:** Enhances the quality of the information fed into the generator.
- **Mechanism:** Uses scoring systems or additional models to assess relevance.

### 3. Generator
- **Function:** Generates a coherent and contextually relevant response using the ranked documents or passages.
- **Implementation:** Often uses pre-trained language models such as BERT, GPT, or T5.
- **Outcome:** Ensures the final output is both informative and appropriate to the context.

## RAG Sequence and RAG Token Types

### RAG Sequence
- Describes the process where the retriever finds relevant documents, the ranker orders them, and the generator produces the final output.
- Enhances response context and accuracy by leveraging external knowledge.

### RAG Token Types
- **Input Tokens:** Initial query or prompt provided to the model.
- **Retrieved Document Tokens:** Tokens from documents retrieved by the retriever.
- **Generated Response Tokens:** Tokens in the final output generated by the model.

## RAG Pipeline: Ingestion, Retrieval, and Generation

### 1. Ingestion
- **Purpose:** Prepares and indexes a large corpus of documents for efficient retrieval.
- **Techniques:** Includes tokenization, embedding creation, and storage of embeddings.

### 2. Retrieval
- **Function:** The retriever searches the indexed corpus for relevant documents based on the input query.
- **Techniques:** Can involve dense retrieval (using neural networks) or sparse retrieval (using inverted indexes).

### 3. Generation
- **Function:** The generator takes the top-ranked documents from the retriever to produce a response.
- **Outcome:** Ensures the response is coherent, contextually appropriate, and informative.
- **Balance:** Utilizes retrieved information while generating new content based on the model’s training.


