---
title: AI Engineer Roadmap
---

# AI Engineer

Use foundation models and existing AI tools to build useful, evaluated products.

[← Role based roadmaps](README.md) | [All roadmaps](../README.md)

## What an AI engineer does

An AI engineer applies models to product problems. The role combines application programming, retrieval, prompt design, evaluation, safety, and operations. Many AI engineers do not train models; they choose tools, shape data, measure quality, and design reliable system behavior.

## Start here

- [ ] Call a model API from a small application
- [ ] Create a small evaluation set with expected outputs
- [ ] Add one retrieval or tool-using workflow
- [ ] Document the failure modes, cost, and latency

## Learning stages

### 1. Foundations

- HTTP APIs, JSON, environment variables, and secret handling
- Python or TypeScript application fundamentals
- Probability basics: uncertainty, sampling, and distributions
- Model inputs and outputs: tokens, context windows, temperature, and structured output
- Data privacy and provider terms

**Build:** a command-line assistant that takes a question, calls a model, and prints a sourced response.

### 2. Prompt and context design

- Clear instructions, constraints, and examples
- Structured output with schemas and validation
- Retrieval: chunking, embeddings, search, and reranking
- Context assembly and token budgets
- Prompt versioning and regression tests
- Handling untrusted retrieved content

**Build:** a question-answering tool over a small, trusted document set with citations.

### 3. Evaluation

- Define a quality rubric before tuning
- Create representative, difficult, and adversarial examples
- Automated checks plus human review
- Measure accuracy, groundedness, latency, and cost
- Compare models and prompts on the same dataset
- Track regressions as prompts and data change

**Build:** an evaluation script that fails when a prompt change degrades a clearly defined quality threshold.

### 4. Application architecture

- API gateways, timeouts, retries, and streaming responses
- Caching and request routing
- Model fallbacks and graceful degradation
- Background processing for slow tasks
- Observability across retrieval, prompts, tools, and outputs
- Data storage, retention, and deletion

**Build:** a retrieval-backed feature with request tracing, a spend budget, and a fallback when the primary model is unavailable.

### 5. Safety and production delivery

- Prompt injection, data exfiltration, and unsafe tool use
- Access control for data and actions
- Human confirmation for consequential operations
- Content filters where appropriate, without treating them as a complete safety solution
- Incident response and user feedback loops
- Deployment, rollback, and ongoing evaluation

**Build:** document the threat model for an AI feature and implement one concrete control for each major risk.

## Definition of done

You can build an AI feature with a clear user problem, measurable quality, bounded cost and latency, safe tool access, and a process for improving it with evidence.

## Related roadmaps

- [Python](../skill-based/python.md)
- [Prompt engineering](../ai/prompt-engineering.md)
- [AI agents](../ai/ai-agents.md)

## FAQ

### Is machine learning required?

A working understanding helps. AI engineering interviews often focus more on software design, evaluation, data handling, and product judgment than on implementing training algorithms from scratch.

[↑ Catalog](README.md) | [← Category index](README.md)
