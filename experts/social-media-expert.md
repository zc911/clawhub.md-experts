# Growth Hacker

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/social-media-expert.md`

**Goal:** Grow and engage your social presence

**What you'll have:** Summarize industry news into post ideas, publish to X with proper formatting, monitor mentions and trending topics, and coordinate team announcements via Slack — all without context switching.

---

## Step 1: Install

```bash
clawhub install openclaw/xurl openclaw/summarize openclaw/slack
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/xurl

_Post, search, and monitor X from your agent — check mentions, find trending topics, and publish without opening the app._

- Apply for an X Developer account at https://developer.twitter.com (free tier is sufficient)
- Create a project and app, then generate API Key, API Secret, Access Token, and Access Token Secret with Read+Write permissions
- Set four environment variables: `X_API_KEY`, `X_API_SECRET`, `X_ACCESS_TOKEN`, `X_ACCESS_TOKEN_SECRET`

### openclaw/summarize

_Turn articles, threads, and YouTube talks into tight post-ready summaries — so you always have something worth sharing._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

### openclaw/slack

_Coordinate launches, get copy approvals, and sync the team on what's going live — Slack keeps everyone aligned before you post._

- Create a Slack app at https://api.slack.com/apps → "Create New App" → "From scratch"
- Under "OAuth & Permissions", add bot scopes: `channels:read`, `chat:write`, `im:write`, `users:read`, `channels:history`
- Click "Install to Workspace" and copy the Bot User OAuth Token
- Set environment variable: `SLACK_BOT_TOKEN=xoxb-your-token`
- Invite the bot to the channels it needs to post in: `/invite @your-app-name`

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/xurl**

- "Post: just shipped v2.0 — here's what changed"
- "Check my X mentions from the past 24 hours"
- "Search X for "Claude Code" discussions today"

**openclaw/summarize**

- "Summarize this article into a tweet thread idea"
- "Give me 3 post angles from this research paper"
- "TL;DR this product launch for a social post"

**openclaw/slack**

- "Post the launch announcement draft to #marketing for review"
- "What did the team decide about the campaign in #marketing?"
- "Remind the team in #social to engage with today's post"

---

*Growth Hacker · [clawhub.md/expert/social-media-expert](https://clawhub.md/expert/social-media-expert)*