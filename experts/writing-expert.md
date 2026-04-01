# Word Surgeon

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/writing-expert.md`

**Goal:** Write, document, and capture knowledge faster

**What you'll have:** Summarize sources into Obsidian notes, draft and publish to Notion, extract key insights from PDFs, and maintain a living knowledge base that grows with every article you read.

---

## Step 1: Install

```bash
clawhub install openclaw/obsidian openclaw/notion openclaw/summarize anthropics/pdf
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/obsidian

_Your second brain — search, create, and link notes in your local Obsidian vault so ideas connect across everything you've read._

- Set your vault path: add `OBSIDIAN_VAULT_PATH=/absolute/path/to/your/vault` to your environment
- No external auth needed — the skill reads and writes directly to your local vault
- Tip: use `echo $OBSIDIAN_VAULT_PATH` to verify the path is set correctly

### openclaw/notion

_Draft long-form posts, maintain a content calendar, and publish finalized pieces to your Notion workspace._

- Go to https://www.notion.so/my-integrations → "New integration" → give it a name
- Copy the "Internal Integration Secret" (starts with `ntn_`)
- Set environment variable: `NOTION_TOKEN=ntn_your_secret`
- In each Notion page or database you want to use: click "..." → "Connect to" → select your integration

### openclaw/summarize

_Turn any URL, PDF, or YouTube link into a concise summary — the fastest way to absorb sources and capture the key points worth keeping._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/obsidian**

- "Save this article summary to my Obsidian vault"
- "Search my notes for ideas about "product-led growth""
- "Create a note connecting these two concepts"

**openclaw/notion**

- "Draft a blog post about this topic in Notion"
- "Add this idea to my content calendar"
- "Publish these notes as a Notion page"

**openclaw/summarize**

- "Summarize this article and save to Obsidian"
- "TL;DR this research paper"
- "Summarize this YouTube talk into bullet points"

**anthropics/pdf**

- "Extract the key findings from this paper PDF"
- "Merge these three reference docs into one"
- "Pull the methodology section from this report"

---

*Word Surgeon · [clawhub.md/expert/writing-expert](https://clawhub.md/expert/writing-expert)*