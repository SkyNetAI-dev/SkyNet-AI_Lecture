### **Lecture 1: Running LLMs**

**Topics Covered:**
- Introduction to running LLMs and the challenges involved
- Overview of LLM APIs
  - Private LLM APIs (OpenAI, Google, Anthropic, Cohere)
  - Open-source LLM APIs (OpenRouter, Hugging Face, Together AI)
- Running LLMs locally
  - Hugging Face Hub and Spaces
  - LM Studio, llama.cpp, Ollama
- Introduction to prompt engineering
  - Zero-shot, Few-shot, Chain of Thought (CoT), ReAct

**Objectives:**
- Understand the challenges and solutions for running LLMs.
- Explore the landscape of LLM APIs and their deployment options.
- Learn about basic prompt engineering techniques.

---

### **Lecture 2: Building a Vector Storage**

**Topics Covered:**
- Introduction to vector storage in LLM applications
- Document ingestion and the challenges of various formats
- Tools for document loading and integration with APIs/databases
- Text splitting techniques for effective document processing
  - Semantic chunking
  - Recursive splitting

**Objectives:**
- Understand the role of document ingestion and splitting in building RAG pipelines.
- Learn about tools and techniques for effective document processing.
- Explore the importance of text splitting for generating high-quality embeddings.

---

### **Lecture 3: Retrieval-Augmented Generation (RAG)**

**Topics Covered:**
- Overview of Retrieval-Augmented Generation (RAG)
- Orchestrators and their role in RAG pipelines
  - LangChain, LlamaIndex, FastRAG
- Advanced retrieval techniques
  - Multi-query retrievers
  - HyDE (Hybrid Dense-Retriever Ensemble)
- Implementing memory systems in RAG pipelines

**Objectives:**
- Understand the concept of RAG and its importance in enhancing LLM outputs.
- Learn how to build RAG pipelines using orchestrators and retrieval techniques.
- Explore the integration of memory systems to improve LLM output relevance.

---

### **Lecture 4: Advanced Techniques in RAG Pipelines**

**Topics Covered:**
- Query construction and interaction with structured data
  - SQL, Cypher queries, and metadata queries
- Introduction to LLM agents and tools
  - Automatic tool selection and interoperability challenges
- Post-processing in RAG pipelines
  - Re-ranking, RAG-fusion, and classification

**Objectives:**
- Gain insights into advanced techniques for handling structured data and automating tool selection in RAG pipelines.
- Learn how to use LLM agents to enhance LLM capabilities.
- Explore post-processing techniques that improve LLM output relevance.

---

### **Lecture 5: Ingesting and Splitting Documents for Vector Storage**

**Topics Covered:**
- Document ingestion in LLM applications
  - Formats, challenges, and best practices
- Document loaders and API/database integration
- Text splitting techniques
  - Semantic chunking for meaningful text processing
  - Recursive splitting to maintain document structure

**Objectives:**
- Understand the role of document ingestion and splitting in RAG pipelines.
- Learn about tools and techniques for effective document processing.
- Explore the importance of semantic chunking and recursive splitting for high-quality embeddings.

---

### **Lecture 6: Embedding Models and Vector Databases**

**Topics Covered:**
- Overview of embedding models and their importance in RAG pipelines
  - Sentence Transformers, MTEB Leaderboard
- Introduction to vector databases
  - Chroma, Pinecone, Milvus, FAISS, Annoy
- Selecting the right embedding model and vector database for your application
- Best practices for implementing embedding models and vector storage

**Objectives:**
- Gain an understanding of embedding models and their role in RAG pipelines.
- Learn about different vector databases and how to select the best one for your needs.
- Explore best practices for using embedding models and vector databases effectively.

---

### **Lecture 7: Building and Optimizing RAG Pipelines**

**Topics Covered:**
- Introduction to RAG pipelines and their components
- Orchestrators: LangChain, LlamaIndex, FastRAG
- Advanced retrieval techniques
  - Multi-query retrievers
  - HyDE (Hybrid Dense-Retriever Ensemble)
- Implementing and optimizing memory systems in RAG pipelines

**Objectives:**
- Understand the concept of RAG and its significance in LLM applications.
- Learn how to build and optimize RAG pipelines using orchestrators and advanced retrieval techniques.
- Explore how to implement memory systems to improve LLM output coherence and relevance.

---

### **Lecture 8: Evaluation of RAG Systems**

**Topics Covered:**
- Importance of evaluation in RAG pipelines
- Tools and metrics for evaluating RAG systems
  - Ragas for retrieval evaluation
  - DeepEval for generation evaluation
- Context precision, recall, and answer relevance in RAG systems
- Strategies for continuous improvement of RAG pipelines

**Objectives:**
- Understand the critical role of evaluation in developing effective RAG pipelines.
- Learn about tools and metrics for evaluating both retrieval and generation stages.
- Explore strategies for using evaluation results to refine and optimize RAG systems.

---

### **Lecture 9: Programmatic Optimization of LLMs**

**Topics Covered:**
- Introduction to programmatic optimization of LLMs
- DSPy framework for programmatic control
  - Modular design and optimization techniques
- Strategies for optimizing prompts and model behaviors
- Use cases for programmatically optimized LLMs in specialized tasks

**Objectives:**
- Understand the concept of programmatic optimization of LLMs and its benefits.
- Learn how to use the DSPy framework to optimize LLMs for specific tasks.
- Explore practical use cases where programmatically optimized LLMs offer significant advantages.

---

### **Lecture 10: Inference Optimization Techniques**

**Topics Covered:**
- Importance of inference optimization in LLM applications
- Flash Attention: mechanics and benefits
- Key-Value caching strategies
  - Multi-Query Attention (MQA)
  - Grouped-Query Attention (GQA)
- Speculative decoding for faster text generation

**Objectives:**
- Understand the need for optimizing inference in LLM applications.
- Learn about advanced techniques like Flash Attention and Key-Value caching.
- Explore how speculative decoding can accelerate text generation while maintaining quality.

---

### **Lecture 11: Deploying and Securing LLMs**

**Topics Covered:**
- Deployment strategies for LLMs
  - Local deployment (LM Studio, Ollama)
  - Cloud deployment (TGI, vLLM, SkyPilot)
  - Edge deployment (MLC LLM, mnn-llm)
- Security challenges in LLM applications
  - Prompt hacking: injection, leaking, jailbreaking
  - Backdoors and training data poisoning
- Defensive measures
  - Red teaming, monitoring, and continuous evaluation

**Objectives:**
- Understand the various strategies for deploying LLMs in production environments.
- Learn about the unique security challenges associated with LLMs and how to mitigate them.
- Explore best practices for securing LLM applications against prompt hacking, backdoors, and other vulnerabilities.

---

### **Lecture 12: Securing LLMs Against Threats and Attacks**

**Topics Covered:**
- Understanding security threats in LLMs
  - Prompt injection, model inversion, adversarial attacks, data poisoning
- Defensive measures to protect LLMs
  - Input sanitization, adversarial training, secure data pipelines
- Regular audits and monitoring
  - Red teaming, continuous evaluation, automated alerts

**Objectives:**
- Understand the security threats that LLMs face and how they can be exploited.
- Learn about defensive measures to protect LLMs from these threats.
- Explore best practices for continuous monitoring and auditing to ensure long-term security.
