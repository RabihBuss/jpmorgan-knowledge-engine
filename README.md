# JPMorgan Chase Knowledge Engine: architecture teardown

**[View the interactive page →](https://rabihbuss.github.io/jpmorgan-knowledge-engine/)**

Also on claude.ai: [Knowledge Engine Architecture](https://claude.ai/artifact/RDUSuBZbDJ86t3S38qXTaN)

An interactive reference architecture for a bank's employee knowledge engine, reconstructed from public statements about JPMorgan Chase's LLM Suite and its four generations of retrieval-augmented generation (RAG). Code walks every question down a trust ladder (scripted answers, live systems of record, durable documents, then temporal material), and one core LLM writes a short answer in which every sentence cites an approved source.

## What's on the page

- **System map:** the online request path in 15 steps, with every component, model call and guarded crossing. Click any box for details, highlight a technique, or step through a worked example.
- **Request flow:** a conversation with a clarifying question, a latency timeline, and a follow-up turn in which the model requests read-only tools.
- **Offline loops:** data preparation, the learning loop and the release loop.
- **Technique map:** where each of 32 techniques sits, from prompt rules to fine-tuning.
- **Anatomy of a core-LLM call, model inventory, contracts, truth and failure, build order.**
- **Rollout and risk:** what peers run in production, real versus perceived risks, what to cut from a first version, a staged rollout and a verdict.
- **Audit and snags:** the page's own self-check, the fixes made before publishing, and open design issues.
- **Start here:** a teaching layer for architects new to AI, with a glossary. Use the *Explanations* switch to hide it.

Works in light and dark themes and at phone width.

## About this design

An independent reference architecture built from public sources. It is **not** a description of JPMorgan Chase's internal systems and is not affiliated with or endorsed by JPMorgan Chase. Component names, policy values, evidence IDs, prompt versions, token counts and latency budgets are illustrative. Every statement about the company carries an evidence label (Confirmed, Reported or Inferred) and links to its source on the page.

## Files

- `index.html`: the complete page, self-contained (no build step; fonts from Google Fonts).
