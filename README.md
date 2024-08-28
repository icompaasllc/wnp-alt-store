

Setup the Environment for Agent Based

# Install Virutal Environment

Two ways (prefer Conda)

## Install using Conda

`conda create -n pyautogen python=3.9.18`
`conda activate pyautogen`


`conda deactivate`


## Install using venv

`python3 -m venv pyautogen`
`source pyautogen/bin/activate`


`deactivate`


# Start Serving LLMs Locally

Ollama Serving

## Mistral Config - Only need this when on a server side not client side - client side use groq SDK

`ollama serve --config mistral-config.json`


pip install 'litellm[proxy]'

litellm --model mistral &


litellm --config llama3-groq-config.yaml