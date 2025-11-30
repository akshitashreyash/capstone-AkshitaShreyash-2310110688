# Title: QUESTION BANK GENERATOR 

## Overview

This repository converts lecture notes (PDF, PPTX, TXT) into a high-quality, structured question bank. Outputs include multiple-choice questions (MCQs), short-answer questions, and concept-check items. Each question includes source excerpt and location, difficulty level, topic tags, and an answer explanation. The system emphasizes reproducibility, low error rate, and demonstrable use of course concepts: Prompting, Structured Output, Semantic Search, RAG, Langgraph (nodes & state), and Langsmith instrumentation for debugging.
## Reason for picking up this project

I have picked this project because it shows a lot of the functions of langchain and langgraph that we have learnt the course. A lot of codes run in this project are to double-check that all of my logistics are in order. Although, this reflects on my right-now novice skills, they only contribute to elaborating the project even further. Following are the skills which have been implemented in the project:

* xyz


## Plan

I plan to execute these steps to complete my project.

[DONE] Step 1: Ingest and clean lecture notes (PDF/PPTX/TXT) into standard .txt format.

[DONE] Step 2: Chunk text and generate embeddings for semantic retrieval.

[DONE] Step 3: Create prompts which will make the model familar with types of questions - MCQs, small questions, explain concepts in short. 

[DONE] Step 4: Execute langgraph pipeline that takes chunks and construct MCQ prompts similar to step 3 (retriever → generator → evaluator). 

[DONE] Step 5: define reusable tools for semantic search and topic inspection over lecture chunks, a tool-calling wrapper function that returns context chunks ready to be consumed by your LangGraph question-generation workflow.

[TODO] Step 6: Add evaluation node for confidence scoring and error-flagging.

[TODO] Step 7: Export results to CSV/JSON/Anki format using tool-calling.

[TODO] Step 8: Build the final demo notebook combining the entire pipeline.

[TODO] Step 9: Test thoroughly, debug using LangSmith, and write conclusion.

## Conclusion:

I had planned to build a full pipeline that converts lecture notes into a structured question bank using retrieval and LangGraph.

----------
  