# Dev Assistant (Chinese Teams)

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/dev-expert-cn.md`

**Goal:** Boost dev team productivity

**What you'll have:** Manage GitHub PRs and Issues with your Agent, sync progress to Feishu, and delegate repetitive coding tasks to AI — all without leaving the terminal.

---

## Step 1: Install

```bash
clawhub install openclaw/github openclaw/feishu openclaw/coding-agent
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/github

_Review PRs, handle Issues, and check CI status via the gh CLI — no browser needed._

- Authenticate with the GitHub CLI: run `gh auth login` and follow the prompts
- Choose HTTPS or SSH, then log in via browser — no extra tokens needed
- The skill uses `gh` under the hood, so all your existing GitHub access applies

### openclaw/coding-agent

_Delegate refactors, code reviews, and migration scripts to a coding agent so you can focus on what matters._

- Ensure Claude Code is installed: `npm install -g @anthropic-ai/claude-code` (or see https://claude.ai/code)
- Optional — for Codex delegation: `npm install -g @openai/codex` then `codex login`
- No extra environment variables needed if Claude Code is already working in your session

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/github**

- "Check if any of my PRs need attention"
- "Create an issue: login page crashes on Safari"
- "What's the CI status on my current branch?"

**openclaw/feishu**

- "Post the PR merge notification to the #engineering Feishu group"
- "What Feishu messages are related to development today?"

**openclaw/coding-agent**

- "Hand this refactor off to a coding agent"
- "Have Codex check this function for edge cases"

---

*Dev Assistant (Chinese Teams) · [clawhub.md/expert/dev-expert-cn](https://clawhub.md/expert/dev-expert-cn)*