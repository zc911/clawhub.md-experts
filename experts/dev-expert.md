# Ship Expert

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/dev-expert.md`

**Goal:** Code, review & ship faster

**What you'll have:** Manage your GitHub workflow and delegate coding tasks to AI agents — all from your agent, with no context switching.

---

## Step 1: Install

```bash
clawhub install openclaw/github openclaw/coding-agent
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/github

_Review open PRs, triage issues, check CI status, and create new issues — all via the gh CLI without opening a browser._

- Authenticate with the GitHub CLI: run `gh auth login` and follow the prompts
- Choose HTTPS or SSH, then log in via browser — no extra tokens needed
- The skill uses `gh` under the hood, so all your existing GitHub access applies

### openclaw/coding-agent

_Delegate a refactor, background task, or code review to Claude Code or Codex while you stay focused on the bigger picture._

- Ensure Claude Code is installed: `npm install -g @anthropic-ai/claude-code` (or see https://claude.ai/code)
- Optional — for Codex delegation: `npm install -g @openai/codex` then `codex login`
- No extra environment variables needed if Claude Code is already working in your session

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/github**

- "Review my open PRs for anything blocking"
- "Create an issue: login page crashes on Safari"
- "What's the CI status on my current branch?"

**openclaw/coding-agent**

- "Delegate this refactor to a coding agent"
- "Have Codex review this function for edge cases"
- "Run this migration script in a background agent"

---

*Ship Expert · [clawhub.md/expert/dev-expert](https://clawhub.md/expert/dev-expert)*