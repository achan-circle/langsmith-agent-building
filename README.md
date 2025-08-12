# Agent Buliding

Welcome to Agent Building

## Introduction
In this session, you will learn about the fundamentals of LangGraph through one of our notebooks. This is a condensed version of LangChain Academy, and is intended to be run in a session with a LangChain engineer. If you're interested in going into more depth, or working through a tutorial on your own, check out LangChain Academy [here](https://academy.langchain.com/courses/intro-to-langgraph)! LangChain Academy has helpful pre-recorded videos from one of our LangChain engineers.

## Pre-work

### Clone the LangSmith Workshops repo
```
git clone https://github.com/langchain-ai/langsmith-workshops
```

### Create an environment and install dependencies  
```
# Ensure you have a recent version of pip and python installed
$ cd langsmith-in-code
$ python3 -m venv .venv
$ source .venv/bin/activate
$ pip install -r requirements.txt
```

 Create a .env file in the root folder using ```.env.example``` as an example.

### Running notebooks
Make sure the following command works and opens the relevant notebooks
```
$ jupyter notebook
```

### Azure OpenAI Instructions

If you are using AzureOpenAI instead of OpenAI, there are a few things you need to do.

1. Set necessary environment variables in a .env file. Specifically, make sure you set
    - AZURE_OPENAI_API_KEY=
    - AZURE_OPENAI_ENDPOINT=
    - AZURE_OPENAI_API_VERSION=

2. Navigate to `models.py`, and uncomment the code for 
    - `AZURE_OPENAI_EMBEDDING_MODEL`= ...
    - `AZURE_OPENAI_GPT_4O`= ...

3. Navigate to `utils.py` and use AzureOpenAIEmbeddings instead of OpenAIEmbeddings

4. In the notebooks, use AzureOpenAI (code already provided in cells) where applicable, instead of OpenAI (default)