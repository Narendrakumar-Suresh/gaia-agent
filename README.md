---
title: Gaia Agent - Intelligent Question Answering System
emoji: 🤖
colorFrom: indigo
colorTo: indigo
sdk: gradio
sdk_version: 5.25.2
app_file: app.py
pinned: false
hf_oauth: true
hf_oauth_expiration_minutes: 480
---

# Gaia Agent - Intelligent Question Answering System

## Overview
Gaia is an advanced question-answering system that combines multiple AI capabilities including web search, Wikipedia lookup, and academic paper analysis to provide comprehensive answers to complex questions.

## Features
- 🔍 Multi-source research (Web, Wikipedia, ArXiv)
- 🧮 Mathematical operations support
- 💾 Vector store for similar question retrieval
- 🤖 Multiple LLM provider support (Google, Groq, HuggingFace)
- 🔐 Secure OAuth authentication

## Tech Stack
- **Framework**: Gradio for UI
- **LLM Integration**: LangChain & LangGraph
- **Vector Store**: Supabase
- **Search Tools**: 
  - Tavily for web search
  - Wikipedia API
  - ArXiv API

## Setup
1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up environment variables in `.env.local`:
   ```bash
   SPACE_ID=your-space-id
   HF_TOKEN=your-hf-token
   # ... other API keys
   ```

## Usage
1. Run the application:
   ```bash
   python app.py
   ```
2. Log in with your Hugging Face account
3. Submit questions and receive comprehensive answers

## Architecture
- `app.py`: Main application and Gradio interface
- `agent.py`: Agent implementation with tools and LLM integration
- `system_prompt.txt`: System instructions for the agent
- `metadata.jsonl`: Question-answer pairs database

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
MIT License

## Contact
Created by [Your Name] - feel free to contact me!
