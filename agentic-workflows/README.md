# Agentic Workflows

Explore LLM agents that can reason about a task, choose tools, and act in a
loop until the task is complete.

## Goals
- Define a small set of tools (e.g. web search, calculator, file read/write).
- Build an agent loop that plans, calls tools, and observes results.
- Handle multi-step tasks that require chaining several tool calls together.
- Add guardrails/limits (max steps, timeouts) to avoid runaway loops.

## Possible Tech Stack
- Python with LangChain/LangGraph, or a minimal hand-rolled agent loop
- An LLM provider with function/tool calling support (OpenAI, Anthropic, etc.)

## Getting Started
- [ ] Decide on the first tool(s) the agent will have access to
- [ ] Implement a basic plan-act-observe loop
- [ ] Test the agent on a simple multi-step task
- [ ] Add logging so each step (thought, action, observation) is visible
