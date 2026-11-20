---
title: Prompt Engineering Roadmap
---

# Prompt Engineering

Design instructions that are testable, maintainable, and grounded in evidence.

[← AI roadmaps](README.md) | [All roadmaps](../README.md)

## Start here

- [ ] Write a versioned system prompt for one narrow task
- [ ] Define an input schema and an expected output format
- [ ] Create five evaluation examples, including one failure case
- [ ] Record the model, settings, and results

## Learning stages

### 1. Requirements before wording

- Define the user, task, and acceptable outcome
- Separate necessary rules from stylistic preferences
- Describe edge cases and what the system should do when information is missing
- Decide whether deterministic code should handle part of the problem
- Identify data that must not be sent to a model

**Build:** a one-page task specification with inputs, outputs, and three examples.

### 2. Instruction structure

- Clear role, goal, context, constraints, and output format
- Examples that demonstrate edge cases, not only the happy path
- Structured JSON or schema-constrained output
- Handling ambiguity and refusal conditions
- Separating trusted instructions from untrusted user or retrieved content
- Token budget and context ordering

**Build:** two competing prompt versions for the same task, each with the same test inputs.

### 3. Retrieval and grounding

- Chunking documents for search
- Embeddings, keyword search, and hybrid retrieval
- Metadata filters and permissions
- Reranking and context selection
- Citation requirements and groundedness checks
- Working with stale, conflicting, or incomplete sources

**Build:** a question-answering workflow over a small document set that returns evidence for each answer.

### 4. Evaluation and iteration

- A representative evaluation dataset
- Rubrics for correctness, completeness, tone, and safety
- Automated scoring where it is reliable, plus human review
- Prompt, model, and retrieval regression tests
- Cost and latency measurements
- Error analysis: categorize failures and fix the most common cause

**Build:** an evaluation report comparing two prompts, with failures grouped by cause.

### 5. Maintenance

- Version prompts alongside the code that calls them
- Track model and provider changes
- Monitor real user feedback and failure rates
- Add guardrails for high-impact or irreversible outputs
- Retire prompts that are no longer used
- Keep an owner and an update process

**Build:** a change log linking prompt revisions to evaluation results and deployment dates.

## Definition of done

You can turn a vague AI task into a measurable specification, build a prompt with representative tests, diagnose failures, and justify changes using evidence rather than intuition.

## Related roadmaps

- [AI engineer](../role-based/ai-engineer.md)
- [AI agents](ai-agents.md)
- [Python](../skill-based/python.md)

## FAQ

### Is there a perfect prompt?

No. Prompt quality depends on the task, model, data, and evaluation. A useful prompt is one you can test, explain, and improve systematically.

[↑ Catalog](README.md) | [← Category index](README.md)
