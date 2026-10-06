# Agent Injection Arena

> A small, reproducible benchmark for indirect prompt injection in tool-using agents.

**Status:** open project seed · **License:** MIT · **Contributions:** welcome

Offline benchmark fixtures for indirect prompt injection and agent tool-use boundaries.

## The question

Can an agent treat instructions in retrieved content as untrusted data, and can the surrounding application prevent unauthorized tool actions?

## Why build this

InjecAgent, AgentDojo, and promptfoo already provide valuable agent-security evaluation. This project will start narrowly with paired tasks, explicit action-level ground truth, and easy-to-review contributions.

## First milestone

A local task runner; 20 synthetic tasks across email, docs, and issue trackers; a declared set of allowed and forbidden tool actions; JSONL results with model/runner versions.

## A first contribution

**Add ten benign-versus-malicious paired fixtures for issue and documentation content, with expected tool-action boundaries.**

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the small, reviewable contribution flow. You can also open an issue with the **good first issue** template, propose a test fixture, review a design choice, improve documentation, or help keep the scope honest. No model API key is needed for the initial milestone.

## Working principles

- Treat model output and retrieved content as untrusted input.
- Prefer deterministic controls, explicit assumptions, and reproducible fixtures.
- Use synthetic or public-domain examples; do not commit credentials, private prompts, personal data, or customer logs.
- Report limits and false positives. A benchmark score or static rule is not a security guarantee.
- Keep security tests inside local fixtures or systems you own and have permission to test.

## Research map

This seed is informed by the [OWASP GenAI Security Project](https://genai.owasp.org/), including its LLM and Agentic Application guidance, and by active open-source work such as [garak](https://github.com/NVIDIA/garak), [promptfoo](https://github.com/promptfoo/promptfoo), [LLM Guard](https://github.com/protectai/llm-guard), and [PyRIT](https://github.com/microsoft/PyRIT). Each project aims for a narrow, inspectable contribution rather than a replacement for those broader tools.

[Compare star histories for garak, promptfoo, LLM Guard, and OWASP's LLM Top 10](https://star-history.com/#NVIDIA/garak&promptfoo/promptfoo&protectai/llm-guard&OWASP/www-project-top-10-for-large-language-model-applications). GitHub stars are an attention signal, not evidence of security quality.

## Join in

If this problem interests you, start with the first milestone above. Open an issue to discuss scope before building a large feature, or send a small pull request with a test and a clear explanation. Contributors from security, engineering, research, design, and documentation are all welcome.
