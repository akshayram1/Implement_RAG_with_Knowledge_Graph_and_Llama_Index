# Implementing RAG (Retrieval-Augmented Generation) with Knowledge Graph and Llama-Index

This project demonstrates how to implement a Retrieval-Augmented Generation (RAG) system that incorporates a Knowledge Graph and Llama-Index to perform multi-document question answering. The application allows users to query a knowledge base derived from multiple documents, leveraging a knowledge graph for enriched contextual understanding and Llama-Index for document indexing and retrieval.

## Project Structure

```
.
├── documents/                  # Folder containing the input documents for knowledge extraction              
├── Knowledge_graph.html        # Visualization of the generated Knowledge Graph
├── graph.html                  # Alternative visualization of the Knowledge Graph
├── requirements.txt            # Python dependencies for the project
└── Implement_RAG_(multidoc)with_Knowledge_Graph_and_Llama_Index.ipynb  # Main implementation notebook
```

## Features

1. **Multi-Document Input**: Supports querying across multiple documents.
2. **Knowledge Graph Integration**: Constructs and visualizes a knowledge graph from the input documents to enhance contextual understanding.
3. **Llama-Index Integration**: Utilizes Llama-Index for efficient document indexing and retrieval.
4. **RAG Pipeline**: Combines retrieval and generation for answering user queries.
5. **Interactive Visualizations**: Knowledge Graphs are rendered in `Knowledge_graph.html` and `graph.html` for interactive exploration.
6. **Output Demonstration**: A GIF demonstrating the output is available [here](Implement-RAG-multidoc-with-Knowledge-Graph-and-Llama-Index-ipynb---Colab-ezgif.com-video-to-gif-converter.gif).

## Prerequisites

- Python 3.8+
- Jupyter Notebook or a similar environment

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Prepare Documents**:
   - Place your input documents (e.g., `.txt`, `.pdf`) in the `documents/` folder.

2. **Run the Notebook**:
   - Open the `Implement_RAG_(multidoc)with_Knowledge_Graph_and_Llama_Index.ipynb` notebook in Jupyter.
   - Execute the cells step-by-step to:
     - Parse and process the input documents.
     - Generate the Knowledge Graph.
     - Index the documents using Llama-Index.
     - Query the RAG system.

3. **Visualize the Knowledge Graph**:
   - After running the notebook, open `Knowledge_graph.html` or `graph.html` in a web browser to interact with the graph.

## Key Components

### Knowledge Graph
A graph-based representation of entities and their relationships extracted from the input documents. This graph enhances query understanding by providing a structured view of the knowledge base.

### Llama-Index
An indexing framework that organizes documents for efficient retrieval. It is integrated into the RAG pipeline to fetch relevant context for answering user queries.

### RAG Pipeline
A combination of retrieval (using Llama-Index) and generation (using an LLM) to produce accurate and contextually relevant answers.

## Example Workflow

1. **Input Documents**:
   - Add documents to the `documents/` folder.
2. **Generate Knowledge Graph**:
   - Parse the documents and extract entities and relationships.
3. **Index Documents**:
   - Use Llama-Index to create an index for the documents.
4. **Query the System**:
   - Enter a question in the notebook interface to retrieve and generate answers.

## Dependencies

The required dependencies are listed in `requirements.txt`. Major libraries include:

- `networkx`: For creating and visualizing the Knowledge Graph
- `llama-index`: For indexing and retrieval
- `openai` or other LLM APIs: For generating answers
- `matplotlib`, `pandas`: For data processing and visualization
- `jupyter`: To run the notebook

## Limitations

- The system's performance heavily depends on the quality of the input documents and the LLM used for generation.
- Visualizations might not scale well for very large Knowledge Graphs.

## Future Enhancements

- Add support for more complex queries and entity linking.
- Improve the scalability of the Knowledge Graph visualization.
- Integrate a real-time query interface for end-users.

## References

- [Llama-Index Documentation](https://github.com/jerryjliu/llama_index)


