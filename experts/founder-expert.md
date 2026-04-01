# Founder Mode

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/founder-expert.md`

**Goal:** Run your startup from your agent

**What you'll have:** Triage your inbox and investor updates via Gmail, review your engineers' PRs from the terminal, coordinate the team on Slack, keep your product roadmap in Notion, and stay on top of market signals — all from a single workflow.

---

## Step 1: Install

```bash
clawhub install openclaw/gog openclaw/github openclaw/slack openclaw/notion openclaw/summarize
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/gog

_Investor updates, customer emails, and board scheduling all live in Gmail and Calendar — your Agent handles the triage so you focus on the signal._

- Run `/gog auth` to start the Google OAuth flow
- Grant access to Gmail, Calendar, Drive, and Sheets when prompted
- Auth persists across sessions — re-run if you ever revoke access

### openclaw/github

_Stay close to the code without context switching — review PRs, check CI, and unblock engineers from the terminal._

- Authenticate with the GitHub CLI: run `gh auth login` and follow the prompts
- Choose HTTPS or SSH, then log in via browser — no extra tokens needed
- The skill uses `gh` under the hood, so all your existing GitHub access applies

### openclaw/slack

_Team standups, launch announcements, and customer escalations all happen in Slack — your Agent keeps you in the loop without reading every message._

- Create a Slack app at https://api.slack.com/apps → "Create New App" → "From scratch"
- Under "OAuth & Permissions", add bot scopes: `channels:read`, `chat:write`, `im:write`, `users:read`, `channels:history`
- Click "Install to Workspace" and copy the Bot User OAuth Token
- Set environment variable: `SLACK_BOT_TOKEN=xoxb-your-token`
- Invite the bot to the channels it needs to post in: `/invite @your-app-name`

### openclaw/notion

_Your product roadmap, hiring tracker, and OKR docs all live in Notion — your Agent keeps them up to date so you're never working from stale info._

- Go to https://www.notion.so/my-integrations → "New integration" → give it a name
- Copy the "Internal Integration Secret" (starts with `ntn_`)
- Set environment variable: `NOTION_TOKEN=ntn_your_secret`
- In each Notion page or database you want to use: click "..." → "Connect to" → select your integration

### openclaw/summarize

_Digest competitor launches, investor memos, and market reports in seconds — so you always have context, never preparation time._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/gog**

- "Draft my monthly investor update email"
- "Summarize my unread emails and flag anything from customers"
- "Schedule a board call for next week"

**openclaw/github**

- "What PRs need my review today?"
- "Is the CI passing on the release branch?"
- "Create an issue: customer reported login failure on mobile"

**openclaw/slack**

- "What's the latest in #engineering today?"
- "Post the launch announcement to #general"
- "Alert the team about the production incident"

**openclaw/notion**

- "Update the Q2 roadmap with this new priority"
- "Add this candidate to the hiring tracker"
- "Draft the Q2 OKRs in Notion"

**openclaw/summarize**

- "Summarize this competitor's product launch post"
- "TL;DR this VC memo on the AI market"
- "Digest the key trends in this industry report"

---

*Founder Mode · [clawhub.md/expert/founder-expert](https://clawhub.md/expert/founder-expert)*