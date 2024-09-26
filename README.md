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