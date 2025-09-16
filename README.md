# Agent Buliding

Welcome to Agent Building

## Introduction
In this session, you will learn about the fundamentals of LangGraph through one of our notebooks. This is a condensed version of LangChain Academy, and is intended to be run in a session with a LangChain engineer. If you're interested in going into more depth, or working through a tutorial on your own, check out LangChain Academy [here](https://academy.langchain.com/courses/intro-to-langgraph)! LangChain Academy has helpful pre-recorded videos from one of our LangChain engineers.

## Pre-work

### Clone the LangSmith Agent Building repo
```
git clone https://github.com/achan/langsmith-agent-building
```

### Install pip and python - skip if already installed

Install through Kandji by searching for "Python 3", or use brew
```
# Install brew
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
# Install python
$ brew install python
```

### Create an environment and install dependencies  
```
# Ensure you have a recent version of pip and python installed
$ cd langsmith-in-code
$ pip install uv
$ uv sync
$ uv venv
```

Create a .env file in the root folder using ```.env.example``` as an example.
### Create .env file
```
$ cp .env.example .env
$ open .env
```
###
1. fill in `LANGSMITH_ENDPOINT`, `LANGSMITH_API_KEY`, `OPENAI_BASE_URL`, and `OPENAI_API_KEY` as instructed.

## Running notebooks
Make sure the following command works and opens the relevant notebooks
```
$ uv run jupyter notebook
```

The notebooks you should use are in the notebooks folder.
