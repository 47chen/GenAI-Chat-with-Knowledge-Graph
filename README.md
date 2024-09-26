# Chat-with-Knowledge-Graph

## Introduction

This project demonstrates how to build a knowledge graph from unstructured data using open-source tools and large language models. It leverages the Ollama Mistral model for entity and relationship extraction, Neo4j for graph database storage, and Streamlit for a user-friendly chat interface.

## Project Overview

The project consists of two main components:

1. **Knowledge Graph Construction:**
   - Uses the Ollama Mistral model served as a RESTful API on a local machine
   - Processes raw data to extract entities and relationships
   - Generates Cypher statements using customized prompt templates
   - Executes Cypher statements to build nodes and relationships in Neo4j

2. **Interactive Chat Interface:**
   - Utilizes Streamlit to create a simple UI for interacting with the knowledge graph
   - Implements LangChain for advanced query processing and graph interactions
   - Uses the Ollama LLaMA 3.1 model for improved English-to-Cypher translation and query from Graph DB Neo4j.

## Key Features

- Open-source LLM integration with Ollama
- Knowledge graph construction from unstructured data
- Neo4j graph database for efficient storage and querying
- Streamlit-based chat interface for user interactions
- LangChain integration for advanced natural language processing and interaction with graph as Chatbot.

## Technologies Used

- Ollama Mistral and LLaMA 3.1 models
- Neo4j as Graph Database
- Streamlit as Chat UI
- LangChain
- Python

##

### Knowledge graph in Neo4j
![image](https://github.com/user-attachments/assets/7096053b-ec3b-4cc1-8151-86360a76266c)

Look closely we can see the relationship between entities
![image](https://github.com/user-attachments/assets/70a0190b-1f9e-485f-81a1-2de9888adb96)
![image](https://github.com/user-attachments/assets/e0d53300-6a10-4603-990d-52811e76fac3)

We can see it as table field as well
![image](https://github.com/user-attachments/assets/cb047e24-1d14-43ca-972a-1f6be39425ae)

## Demo
* Each request&returning response takes aprox. 20sec based on performance via Ollama LLama3.1-8b
#### Question: Which projects use Azure? Answer includes human response + cypher statement + query result from neo4j
![image](https://github.com/user-attachments/assets/364f2d49-0a25-4d9a-b9cf-ac99ce2354b4)

#### Question:Which project use Azure and the name starts character B?
![image](https://github.com/user-attachments/assets/7d43217e-e949-40f3-b6fa-be85615b9198)

#### If you ask something that exceed the knowledge graph, it is already prompted to answer "I don't know"
![image](https://github.com/user-attachments/assets/d20c7aa4-ee87-4c34-a938-f4556144254a)


