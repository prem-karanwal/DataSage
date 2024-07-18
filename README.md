# DataSage: Natural Language Query Agent

## Introduction

DataSage is a project that implements a Natural Language Query Agent designed to answer questions based on various types of documents, including lecture notes, articles, and tables. The system leverages Large Language Models (LLMs) and vector indexing frameworks for query processing and response generation.

## Approach

### Data Collection

- **Document Sources**: Supports extraction from URLs or uploaded documents using web scraping techniques.
- **Content Types**: Handles various document formats, including text articles etc.

### Data Processing

- **Web Scraping**: Utilizes BeautifulSoup for extracting text from URLs.
- **Document Parsing**: Cleans and organizes extracted content into structured data.

### Embedding Generation

- **Embedding Model**: Utilizes Google Generative AI model (Gemini) to generate embeddings for document contents.
- **Vector Store Creation**: Implements FAISS library to store embeddings for efficient similarity searches.

### Query Handling

- **Query Embedding**: Converts incoming queries into embeddings for semantic matching.
- **Similarity Search**: Uses vector store to find relevant documents matching query embeddings.
- **Answer Generation**: Generates natural language answers using LLM based on retrieved document content.

## Areas of Improvement

1. **Conversational Memory**:
   - Implement a memory module for maintaining context across multiple queries.
   
2. **Citation of References**:
   - Enhance answer generation to include citations from source documents.
   
3. **Scalability**:
   - Develop strategies for scaling to handle larger datasets and ensure efficient performance and storage.

