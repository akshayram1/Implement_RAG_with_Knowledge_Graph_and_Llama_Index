# RAG with Knowledge Graph and Llama-Index

## Overview

This project implements a Retrieval-Augmented Generation (RAG) system using a Knowledge Graph and Llama-Index. The system leverages advanced natural language processing techniques to create an intelligent document retrieval and query answering framework.

## Features

- **Knowledge Graph Construction**: Builds a knowledge graph from input documents
- **Advanced Embedding**: Uses Hugging Face embeddings for semantic understanding
- **Hybrid Query Engine**: Employs tree summarization and embedding-based retrieval
- **Visualization**: Generates an interactive knowledge graph visualization

## Prerequisites

### System Requirements
- Python 3.8+
- pip package manager

### Required Packages
- llama-index (v0.10.33)
- langchain (v0.1.16)
- pyvis
- huggingface_hub
- IPython



## Configuration

### Hugging Face API Token
- Obtain a Hugging Face API token from [Hugging Face](https://huggingface.co/)
- Replace `HF_TOKEN` in the script with your personal token

### Document Preparation
- Place your documents in the `/content/documents` directory
- Supported document formats include PDF, TXT, etc.

## Usage

### Running the Script
```python
python implement_rag_with_knowledge_graph_and_llama_index.py
```

### Customizing the Query
- Modify the `query` variable to change the search topic
- Adjust `max_triplets_per_chunk`, `similarity_top_k`, and other parameters as needed

## Key Components

### Models Used
- **Language Model**: HuggingFaceH4/zephyr-7b-beta
- **Embedding Model**: thenlper/gte-large

### Query Engine Configuration
- Response Mode: Tree Summarize
- Embedding Mode: Hybrid
- Top-K Similarity: 5 documents

## Output

The script generates:
- Console output with query response
- Formatted source references
- Interactive HTML knowledge graph visualization (`Knowledge_graph.html`)

## Visualization

The knowledge graph is saved as `Knowledge_graph.html`, which can be opened in a web browser to explore document relationships interactively.

## Customization

You can customize the script by:
- Changing embedding and language models
- Adjusting chunk sizes
- Modifying query engine parameters
- Implementing different retrieval strategies

## Limitations

- Requires a Hugging Face API token
- Performance depends on the quality and quantity of input documents
- Embedding and language model performance can vary

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

