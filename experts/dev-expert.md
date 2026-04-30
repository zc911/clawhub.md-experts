# Ship Expert

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/dev-expert.md`

**Goal:** Code, review & ship faster

**What you'll have:** Manage your GitHub workflow, delegate coding tasks to AI agents, run scheduled Routines in the cloud, and use worktree parallelism to ship multiple features at once — all from your agent, with no context switching.

---

## Step 1: Install

```bash
clawhub install openclaw/github openclaw/coding-agent openclaw/cloud-routines
```

## Step 2: Try it

After setup, say these to your agent:

**openclaw/github**

- "Review my open PRs for anything blocking"
- "Create an issue: login page crashes on Safari"
- "What's the CI status on my current branch?"

**openclaw/coding-agent**

- "Delegate this refactor to a coding agent"
- "Have Codex review this function for edge cases"
- "Run this migration script in a background agent"

**openclaw/cloud-routines**

- "Set up a routine that runs tests when a PR is opened"
- "Schedule a nightly build and deploy routine"
- "Auto-assign reviewers via a cloud routine"

---

*Ship Expert · [clawhub.md/expert/dev-expert](https://clawhub.md/expert/dev-expert)*