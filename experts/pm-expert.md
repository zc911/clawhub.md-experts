# Product Mind

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/pm-expert.md`

**Goal:** Stay on top of product and stakeholder work

**What you'll have:** Draft PRDs and specs in Notion, summarize meeting outputs, keep your inbox under control, and coordinate with engineering and design via Slack — without context switching.

---

## Step 1: Install

```bash
clawhub install openclaw/gog openclaw/notion openclaw/slack openclaw/summarize
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/gog

_Manage your Gmail inbox, schedule stakeholder syncs on Google Calendar, and pull research from Drive — the core communication layer for most PMs._

- Run `/gog auth` to start the Google OAuth flow
- Grant access to Gmail, Calendar, Drive, and Sheets when prompted
- Auth persists across sessions — re-run if you ever revoke access

### openclaw/notion

_Write PRDs, track feature decisions, and maintain your product wiki — Notion is where PM work lives._

- Go to https://www.notion.so/my-integrations → "New integration" → give it a name
- Copy the "Internal Integration Secret" (starts with `ntn_`)
- Set environment variable: `NOTION_TOKEN=ntn_your_secret`
- In each Notion page or database you want to use: click "..." → "Connect to" → select your integration

### openclaw/slack

_Post sprint updates, coordinate cross-functional work, and stay on top of engineering blockers — Slack is where the real-time product work happens._

- Create a Slack app at https://api.slack.com/apps → "Create New App" → "From scratch"
- Under "OAuth & Permissions", add bot scopes: `channels:read`, `chat:write`, `im:write`, `users:read`, `channels:history`
- Click "Install to Workspace" and copy the Bot User OAuth Token
- Set environment variable: `SLACK_BOT_TOKEN=xoxb-your-token`
- Invite the bot to the channels it needs to post in: `/invite @your-app-name`

### openclaw/summarize

_Digest competitor articles, user research reports, and long design docs in seconds — so you always have context before any meeting._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/gog**

- "Summarize my unread emails and flag anything urgent"
- "Schedule a 30-min sync with the eng team tomorrow"
- "Find the Q2 roadmap doc in my Drive"

**openclaw/notion**

- "Draft a PRD for this feature in Notion"
- "Add these meeting decisions to the product wiki"
- "Create a new spec page for the onboarding redesign"

**openclaw/slack**

- "Post this week's sprint update to #product"
- "What are the current engineering blockers in #eng?"
- "DM the design lead about the deadline change"

**openclaw/summarize**

- "Summarize this user research report"
- "TL;DR this competitor product announcement"
- "Digest the key points of this 50-page spec"

---

*Product Mind · [clawhub.md/expert/pm-expert](https://clawhub.md/expert/pm-expert)*