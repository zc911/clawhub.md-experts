# Solo Founder Dev

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/indie-dev-expert.md`

**Goal:** Build, ship, and grow as a solo developer

**What you'll have:** Manage GitHub from the terminal, delegate boilerplate and tests to a coding agent, announce releases on X to build an audience, and package your best workflows into reusable skills — so each project makes you faster than the last.

---

## Step 1: Install

```bash
clawhub install openclaw/github openclaw/coding-agent openclaw/xurl anthropics/skill-creator
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/github

_Manage PRs, Issues, and CI from the terminal — stay close to the code without context switching._

- Authenticate with the GitHub CLI: run `gh auth login` and follow the prompts
- Choose HTTPS or SSH, then log in via browser — no extra tokens needed
- The skill uses `gh` under the hood, so all your existing GitHub access applies

### openclaw/coding-agent

_Delegate test generation, boilerplate, and repetitive refactors to Claude Code or Codex — stay in flow on the parts only you can do._

- Ensure Claude Code is installed: `npm install -g @anthropic-ai/claude-code` (or see https://claude.ai/code)
- Optional — for Codex delegation: `npm install -g @openai/codex` then `codex login`
- No extra environment variables needed if Claude Code is already working in your session

### openclaw/xurl

_Announce releases, share what you're building, and engage with users who reply — building in public is how indie devs grow._

- Apply for an X Developer account at https://developer.twitter.com (free tier is sufficient)
- Create a project and app, then generate API Key, API Secret, Access Token, and Access Token Secret with Read+Write permissions
- Set four environment variables: `X_API_KEY`, `X_API_SECRET`, `X_ACCESS_TOKEN`, `X_ACCESS_TOKEN_SECRET`

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/github**

- "List my open PRs and flag anything blocking"
- "What's the CI status on my current branch?"
- "Create an issue for the bug I just found"

**openclaw/coding-agent**

- "Delegate writing tests for this module to Claude Code"
- "Have Codex scaffold the API routes for this feature"
- "Run this refactor in a background agent"

**openclaw/xurl**

- "Post the v1.0 launch announcement"
- "Check my X mentions since yesterday"
- "Search for people asking about this type of tool"

**anthropics/skill-creator**

- "Package this deploy workflow as a reusable skill"
- "Create a skill that automates my release checklist"
- "Audit my SKILL.md for best practices"

---

*Solo Founder Dev · [clawhub.md/expert/indie-dev-expert](https://clawhub.md/expert/indie-dev-expert)*