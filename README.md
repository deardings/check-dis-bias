# Disability Bias in Open AI API Models

I am wrtiting a paper on disability bias in recent OpenAI models (GPT4.1, that is). This repo holds the Jupyter notebook with the code used for my study. The code holds not only the prompts, but also the complete materials provided to the agent. My reference is a paper by [Glazko et al](https://dl.acm.org/doi/10.1145/3630106.3658933), written for FAccT Conference 2024.

## Installation via `uv`

First, clone the repo:

```
git clone
```

I used [uv](https://docs.astral.sh/uv/) for package management and creating my `.venv`. You are recommended to do so, too.

### Windows

```pwsh note="on Windows"
uv venv -p313
.venv/Scritps/activate
uv sync
```

### Linux

```bash
uv venv -p313
source .venv/bin/activate
uv sync
```

## Installation via `pip`

If you prefer pip, a recent requirements.txt is also provided. Just use

```bash
pip install -r requirements.txt
```

## Running the Notebook

I used VS Code with a very basic configuration for editing and executing my notebook. If you prefer running your own Jupyter server, you should be familiar with how to do so yourself.

The code need an API-Key for OpenAI. You can also change the provider URL and try to run the experiment on any other model that is compatible with the OpenAI response API.

