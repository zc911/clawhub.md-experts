# Content Machine

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/creator-expert.md`

**Goal:** Write, publish & grow an audience

**What you'll have:** Summarize source material, draft in Notion, publish to X, and track engagement — without switching between five different apps.

---

## Step 1: Install

```bash
clawhub install openclaw/summarize openclaw/notion openclaw/xurl
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/summarize

_Quickly digest articles, papers, and videos to extract the ideas worth writing about._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

### openclaw/notion

_Draft and organize your content in Notion — keep a writing queue, outline posts, and store your ideas in one place._

- Go to https://www.notion.so/my-integrations → "New integration" → give it a name
- Copy the "Internal Integration Secret" (starts with `ntn_`)
- Set environment variable: `NOTION_TOKEN=ntn_your_secret`
- In each Notion page or database you want to use: click "..." → "Connect to" → select your integration

### openclaw/xurl

_Publish threads, check mentions, and monitor how your posts are doing — without opening the app._

- Apply for an X Developer account at https://developer.twitter.com (free tier is sufficient)
- Create a project and app, then generate API Key, API Secret, Access Token, and Access Token Secret with Read+Write permissions
- Set four environment variables: `X_API_KEY`, `X_API_SECRET`, `X_ACCESS_TOKEN`, `X_ACCESS_TOKEN_SECRET`

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/summarize**

- "Summarize this article into key points I can write about"
- "TL;DR this research paper in plain English"
- "What are the most interesting ideas in this YouTube talk?"

**openclaw/notion**

- "Create a Notion draft for a post about AI agents"
- "Add this idea to my content queue in Notion"
- "What's in my writing backlog?"

**openclaw/xurl**

- "Post this thread to X"
- "Check my mentions and replies from today"
- "What's my most-engaged post this week?"

---

*Content Machine · [clawhub.md/expert/creator-expert](https://clawhub.md/expert/creator-expert)*