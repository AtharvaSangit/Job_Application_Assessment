
# Job Application Assessment Agent using LangGraph & LangChain

This project demonstrates a stateful multi-agent system that evaluates job applications using **LangGraph**, **LangChain**, and **OpenAI's GPT-4**.

## Overview

The system takes structured input—**job title**, **experience level**, and **skills**—and processes it through a graph of LLM-powered nodes. Each node performs a reasoning task (e.g., role matching, experience validation) and contributes to generating a final assessment.

## 🛠️ Tech Stack

* **LangGraph** – for graph-based multi-agent workflows
* **LangChain** – to manage LLM chains
* **OpenAI** – for natural language processing
* **Python** – implementation language
* **Google Colab** – development environment

## How It Works

* A `TypedDict` defines a shared application state (`job_title`, `experience`, `skills`, etc.).
* LangGraph nodes process this state:

  * Node 1: Determines if the job title matches a known category.
  * Node 2: Evaluates experience level relevance.
  * Node 3: Checks skill alignment.
  * Final Node: Generates an LLM-based response with suggestions or feedback.
* The graph supports conditional flows and loops, enabling robust evaluation logic.

## Output

An assessment summarizing how well the applicant fits the role and suggesting improvements if needed.


