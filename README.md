# fact-checker-llm
Retrieval-augmented, LLM-powered fact-checking pipeline for verifying news and social media claims using embeddings and local language models. Built in Jupyter Notebook, with CSV export support.
This project is an **AI-powered, retrieval-augmented fact-checker** for news and social claims.  
It leverages modern NLP transformers to extract claims from input text and matches them against a dataset of verified facts using embedding-based similarity search (FAISS).  
LLM verdicts (True/False/Unverifiable) and reasoning are generated from a local open-source language model (Flan-T5).

## Features
- Claim/Entity Extraction from arbitrary input
- Embedding similarity retrieval from custom fact database (100+ facts)
- LLM-powered verdict (uses HuggingFace Flan-T5, purely local)
- Confidence scoring for each claim result
- Batch/Single claim support
- Exports result to CSV/Excel for reporting/evaluation
- Modifiable in Jupyter Notebook or Python scripts

## How to Use
1. Add and update verified facts in `facts.csv`.
2. Run all notebook cells to initialize models and generate embeddings.
3. Input any statement—extract claim, find similar facts, get a verdict.
4. Export results to CSV/Excel for sharing or documentation.
5. Upload all files and notebook to GitHub for collaboration/submission.

## Technologies
- Jupyter Notebook
- Pandas, NumPy
- sentence-transformers
- HuggingFace transformers (Flan-T5)
- FAISS (vector similarity)
- Export to CSV/XLSX
