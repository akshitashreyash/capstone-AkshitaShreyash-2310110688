# Title: QUESTION BANK GENERATOR 

## Overview

This repository converts lecture notes (PDF, PPTX, TXT) into a high-quality, structured question bank. Outputs include multiple-choice questions (MCQs), short-answer questions, and concept-check items. Each question includes source excerpt and location, difficulty level, topic tags, and an answer explanation. The system emphasizes reproducibility, low error rate, and demonstrable use of course concepts: Prompting, Structured Output, Semantic Search, RAG, Langgraph (nodes & state), and Langsmith instrumentation for debugging.
## Reason for picking up this project


## Plan

I plan to execute these steps to complete my project.

[DONE] Step 1: Ingest and clean lecture notes (PDF/PPTX/TXT) into standard .txt format.

[TODO] Step 2: Chunk text and generate embeddings for semantic retrieval.

[TODO] Step 3: Build FAISS index and test semantic search.

[TODO] Step 4: Create prompt templates and JSON schemas for MCQs and SAQs.

[TODO] Step 5: Build LangGraph pipeline (retriever → generator → evaluator).

[TODO] Step 6: Add evaluation node for confidence scoring and error-flagging.

[TODO] Step 7: Export results to CSV/JSON/Anki format using tool-calling.

[TODO] Step 8: Build the final demo notebook combining the entire pipeline.

[TODO] Step 9: Test thoroughly, debug using LangSmith, and write conclusion.

## Conclusion:

I had planned to build a full pipeline that converts lecture notes into a structured question bank using retrieval and LangGraph.

----------
  