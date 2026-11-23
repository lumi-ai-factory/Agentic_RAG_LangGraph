# Agentic RAG with LangGraph

A worked example of **agentic RAG** from the LUMI AI Factory.

Ordinary RAG is a fixed pipeline: embed the question, fetch the top few chunks, paste them into
the prompt, answer. It works until the question is vague, or spans two topics, or the first
search simply misses. Agentic RAG replaces that straight line with a loop the model controls —
it decides whether to search, what to search for, whether the result was good enough, and when
to search again with different words. This repository builds one, from the simplest thing that
works up to a full [LangGraph](https://langchain-ai.github.io/langgraph/) implementation.

Both notebooks use material no language model has read during training, so you can see plainly
when an answer came from retrieval and when it was invented.

## The notebooks

| Notebook | What it covers |
| --- | --- |
| `01_RAG_Basics.ipynb` | Start here. Ask a model about LUMI AI Factory with and without RAG, then let it search for itself. A handful of short cells, no prior knowledge needed. Uses the saved copy of the LUMI AI Factory website in `lumi_aif_website/`. |
| `02_agentic_rag.ipynb` | The advanced version: rolling conversation memory, query rewriting, human-in-the-loop clarification, parallel sub-agents, and context compression. Downloads the latest [LUMI documentation](https://docs.lumi-supercomputer.eu/) on every run and rebuilds its index only when the documentation has changed. |

Answers link to the pages they are based on.

Have PDFs rather than markdown? The upstream project has a
[PDF-to-markdown notebook](https://github.com/GiovanniPasq/agentic-rag-for-dummies/blob/main/notebooks/pdf_to_markdown.ipynb).

## The theory lives elsewhere

This repository is deliberately code-only. If you want to understand *why* any of it is shaped
the way it is, read these first — they are written for the same audience:

- **[Retrieval-Augmented Generation](https://arbruiser.github.io/The-Pragmatic-Guide-to-LLMs/8-rag)** —
  the indexing–retrieval–generation pipeline, chunking, hybrid search, reranking, and how to
  evaluate the result.
- **[Agentic RAG](https://arbruiser.github.io/The-Pragmatic-Guide-to-LLMs/9-agentic-rag)** —
  where the fixed pipeline breaks down, what an agent adds, and why a graph rather than a loop.

Both are chapters of [The Pragmatic Guide to LLMs](https://arbruiser.github.io/The-Pragmatic-Guide-to-LLMs/).

## Getting started

The language model and the embedding model are called over an API; the vector database runs
inside the notebook. A laptop with Python 3.11+ and `git` is enough — no GPU, no model downloads.

```bash
git clone https://github.com/lumi-ai-factory/Agentic_RAG_LangGraph.git
cd Agentic_RAG_LangGraph

python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

cp .env.example .env
```

Put your API key in `.env`, then open a notebook:

- **VS Code** (with the Python and Jupyter extensions): open `01_RAG_Basics.ipynb`, click
  **Select Kernel** in the top right → **Python Environments…** → `.venv`.
- **In the browser:** with the virtual environment active, run `pip install jupyterlab` and then
  `jupyter lab`.

Run the cells from top to bottom with **Shift + Enter**.

If you would rather not install anything locally, the notebooks are meant to also run on
**[Noppe](https://noppe.csc.fi)**, CSC's browser-based Jupyter platform. Instructions will follow.

### Choosing a language model

The notebooks default to [Aitta](https://aitta.csc.fi/public), CSC's inference service, because
it is what Finnish and European users are most likely to already have access to. Put your key in
`.env` as `AITTA_API_KEY` and you are done.

Nothing in the code is tied to it, though. Both models are created through LangChain's
OpenAI-compatible clients, so switching providers means changing the settings at the top of
the notebook — the service address, the API key, and the model names:

```python
BASE_URL = "https://aitta-api.csc.fi/openai/v1"   # ← any OpenAI-compatible endpoint
API_KEY = os.environ["AITTA_API_KEY"]
LLM_MODEL = "google/gemma-4-26B-A4B-it"
EMBEDDING_MODEL = "intfloat/multilingual-e5-large"
```

That covers a local [Ollama](https://ollama.com) or [vLLM](https://docs.vllm.ai/) server, OpenAI
itself, and most hosted gateways. For providers that are *not* OpenAI-compatible — Anthropic and
Google Gemini, say — the upstream project this is based on has
[ready-made configuration for each](https://github.com/GiovanniPasq/agentic-rag-for-dummies#llm-provider-configuration).

Whatever you pick needs **tool calling**; without it the agent cannot search.

## Credits

This project is adapted from
**[agentic-rag-for-dummies](https://github.com/GiovanniPasq/agentic-rag-for-dummies)** by
Giovanni Pasqualino — copyright © 2025, MIT licensed. That is where the parent/child retrieval
design and the overall graph architecture come from. It is a genuinely good piece of teaching
material and well worth reading in its own right; it also ships the same ideas as a structured
Python package under `project/`, if you would rather have that than a notebook.

The adaptation here swaps in the LUMI documentation, targets CSC's Aitta inference service by
default, and rewrites the material to sit alongside the guide linked above.

The pages in `lumi_aif_website/` are a snapshot of [lumi-ai-factory.eu](https://lumi-ai-factory.eu/),
© 2026 LUMI AI Factory; see `lumi_aif_website/SOURCE.txt`.
