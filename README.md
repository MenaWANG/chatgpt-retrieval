# chatgpt-retrieval & Rag

This repository is based on the work and demonstration by TechLead on ChatGPT Retrieval. You can find the original [YouTube Video here](https://youtu.be/9AXP7tCI9PI).

I also added a RAG implementation to the repo.  

In addition, `pipenv` is utilized for environment management. Pls see details below.

## Installation

Install `pipenv` if you don't have it already
```
pip install pipenv
```

Activate the virtual environment
```
pipenv shell
```


Install the dependencies specified in the `Pipfile.lock` file
```
pipenv install
```

## Custom Data

Place your own data into the `data/` folder.

## Example usage
Test reading `data/data.txt` file.
```
> python chatgpt.py "what is my dog's name"
Your dog's name is Sunny.
```

Test reading `data/cat.pdf` file.
```
> python chatgpt.py "what is my cat's name"
Your cat's name is Muffy.
```

## RAG

In addition to what's in the original repo, I also experimented a bit more with RAG 🤩, following the [LangChain doc](https://python.langchain.com/docs/use_cases/question_answering/), I added a RAG implementation that utilizes a webpage as the knowledge base. Pls run `rag_web.py` for fun, or check out `rag_web.ipynb` for sample results. 

