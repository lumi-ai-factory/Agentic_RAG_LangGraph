# Agentic RAG with LangGraph

A worked example of **agentic RAG** from the LUMI AI Factory.

Ordinary RAG is a fixed pipeline: embed the question, fetch the top few chunks, paste them into
the prompt, answer. It works until the question is vague, or spans two topics, or the first
search simply misses. Agentic RAG replaces that straight line with a loop the model controls —
it decides whether to search, what to search for, whether the result was good enough, and when
to search again with different words. This repository builds one, from the simplest thing that
works up to a full [LangGraph](https://langchain-ai.github.io/langgraph/) implementation.

The demo corpus is the [LUMI supercomputer documentation](https://docs.lumi-supercomputer.eu/),
picked because it is full of specifics no language model knows from training — partition names,
module versions, quota commands — so you can see plainly when an answer came from retrieval and
when it was invented. Swapping in your own documents is a one-line change.

## The notebooks

| Notebook | What it covers |
| --- | --- |
| `01_RAG_Basics.ipynb` | Traditional RAG in about fifteen lines, then the smallest agentic version that beats it. Start here. |
| `02_Agentic_RAG.ipynb` | The full system: rolling conversation memory, query rewriting, human-in-the-loop clarification, parallel sub-agents, context compression, a Gradio chat UI, and a small evaluation harness. |

`PDF_to_Markdown.ipynb` is an optional side quest for pointing the system at your own PDFs.

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

The embedding model and the vector database run locally on CPU, so a laptop is enough. Only the
language model is called over the network.

```bash
git clone https://github.com/lumi-ai-factory/Agentic_RAG_LangGraph.git
cd Agentic_RAG_LangGraph

python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt

cp .env.example .env
```

Fetch the demo corpus — 110 markdown pages, a few seconds:

```bash
git clone --depth 1 --branch production \
  https://github.com/Lumi-supercomputer/lumi-userguide.git .lumi-docs
mkdir -p corpus && cp -r .lumi-docs/docs/. corpus/
rm -rf .lumi-docs corpus/assets
```

Then open `01_RAG_Basics.ipynb`. The first run downloads the embedding model, about 1.2 GB.

If you would rather not install anything locally, the notebooks also run on
**[Noppe](https://noppe.csc.fi)**, CSC's browser-based Jupyter platform — see the setup section
inside `01_RAG_Basics.ipynb`.

### Choosing a language model

The notebooks default to [Aitta](https://aitta.csc.fi/public), CSC's inference service, because
it is what Finnish and European users are most likely to already have access to. Put your key in
`.env` as `AITTA_API_KEY` and you are done.

Nothing in the code is tied to it, though. The model is created through LangChain's
OpenAI-compatible client, so switching providers means changing two lines:

```python
llm = ChatOpenAI(
    model="openai/gpt-oss-120b",
    base_url="https://aitta-api.csc.fi/openai/v1",   # ← any OpenAI-compatible endpoint
    api_key=os.environ["AITTA_API_KEY"],
)
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
