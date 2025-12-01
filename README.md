# Title: QUESTION BANK GENERATOR 

## Overview

This repository converts lecture notes (PDF, PPTX, TXT) into a high-quality, structured question bank. Outputs include multiple-choice questions (MCQs), short-answer questions, and concept-check items. Each question includes source excerpt and location, difficulty level, topic tags, and an answer explanation. The system emphasizes reproducibility, low error rate, and demonstrable use of course concepts: Prompting, Structured Output, Semantic Search, RAG, Langgraph (nodes & state), and Langsmith instrumentation for debugging.

## Reason for picking up this project

I have picked this project because it shows a lot of the functions of langchain and langgraph that we have learnt the course. A lot of codes run in this project are to double-check that all of my logistics are in order. Although, this reflects on my right-now novice skills, they only contribute to elaborating the project even further. Following are the skills which have been implemented in the project:

1. **PROMPTING** : designing detailed prompts that tell the model exactly the type of content to generate. In this project the model generates MCQs in a detailed manner.
2. **SEMANTIC SEARCH** :Built a TF‑IDF embedding over all lecture chunks and wrote semantic_search_local(query, k) to fetch the most relevant text pieces for any topic before generating questions.
3. **RAG**: Combined semantic search outputs with prompting so the model always sees concrete lecture excerpts in the context block and generates questions grounded in that material.
4. **TOOL CALLING**: Wrapped semantic search and helper functions as “tools” that a future LLM agent could call step‑by‑step instead of doing everything in one prompt.
5. **LANGGRAPH**: Used QGenState(task of holding everything while the code runs) and also built nodes (retrieve, build_prompt, llm_call, validate) wired in a StateGraph so question generation becomes a clear pipeline with explicit state updates and conditional edges.

**VIDEO SUMMARY LINK**: 


## Plan

I plan to execute these steps to complete my project.

**[DONE]** Step 1: Ingest and clean lecture notes (PDF/PPTX/TXT) into standard .txt format.

**[DONE]** Step 2: Chunk text and generate embeddings for semantic retrieval.

**[DONE]** Step 3: Create prompts which will make the model familar with types of questions - MCQs, small questions, explain concepts in short. 

**[DONE]** Step 4: Execute langgraph pipeline that takes chunks and construct MCQ prompts similar to step 3 (retriever → generator → evaluator). 

**[DONE]** Step 5: define reusable tools for semantic search and topic inspection over lecture chunks, a tool-calling wrapper function that returns context chunks ready to be consumed by your LangGraph question-generation workflow.

**[DONE]** Step 6: load the generated MCQs from CSV. Save both full evaluation results and a clean subset for further use

**[DONE]** Step 7: Export results to CSV/JSON/Anki format using tool-calling. Use the app called Anki, a free flashcard generating app.

**[DONE]** Step 8:  runs the LangGraph question-generation pipeline end‑to‑end for chosen topics, saves the resulting MCQs to CSV.

**[DONE]** Step 9: Test thoroughly and create a tester example in working condition which will replace dummy questions (placeholders) with real questions.

## Conclusion:

I had planned to build a full pipeline that converts lecture notes into a structured question bank. Once the code is run, a cvs file gets generated and produces an EXCEL file which contains the output ie the questions What my project does is take in lecture notes in pdf form, breaks them into chunks and then picks up the relevant information which the perplexity model then uses to formulate questions. I am satisfied with the project as it delivers the aim behind the project. With a little refurbishing, it can be turned into a highly useful application which is helpful in the day to day life of students. 

----------
  