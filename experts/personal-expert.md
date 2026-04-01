# Life Admin

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/personal-expert.md`

**Goal:** Own your day and capture everything

**What you'll have:** Start every morning with a Gmail digest and calendar briefing, check the weather before you commit to plans, capture stray ideas directly into your Obsidian vault, and discover new skills to extend your Agent as your needs evolve.

---

## Step 1: Install

```bash
clawhub install openclaw/gog openclaw/weather openclaw/obsidian openclaw/clawhub
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/gog

_Your day starts with email and calendar — let your Agent triage the inbox, flag what needs a response, and surface what's on your schedule._

- Run `/gog auth` to start the Google OAuth flow
- Grant access to Gmail, Calendar, Drive, and Sheets when prompted
- Auth persists across sessions — re-run if you ever revoke access

### openclaw/weather

_Check the forecast before you plan outdoor activities, commute decisions, or travel — no app-switching needed._

- No configuration needed — uses public APIs (wttr.in and Open-Meteo)
- Works immediately after install

### openclaw/obsidian

_Capture every idea, bookmark, and stray thought directly into your Obsidian vault — before it slips away._

- Set your vault path: add `OBSIDIAN_VAULT_PATH=/absolute/path/to/your/vault` to your environment
- No external auth needed — the skill reads and writes directly to your local vault
- Tip: use `echo $OBSIDIAN_VAULT_PATH` to verify the path is set correctly

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/gog**

- "Give me my morning briefing: emails + calendar"
- "Flag any emails that need a reply today"
- "What's on my calendar this week?"

**openclaw/weather**

- "What's the weather this weekend?"
- "Will it rain during my commute tomorrow?"
- "7-day forecast for my city"

**openclaw/obsidian**

- "Save this idea to my Obsidian vault"
- "Search my notes for the book recommendation I saved last week"
- "Create a note: things to do before the move"

**openclaw/clawhub**

- "Search clawhub for a skill that can read Slack"
- "Install the gog skill for Google Workspace"
- "What skills are trending on clawhub this week?"

---

*Life Admin · [clawhub.md/expert/personal-expert](https://clawhub.md/expert/personal-expert)*