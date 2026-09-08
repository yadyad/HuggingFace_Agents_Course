# Hugging Face Agents Course

A hands-on learning repository for exploring **AI agents, LangChain, and LangGraph**, based on the [Hugging Face Agents Course](https://huggingface.co/learn/agents-course).

This repository contains experiments, notebooks, and small projects created while learning how LLM-based agents work.

## What I'm Learning

* LangChain
* LangGraph
* AI agents and agent workflows
* Tools and tool calling
* State management
* Conditional routing
* Local LLMs with Ollama
* LLM observability with Langfuse
* Mermaid graph visualization

## Repository Structure

```text
HuggingFace_Agents_Course/
│
├── langgraph-practise/
│   ├── HelloWorld_langgraph.ipynb
│   └── accessing_local_LLM.ipynb
│
├── dummy_agent.ipynb
├── firstagent.py
├── requirements.txt
└── README.md
```

## LangGraph Practice

One of the main projects is a simple **email processing agent** built with LangGraph.

The workflow:

```text
Incoming Email
      ↓
Read Email
      ↓
Classify Email
      ↓
 ┌────┴────┐
Spam    Legitimate
 ↓          ↓
Handle    Draft
Spam     Response
            ↓
       Notify User
```

This project is helping me understand:

* Graph state
* Nodes and edges
* Conditional routing
* Multi-step LLM workflows
* Structured LLM responses

## Local LLMs

I'm experimenting with running models locally using **Ollama**, allowing the LangChain and LangGraph workflows to work with local LLMs.

## Observability

I'm also experimenting with **Langfuse** to trace and understand LLM calls and agent workflows.

## Setup

Clone the repository:

```bash
git clone https://github.com/yadyad/HuggingFace_Agents_Course.git
cd HuggingFace_Agents_Course
```

Create a virtual environment:

```bash
python -m venv .venv
```

Activate it and install dependencies:

```bash
pip install -r requirements.txt
```

For experiments requiring API keys, create a `.env` file:

```env
LANGFUSE_PUBLIC_KEY=your_public_key
LANGFUSE_SECRET_KEY=your_secret_key
LANGFUSE_HOST=your_langfuse_host
```

Then load it with:

```python
from dotenv import load_dotenv

load_dotenv()
```

## Project Status

🚧 **Work in progress**

This is primarily a learning and experimentation repository. The code will evolve as I learn more about LangChain, LangGraph, and AI agent architectures.

## Resources

* [Hugging Face Agents Course](https://huggingface.co/learn/agents-course)
* [LangChain](https://www.langchain.com/)
* [LangGraph](https://www.langchain.com/langgraph)
* [Langfuse](https://langfuse.com/)
* [Ollama](https://ollama.com/)

---

**Learning by building, experimenting, and debugging.**
