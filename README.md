# Local RAG System Implementation

This repository contains a locally implemented RAG (Retrieve and Generate) system that leverages the book. The project includes code for generating answers based on retrieved context from the book, as well as example inputs and outputs.

## Overview

The RAG system utilizes embeddings and language models to generate answers to questions based on the content of the specified book. The code allows users to query the system and receive relevant information extracted from the book's context.

### Features

- Local implementation of a RAG system.
- Embedding model: `all-mpnet-base-v2`
- Language model: `google/gemma-2-2b-it`
- PDF of the book is included for reference.
- Excel file generated during execution for tracking queries and responses.

## Contents
- `rag.ipynb`: The main notebook containing the implementation details, code, and results.
- `book.pdf`: The PDF used as the knowledge base.
    The official link:
    https://web.stanford.edu/class/psych209/Readings/SuttonBartoIPRLBook2ndEd.pdf

- `text_chunks_and_embeddings.csv`: The Excel file generated during execution.

## Dependencies
Ensure you have the following libraries installed to run the notebook:
    ```bash
    pip install transformers torch pandas openpyxl

## Usage
    1. Clone the repository to your local machine.
    2. Open the notebook in Jupyter Notebook or 3. Jupyter Lab.
    4. Execute the cells in order to run the RAG implementation and generate results.

## Model Information
- Embedding Model: `all-mpnet-base-v2`
    - Dimensions: 768
    - Token Limit: 384
    - Note: This model is efficient, fast, and provides good accuracy for embedding tasks.
    
- LLM Model: `google/gemma-2-2b-it`
    - Note: This model is used given the available 4GB GPU VRAM Alternative models can be explored for experimentation.

## Acknowledgments
This work utilizes concepts from the book *"Reinforcement Learning: An Introduction"* by Richard S. Sutton and Andrew G. Barto, which served as a valuable reference for understanding certain foundational ideas in the context of building a local Retrieval-Augmented Generation (RAG) system. The implementation leverages embeddings and language models to enhance information retrieval and generation tasks.