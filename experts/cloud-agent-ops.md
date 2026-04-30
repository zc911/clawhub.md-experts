# Cloud Agent Ops

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/cloud-agent-ops.md`

**Goal:** Run agents in the cloud, not just locally

**What you'll have:** Set up Claude Code Routines that run on Anthropic infrastructure even when your computer is off, trigger Managed Agents via REST API or webhooks, and push results to Slack, GitHub, or email — cloud-native agent operations.

---

## Step 1: Install

```bash
clawhub install openclaw/cloud-routines openclaw/github openclaw/coding-agent
```

## Step 2: Try it

After setup, say these to your agent:

**openclaw/cloud-routines**

- "Set up a routine that runs tests every morning at 9am"
- "Create a webhook-triggered routine for PR auto-review"
- "Schedule a weekly report and post to Slack"

**openclaw/github**

- "Check CI status on the release branch"
- "Auto-assign reviewers when a PR is opened"
- "Create an issue from the routine output"

**openclaw/coding-agent**

- "Have the routine delegate bug fixes to a coding agent"
- "Run a background agent for the long migration script"
- "Trigger Codex from a scheduled routine"

---

*Cloud Agent Ops · [clawhub.md/expert/cloud-agent-ops](https://clawhub.md/expert/cloud-agent-ops)*