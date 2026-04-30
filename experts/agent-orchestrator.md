# Agent Orchestrator

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/agent-orchestrator.md`

**Goal:** Orchestrate agents that talk to each other

**What you'll have:** Design multi-agent architectures where agents discover each other via A2A Agent Cards, communicate through standard protocols, and build on MCP for tool integration — the full stack for agent-to-agent collaboration.

---

## Step 1: Install

```bash
clawhub install openclaw/a2a anthropics/mcp-builder openclaw/coding-agent
```

## Step 2: Try it

After setup, say these to your agent:

**openclaw/a2a**

- "Create an Agent Card for my research agent"
- "Discover agents that can handle PDF analysis"
- "Send a long-running task to another agent with streaming"

**anthropics/mcp-builder**

- "Build an MCP server for my REST API"
- "Add a database read tool to my MCP server"
- "Create an MCP server from scratch"

**openclaw/coding-agent**

- "Delegate the MCP server boilerplate to a coding agent"
- "Have Codex scaffold the A2A transport layer"
- "Run this integration test in a background agent"

---

*Agent Orchestrator · [clawhub.md/expert/agent-orchestrator](https://clawhub.md/expert/agent-orchestrator)*