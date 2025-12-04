.

## API Key

To run the experimentation notebooks, add your own Groq API key.  
The key used during development has been removed for security reasons.
## 1. Overview
This repository contains the complete experimentation code, dataset, and supporting files used in my MSc thesis.
The research analyses how different prompt-based techniques and RAG methods influence hallucination reduction in biomedical question-answering.
All experiments were executed using Python notebooks and API-based LLM calls. No model weights are stored inside this repository.
The repository is structured to allow anyone to understand how the dataset was prepared, how the experiments were run, and how evaluation metrics were computed.

## 2. Thesis Title
“Reducing Hallucinations in Healthcare Chatbots: A Comparative Study of Prompting Techniques versus Retrieval-Augmented Generation (RAG)”
## 3. Repository Structure
LJMU_MS_ML_AI/
│
├── Experimentation_Code/
│   │
│   ├── Data_preprpceesing/
│   │   └── Contains the MedQuAD dataset used for experiments & preprocessing code
│   │
│   ├── Prompt_Methods/
│   │   └── Code and notebooks for all prompt-based methods, evaluation
│   │
│   ├── RAG_Methods/
│       └── Implementation of RAG pipelines and retrieval setups, evaluation
│   
│   
└── README.md   (This file)

## 4. Experiments Included
### 4.1 Dataset Preparation
Loading the biomedical QA dataset
Verifying required fields (qtype, question, answer)
Cleaning and arranging the final dataset used across all experiments

### 4.2 Prompt-Based Techniques
The following prompt strategies were implemented and tested:
Zero-Shot
Few-Shot
Chain-of-Thought
Self-Consistency
Tree-of-Thought

### 4.3 RAG-Based Techniques
Sparse, Dense, Hybrid RAG

### 4.4 Evaluation Metrics
All outputs from prompting and RAG were evaluated using:
Faithfulness,Hallucination rate,Correctness,Relevance
(For RAG only) Context Precision, Context Recall
