# Disability Bias in Open AI API Models

I am wrtiting a paper on disability bias in recent OpenAI models (GPT4.1, that is). This repo contains the paper itself, all data and prompts used in the experiment, the Jupyter notebook the experiment itself as well as the results.

It holds three Jupyter notebooks:   
* `cv_creation.ipynb` with a protocol of the creation a control curriculum vitae (CV) and 6 enhanced variants with references to disability.
* `experimnet.ipynb` with the actual conduction of the experiment 
The code holds not only the prompts, but also the complete materials provided to the agent. My reference is a paper by [Glazko et al](https://dl.acm.org/doi/10.1145/3630106.3658933), written for FAccT Conference 2024.
* `charts.ipynb` used to create a chart for the paper.

In the `results` folder you can also find a .csv-export with the results of 10x10 runs of the experiment using GPT-4.1. 

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

