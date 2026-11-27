# Agentic RAG with LangGraph

Hands-on examples of **agentic RAG** from the LUMI AI Factory.

Standard RAG runs as a static pipeline: embed a query, fetch the top chunks, and pass them to the model. That works for straightforward lookups, but breaks down when a question is ambiguous, covers multiple topics, or misses on the first search. Agentic RAG puts the LLM in **a loop** instead, letting it decide when to search, what queries to run, and whether to try again with different terms before answering.

New to RAG? The [RAG chapter](https://lumi-ai-factory.github.io/The-Pragmatic-Guide-to-LLMs/8-rag) of *The Pragmatic Guide to LLMs* gives a short introduction.

## Notebooks

| Notebook | Description |
| --- | --- |
| `01_RAG_Basics.ipynb` | Introductory notebook requiring no prior knowledge. Queries a model about LUMI AI Factory with and without RAG, then adds basic agentic search and compares it with putting the whole website in the prompt. Uses the local copy of the LUMI AI Factory website in `lumi_aif_website/`. Ends with a section for trying the agent on your own markdown files or PDFs (put them in `own_docs/`). |
| `02_agentic_rag.ipynb` | Full LangGraph implementation with rolling conversation memory, query rewriting, human-in-the-loop clarification, parallel sub-agents, and context compression. Downloads the latest [LUMI documentation](https://docs.lumi-supercomputer.eu/) on each run and only rebuilds the index when the docs have changed. |

## Setup

You need [Python 3.11+](https://www.python.org/downloads/) and `git`; the commands below install everything else. No GPU or model downloads required.

**macOS / Linux:** check for git with `git --version`. On macOS this offers to install it if it is missing; on Linux use your package manager (for example `sudo apt install git` on Ubuntu/Debian, `sudo dnf install git` on Fedora).

```bash
git clone https://github.com/lumi-ai-factory/Agentic_RAG_LangGraph.git
cd Agentic_RAG_LangGraph

python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

cp .env.example .env
```

**Windows (PowerShell):** install git with `winget install --id Git.Git -e` (if it is already installed, winget says so), then open a new PowerShell window.

```powershell
git clone https://github.com/lumi-ai-factory/Agentic_RAG_LangGraph.git
cd Agentic_RAG_LangGraph

py -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt

copy .env.example .env
```

If PowerShell refuses to run `Activate.ps1` ("running scripts is disabled"), run
`Set-ExecutionPolicy -Scope CurrentUser RemoteSigned` once and try again.

Add your [Aitta](https://aitta.csc.fi/public) API key to `.env`. That's the only change needed to run both notebooks. Then open `01_RAG_Basics.ipynb`:

- **VS Code** (with the Python and Jupyter extensions): click **Select Kernel** in the top right -> **Python Environments...** -> `.venv`.
- **JupyterLab**: with `.venv` active, run `pip install jupyterlab && jupyter lab`.

Support for running these notebooks on [Noppe](https://noppe.csc.fi) (CSC's browser-based Jupyter platform) is planned; instructions will be added here when ready.

### Model configuration
Both the LLM and embedding model are called over an API. The default provider is [Aitta](https://aitta.csc.fi/public) (inference service by LUMI AI Factory at CSC). Only the vector database runs locally in the notebook.

Both the LLM and the embedding model use LangChain's OpenAI-compatible clients, so you can switch to OpenAI, a local [Ollama](https://ollama.com) or [vLLM](https://docs.vllm.ai/) server, or another hosted gateway by editing the settings at the top of notebook 2:

```python
BASE_URL = "https://aitta-api.csc.fi/openai/v1"
API_KEY = os.environ["AITTA_API_KEY"]
LLM_MODEL = "google/gemma-4-26B-A4B-it"
EMBEDDING_MODEL = "intfloat/multilingual-e5-large"
```

The model you choose must support **tool calling** so the agent can invoke search. For providers that are not OpenAI-compatible (such as Anthropic or Google Gemini), see the [LLM provider configuration](https://github.com/GiovanniPasq/agentic-rag-for-dummies#llm-provider-configuration) in the upstream repo.

## Credits

Adapted from [agentic-rag-for-dummies](https://github.com/GiovanniPasq/agentic-rag-for-dummies)
by Giovanni Pasqualino (© 2025, MIT License), which provides the parent/child retrieval design and LangGraph architecture.

This adaptation swaps in the LUMI documentation, defaults to CSC's Aitta service, and aligns the notebooks with *[The Pragmatic Guide to LLMs](https://lumi-ai-factory.github.io/The-Pragmatic-Guide-to-LLMs/)*.

The pages in `lumi_aif_website/` are a snapshot of [lumi-ai-factory.eu](https://lumi-ai-factory.eu/) (© 2026 LUMI AI Factory; see `lumi_aif_website/SOURCE.txt`).
