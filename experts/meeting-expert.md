# Meeting Ninja

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/meeting-expert.md`

**Goal:** Prep & follow up on meetings

**What you'll have:** Brief before every call, clean notes after. Your agent pulls the context, captures decisions, and sends the follow-ups — so you can focus on the conversation.

---

## Step 1: Install

```bash
clawhub install openclaw/gog openclaw/summarize openclaw/notion
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/gog

_Check your calendar for upcoming meetings, pull relevant emails for context, and send follow-up emails when the call is done._

- Run `/gog auth` to start the Google OAuth flow
- Grant access to Gmail, Calendar, Drive, and Sheets when prompted
- Auth persists across sessions — re-run if you ever revoke access

### openclaw/summarize

_Summarize a doc, slide deck, or past meeting recording before the call so you're never walking in cold._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

### openclaw/notion

_Store meeting notes, decisions, and action items in Notion so nothing gets lost after the call._

- Go to https://www.notion.so/my-integrations → "New integration" → give it a name
- Copy the "Internal Integration Secret" (starts with `ntn_`)
- Set environment variable: `NOTION_TOKEN=ntn_your_secret`
- In each Notion page or database you want to use: click "..." → "Connect to" → select your integration

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/gog**

- "What meetings do I have today?"
- "Pull emails from Alice about the Q2 project"
- "Send a follow-up to everyone on today's 3pm call"

**openclaw/summarize**

- "Summarize this proposal PDF before my 2pm"
- "TL;DR the last 3 emails in this thread"
- "Summarize the recording from last week's kickoff"

**openclaw/notion**

- "Create a meeting note in Notion for today's standup"
- "Add these action items to my Notion tasks"
- "Log the decisions from this call to the project page"

---

*Meeting Ninja · [clawhub.md/expert/meeting-expert](https://clawhub.md/expert/meeting-expert)*