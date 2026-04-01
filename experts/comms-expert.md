# Inbox Zero

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/comms-expert.md`

**Goal:** Manage email & comms

**What you'll have:** Control Gmail, Slack, and X from your agent — read, send, and organize without switching apps.

---

## Step 1: Install

```bash
clawhub install openclaw/gog openclaw/slack openclaw/xurl
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/gog

_Read, send, and organize Gmail. Check your calendar, share Drive files, and update Sheets — all from your agent._

- Run `/gog auth` to start the Google OAuth flow
- Grant access to Gmail, Calendar, Drive, and Sheets when prompted
- Auth persists across sessions — re-run if you ever revoke access

### openclaw/slack

_Post to channels, read threads, and manage your Slack workspace directly from the terminal._

- Create a Slack app at https://api.slack.com/apps → "Create New App" → "From scratch"
- Under "OAuth & Permissions", add bot scopes: `channels:read`, `chat:write`, `im:write`, `users:read`, `channels:history`
- Click "Install to Workspace" and copy the Bot User OAuth Token
- Set environment variable: `SLACK_BOT_TOKEN=xoxb-your-token`
- Invite the bot to the channels it needs to post in: `/invite @your-app-name`

### openclaw/xurl

_Monitor X (Twitter) mentions, post updates, and search trends via the authenticated API._

- Apply for an X Developer account at https://developer.twitter.com (free tier is sufficient)
- Create a project and app, then generate API Key, API Secret, Access Token, and Access Token Secret with Read+Write permissions
- Set four environment variables: `X_API_KEY`, `X_API_SECRET`, `X_ACCESS_TOKEN`, `X_ACCESS_TOKEN_SECRET`

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/gog**

- "Check my inbox for anything urgent"
- "Schedule a meeting tomorrow at 2pm with Alice"
- "Share this file with my team on Drive"

**openclaw/slack**

- "Post to #general: deployment is live"
- "What's new in #engineering today?"
- "Send a DM to Alice about the PR"

**openclaw/xurl**

- "Check my X mentions from today"
- "Post a tweet: just shipped v2.0"
- "Search X for "openclaw" trends"

---

*Inbox Zero · [clawhub.md/expert/comms-expert](https://clawhub.md/expert/comms-expert)*