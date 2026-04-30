# Agent Builder

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/ai-builder-expert.md`

**Goal:** Build and ship AI agents end to end

**What you'll have:** Scaffold Claude API apps with the Agent SDK (Python/TS), build MCP servers that give LLMs new tools, add A2A protocol for agent-to-agent communication, publish skills to the Claude Code marketplace, and delegate coding to agents — the full agent builder stack.

---

## Step 1: Install

```bash
clawhub install anthropics/claude-api anthropics/mcp-builder openclaw/a2a anthropics/skill-creator openclaw/coding-agent
```

## Step 2: Try it

After setup, say these to your agent:

**anthropics/claude-api**

- "Build an agent with the Claude Agent SDK"
- "Add tool use and structured output to my agent"
- "Set up subagents for parallel task execution"

**anthropics/mcp-builder**

- "Build an MCP server for my REST API"
- "Add Elicitation support for user prompts"
- "Create a new MCP server with TypeScript SDK"

**openclaw/a2a**

- "Generate an Agent Card for my agent"
- "Add A2A skill discovery to my agent"
- "Set up task streaming between my agent and others"

**anthropics/skill-creator**

- "Package this agent as a publishable skill"
- "Audit my SKILL.md for marketplace requirements"
- "Create a namespaced plugin for the Claude Code marketplace"

**openclaw/coding-agent**

- "Delegate writing tests for this module to an agent"
- "Have Claude Code scaffold the boilerplate for this feature"

---

*Agent Builder · [clawhub.md/expert/ai-builder-expert](https://clawhub.md/expert/ai-builder-expert)*