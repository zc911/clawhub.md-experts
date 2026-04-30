# Self-Driving Dev

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/self-driving-dev.md`

**Goal:** Run multiple agents in parallel across IDEs

**What you'll have:** Run parallel git worktrees with Cursor SDK, Windsurf+Devin, and Claude Code simultaneously — local agents for fast iteration, cloud agents for long-running tasks, adaptive model routing for optimal results per task type.

---

## Step 1: Install

```bash
clawhub install openclaw/cursor-sdk openclaw/github openclaw/coding-agent
```

## Step 2: Try it

After setup, say these to your agent:

**openclaw/cursor-sdk**

- "Set up parallel worktrees for frontend, backend, and tests"
- "Configure Windsurf Devin for cloud-based debugging"
- "Route code review tasks to the strongest model"

**openclaw/github**

- "Check CI status across all my worktrees"
- "Create a PR from the frontend worktree"
- "Review PRs while the backend agent is still running"

**openclaw/coding-agent**

- "Delegate the API migration to a background coding agent"
- "Have Codex write tests for all three worktrees"
- "Run this refactor in a parallel Claude Code session"

---

*Self-Driving Dev · [clawhub.md/expert/self-driving-dev](https://clawhub.md/expert/self-driving-dev)*