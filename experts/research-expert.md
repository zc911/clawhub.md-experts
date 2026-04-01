# Deep Dive

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/research-expert.md`

**Goal:** Research & take notes

**What you'll have:** Summarize any URL, PDF, or video and save the insights to Obsidian or Notion — in seconds.

---

## Step 1: Install

```bash
clawhub install openclaw/summarize openclaw/obsidian openclaw/notion
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/summarize

_Paste a URL, file, or YouTube link — get a clean summary in seconds._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

### openclaw/obsidian

_Save summaries and notes directly into your Obsidian vault with automatic linking._

- Set your vault path: add `OBSIDIAN_VAULT_PATH=/absolute/path/to/your/vault` to your environment
- No external auth needed — the skill reads and writes directly to your local vault
- Tip: use `echo $OBSIDIAN_VAULT_PATH` to verify the path is set correctly

### openclaw/notion

_Alternatively, push research notes into Notion pages or databases._

- Go to https://www.notion.so/my-integrations → "New integration" → give it a name
- Copy the "Internal Integration Secret" (starts with `ntn_`)
- Set environment variable: `NOTION_TOKEN=ntn_your_secret`
- In each Notion page or database you want to use: click "..." → "Connect to" → select your integration

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/summarize**

- "Summarize this URL: https://..."
- "TL;DR this PDF"
- "Summarize this YouTube video"

**openclaw/obsidian**

- "Save this summary to my Obsidian vault"
- "Create a note about today's meeting"
- "Add this to my research folder in Obsidian"

**openclaw/notion**

- "Add this to my Notion research database"
- "Create a Notion page with these notes"
- "Update my reading list in Notion"

---

*Deep Dive · [clawhub.md/expert/research-expert](https://clawhub.md/expert/research-expert)*