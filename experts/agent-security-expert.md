# Agent Sentinel

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/agent-security-expert.md`

**Goal:** Secure your agents before they go to production

**What you'll have:** Configure sandbox boundaries, detect indirect prompt injections, enforce permission allow/deny lists, and add human-in-the-loop approval for sensitive operations — so your agents are safe to run in production.

---

## Step 1: Install

```bash
clawhub install openclaw/agent-guard anthropics/mcp-builder openclaw/coding-agent
```

## Step 2: Try it

After setup, say these to your agent:

**openclaw/agent-guard**

- "Set up permission boundaries for my agent"
- "Block my agent from running sudo or rm -rf"
- "Scan this URL for indirect prompt injection"

**anthropics/mcp-builder**

- "Build an MCP server with scoped read-only access"
- "Add authentication to my existing MCP server"
- "Audit my MCP server for excessive permissions"

**openclaw/coding-agent**

- "Delegate security test generation to Claude Code"
- "Have Codex scan this codebase for injection vulnerabilities"
- "Run OWASP compliance checks in a background agent"

---

*Agent Sentinel · [clawhub.md/expert/agent-security-expert](https://clawhub.md/expert/agent-security-expert)*