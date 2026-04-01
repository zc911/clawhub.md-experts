# OSS Maintainer

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/open-source-expert.md`

**Goal:** Maintain your OSS project without burning out

**What you'll have:** Triage GitHub issues and PRs from the terminal, post release announcements to X, keep your community synced via Slack, and summarize incoming issues and discussions so you always know what the community needs.

---

## Step 1: Install

```bash
clawhub install openclaw/github openclaw/xurl openclaw/slack openclaw/summarize
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/github

_Triage issues, review community PRs, check CI on contributor branches, and create release issues — the core of OSS maintenance._

- Authenticate with the GitHub CLI: run `gh auth login` and follow the prompts
- Choose HTTPS or SSH, then log in via browser — no extra tokens needed
- The skill uses `gh` under the hood, so all your existing GitHub access applies

### openclaw/xurl

_Announce releases, engage with users who mention your project, and share what the community is building — social visibility for OSS._

- Apply for an X Developer account at https://developer.twitter.com (free tier is sufficient)
- Create a project and app, then generate API Key, API Secret, Access Token, and Access Token Secret with Read+Write permissions
- Set four environment variables: `X_API_KEY`, `X_API_SECRET`, `X_ACCESS_TOKEN`, `X_ACCESS_TOKEN_SECRET`

### openclaw/slack

_Keep your contributor community engaged in Slack — share roadmap updates, answer questions, and announce breaking changes before they hit._

- Create a Slack app at https://api.slack.com/apps → "Create New App" → "From scratch"
- Under "OAuth & Permissions", add bot scopes: `channels:read`, `chat:write`, `im:write`, `users:read`, `channels:history`
- Click "Install to Workspace" and copy the Bot User OAuth Token
- Set environment variable: `SLACK_BOT_TOKEN=xoxb-your-token`
- Invite the bot to the channels it needs to post in: `/invite @your-app-name`

### openclaw/summarize

_Summarize long issue threads, PRs with 50+ comments, and community discussions so you can respond with context — not noise._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/github**

- "List all open issues with more than 5 thumbs-up"
- "Review this community PR for quality"
- "Create a release checklist issue for v2.0"

**openclaw/xurl**

- "Post the v2.0 release announcement thread"
- "Check X for mentions of my project this week"
- "Search for users asking questions about this library"

**openclaw/slack**

- "Post the release notes to #announcements"
- "What are contributors discussing in #contributors today?"
- "Announce the breaking change to #general"

**openclaw/summarize**

- "Summarize this 80-comment issue thread"
- "TL;DR this PR discussion and tell me the sticking point"
- "What are the top 5 feature requests from issues this month?"

---

*OSS Maintainer · [clawhub.md/expert/open-source-expert](https://clawhub.md/expert/open-source-expert)*