# Study Buddy

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/student-expert.md`

**Goal:** Learn and research more efficiently

**What you'll have:** Summarize papers and lectures in seconds, extract text and citations from PDFs, save insights directly to your Obsidian vault, and keep your study calendar organized via Google — all in one workflow.

---

## Step 1: Install

```bash
clawhub install openclaw/summarize openclaw/obsidian anthropics/pdf openclaw/gog
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/summarize

_Summarize academic papers, lecture videos, and reading list articles in seconds — compress hours of reading into minutes._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

### openclaw/obsidian

_Build a connected note system in your Obsidian vault — save summaries, link concepts, and search across everything you've studied._

- Set your vault path: add `OBSIDIAN_VAULT_PATH=/absolute/path/to/your/vault` to your environment
- No external auth needed — the skill reads and writes directly to your local vault
- Tip: use `echo $OBSIDIAN_VAULT_PATH` to verify the path is set correctly

### openclaw/gog

_Keep your study schedule and assignment deadlines in Google Calendar, and save research notes to Drive — the backbone of your academic workflow._

- Run `/gog auth` to start the Google OAuth flow
- Grant access to Gmail, Calendar, Drive, and Sheets when prompted
- Auth persists across sessions — re-run if you ever revoke access

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/summarize**

- "Summarize this research paper into key findings"
- "TL;DR this YouTube lecture on machine learning"
- "Give me the main argument of this article"

**openclaw/obsidian**

- "Save this paper summary to my Obsidian vault"
- "Search my notes for "transformer architecture""
- "Create a note linking these two theories"

**anthropics/pdf**

- "Extract all citations from this PDF paper"
- "Pull the abstract and conclusions from these 5 papers"
- "Merge my annotated PDFs into one document"

**openclaw/gog**

- "Add my exam dates to Google Calendar"
- "Schedule study blocks for the next two weeks"
- "Save this research summary to my Drive folder"

---

*Study Buddy · [clawhub.md/expert/student-expert](https://clawhub.md/expert/student-expert)*