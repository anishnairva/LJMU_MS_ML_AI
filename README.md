
## 1. Overview
This repository contains the complete experimentation code, dataset, and supporting files used in my MSc thesis.
The research analyses how different prompt-based techniques and RAG methods influence hallucination reduction in biomedical question-answering.
All experiments were executed using Python notebooks and API-based LLM calls. No model weights are stored inside this repository.
The repository is structured to allow anyone to understand how the dataset was prepared, how the experiments were run, and how evaluation metrics were computed.

## 2. Thesis Title
“Reducing Hallucinations in Healthcare Chatbots: A Comparative Study of Prompting Techniques versus Retrieval-Augmented Generation (RAG)”

## 3. Experiments Included
### 3.1 Dataset Preparation
Loading the biomedical QA dataset
Verifying required fields (qtype, question, answer)
Cleaning and arranging the final dataset used across all experiments

### 3.2 Prompt-Based Techniques
The following prompt strategies were implemented and tested:
Zero-Shot
Few-Shot
Chain-of-Thought
Self-Consistency
Tree-of-Thought

### 3.3 RAG-Based Techniques
Sparse, Dense, Hybrid RAG

### 3.4 Evaluation Metrics
All outputs from prompting and RAG were evaluated using:
Faithfulness,Hallucination rate,Correctness,Relevance
(For RAG only) Context Precision, Context Recall

## 5. Environment Requirements
Python (Jupyter Notebook environment)
Standard scientific libraries (pandas, numpy, etc.)
Additional libraries for embeddings, retrieval, or API calls
External LLMs accessed through API keys (keys are not included)
To run the experimentation notebooks, add your own Groq API key.  


