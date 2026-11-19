# PlayerOne - Local LLM Flow Engine

A lightweight, fully offline local LLM orchestration framework inspired by Azure Prompt Flow. Enables declarative construction and evaluation of conversational agent pipelines using open-source models without cloud API dependencies.

## Architecture

- Declarative Flows: Define execution DAGs and conversational parameters using standard YAML configuration files.
- Local Inference: Integrates HuggingFace `transformers` and `torch` to run models (such as GPT-2 or Phi-2) locally on CPU or CUDA.
- Interactive CLI: Built with `typer` to provide rapid initialization, testing, and debugging directly from terminal sessions.

## Quick Start

```bash
# Install dependencies
pip install -r PlayerOne/requirements.txt

# Initialize a new conversational flow
python -m PlayerOne.main init my_chatbot

# Run interactive chatbot session
python -m PlayerOne.main test my_chatbot
```
