### **Lecture 2: Building a Vector Storage**

---

#### **Introduction**

Building a vector storage is a foundational step in creating Retrieval-Augmented Generation (RAG) pipelines. Vector storage involves converting documents into vector representations (embeddings) that capture the semantic meaning of the text. These embeddings are then stored in vector databases, enabling efficient retrieval of relevant data during inference. This lecture covers the process of ingesting documents, splitting them into meaningful chunks, generating embeddings, and storing them in vector databases.

---

#### **Ingesting Documents**

**Overview**:  
Ingesting documents involves extracting text from various formats and preparing it for further processing. The goal is to create a standardized dataset that can be used to generate embeddings.

**Supported Formats**:
- **PDF**: Commonly used for official documents; can contain both text and images.
- **JSON**: Often used for structured data; requires careful parsing to extract relevant text.
- **HTML**: Web pages that contain a mix of text, images, and scripts; text extraction can be complex due to the HTML structure.
- **Markdown**: A lightweight markup language used for formatting text; relatively easy to parse.

**Document Loaders**:
- **LangChain**: A comprehensive library that provides document loaders for various formats. It supports direct retrieval from APIs like GitHub, Reddit, and Google Drive.
- **PDFMiner**: A tool for extracting text from PDF files with support for layout analysis.
- **BeautifulSoup**: A Python library for parsing HTML and XML documents, useful for web scraping.

**Considerations**:
- **Data Quality**: Ensure that the extracted text is clean and free from noise, such as irrelevant metadata or formatting errors.
- **Consistency**: Standardize the extracted text to ensure uniformity across different document formats.

---

#### **Splitting Documents**

**Overview**:  
After ingestion, documents need to be split into smaller, semantically meaningful chunks. This process is crucial for generating accurate embeddings and improving the efficiency of the retrieval process.

**Text Splitting Techniques**:
- **Semantic Chunking**: Splitting text based on semantic boundaries, such as sentences or paragraphs, rather than arbitrary character counts. This helps preserve the context and meaning of the text.
- **Recursive Splitting**: A hierarchical approach that breaks down documents into sections, subsections, and paragraphs, maintaining the document’s structure.
- **Header-Based Splitting**: Splitting text based on headers and subheaders, useful for documents with clear sections, such as reports or articles.

**Tools and Libraries**:
- **LangChain**: Provides a variety of text splitters that can be customized for different types of documents. It supports semantic chunking and recursive splitting.
- **NLTK (Natural Language Toolkit)**: A Python library that includes tools for sentence segmentation and text tokenization.
- **spaCy**: An advanced NLP library that can be used to split text into sentences and other linguistic units.

**Considerations**:
- **Context Preservation**: Ensure that each chunk of text retains enough context to be meaningful on its own.
- **Metadata**: Attach metadata to each chunk (e.g., document title, section headers) to enhance retrieval and analysis.

---

#### **Embedding Models**

**Overview**:  
Embedding models convert text into high-dimensional vectors that capture the semantic meaning of the text. These embeddings enable more nuanced understanding and retrieval of information compared to traditional keyword-based methods.

**Popular Embedding Models**:
- **Sentence Transformers**: A popular library for generating high-quality sentence embeddings. It supports a wide range of pre-trained models and is optimized for tasks like semantic search and clustering.
- **BERT (Bidirectional Encoder Representations from Transformers)**: Generates context-aware embeddings that understand the meaning of words in their context.
- **GPT-based Embeddings**: Transformer models like GPT can be used to generate embeddings that capture the broader context and relationships between words.
- **Universal Sentence Encoder**: Optimized for generating sentence-level embeddings, making it suitable for tasks like text classification and clustering.

**Considerations**:
- **Model Size**: Larger models tend to generate more accurate embeddings but require more computational resources.
- **Task Specificity**: Choose embedding models based on the specific task, such as sentence embeddings for search or paragraph embeddings for document retrieval.
- **Training Data**: The quality and domain of the training data impact the model’s ability to generate accurate embeddings.

---

#### **Vector Databases**

**Overview**:  
Vector databases are specialized databases designed to store and retrieve high-dimensional vectors efficiently. They are essential for building scalable RAG pipelines that can quickly retrieve relevant information based on vector similarity.

**Top Vector Databases**:
- **Chroma**: Known for its high performance and ease of use. It is ideal for small to medium-scale applications and offers integration with popular machine learning frameworks.
- **Pinecone**: A scalable vector database that supports large-scale, high-throughput applications. It provides features like automatic indexing and data sharding.
- **Milvus**: An open-source vector database that is highly scalable and supports various indexing algorithms. It is suitable for both research and production environments.
- **FAISS (Facebook AI Similarity Search)**: Developed by Facebook AI Research, FAISS is optimized for fast similarity search in high-dimensional spaces.
- **Annoy (Approximate Nearest Neighbors Oh Yeah)**: Developed by Spotify, Annoy is optimized for memory efficiency and is suitable for approximate nearest neighbor search.

**Key Features**:
- **Indexing Algorithms**: Vector databases use specialized indexing algorithms (e.g., HNSW, IVF) to optimize the search and retrieval of vectors.
- **Scalability**: Consider the scalability of the vector database based on the volume of data and the expected query load.
- **Integration**: Ensure that the vector database integrates well with existing data pipelines and machine learning frameworks.

---

#### **References**

- **LangChain - Text Splitters**: [Link](https://python.langchain.com/docs/modules/data_connection/document_transformers/)
  - A guide to different text splitting techniques implemented in LangChain.
- **Sentence Transformers Library**: [Link](https://www.sbert.net/)
  - A popular library for generating sentence embeddings with pre-trained models.
- **MTEB Leaderboard**: [Link](https://huggingface.co/spaces/mteb/leaderboard)
  - A leaderboard for evaluating the performance of various embedding models.
- **The Top 5 Vector Databases by Moez Ali**: [Link](https://www.datacamp.com/blog/the-top-5-vector-databases)
  - A comparison of the best and most popular vector databases.

---

