---
title: AI Agents Roadmap
---

# AI Agents

Build systems where a model can choose tools and take steps toward a goal—without giving up control.

[← AI roadmaps](README.md) | [All roadmaps](../README.md)

## Start here

- [ ] Build a single-tool agent with an explicit stop condition
- [ ] Log every model decision and tool result
- [ ] Add input validation and a timeout
- [ ] Test one successful and one failing run

## Learning stages

### 1. Agent fundamentals

- The difference between a workflow and an open-ended agent
- The model–tool loop: decide, act, observe, repeat
- Tool schemas and clear tool descriptions
- State, memory, and conversation context
- Stop conditions, iteration limits, and recovery
- When a deterministic workflow is a better choice

**Build:** a research helper that searches one approved source and summarizes the result.

### 2. Tools and actions

- Separate read-only tools from tools with side effects
- Validate tool arguments before execution
- Return compact, useful observations to the model
- Handle partial failure and retries
- Require confirmation for irreversible actions
- Apply least-privilege credentials per tool

**Build:** a note-taking agent that proposes changes but requires user confirmation before writing.

### 3. Reliable execution

- Timeouts and cancellation
- Idempotency keys and duplicate protection
- Loop detection and budget limits
- Parallel tool calls and dependency ordering
- Human-in-the-loop checkpoints
- Long-running jobs and resumable state

**Build:** an agent that can recover after a failed tool call without repeating a completed side effect.

### 4. Evaluation and observability

- Task-level end-to-end tests
- Trajectory review: not just the answer, but how it was reached
- Error categories: retrieval, tool choice, arguments, and reasoning
- Cost and latency per run
- Traces spanning model calls, retrieval, and tools
- Regression tests for security and privacy behavior

**Build:** a test suite that checks both the final result and the required tool actions for representative tasks.

### 5. Safety and operations

- Prompt injection through web pages, files, and tool output
- Data exfiltration and permission boundaries
- Destructive actions and approval gates
- Secrets isolation and sandboxed execution
- Abuse monitoring, kill switches, and rate limits
- Incident response and user transparency

**Build:** write a threat model and implement a kill switch, an action allow-list, and a confirmation step for one sensitive tool.

## Definition of done

You can build an agent with bounded authority, traceable decisions, repeatable evaluation, and safe failure behavior—and explain why an agent is preferable to a fixed workflow.

## Related roadmaps

- [AI engineer](../role-based/ai-engineer.md)
- [Prompt engineering](prompt-engineering.md)
- [Backend developer](../role-based/backend-developer.md)

## FAQ

### Does every AI product need an agent?

No. Most tasks are better served by predictable workflows. Use an agent when the task genuinely requires choosing among tools or adapting a plan to intermediate results.

[↑ Catalog](README.md) | [← Category index](README.md)
