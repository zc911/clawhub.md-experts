# Morning Intel

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/daily-briefing.md`

**Goal:** Start your day in 30 seconds

**What you'll have:** One command. Today's weather, inbox highlights, and what's on your calendar — so you know what matters before the day starts.

---

## Step 1: Install

```bash
clawhub install openclaw/gog openclaw/weather openclaw/summarize
```

## Step 2: Configure

Each skill may need credentials or auth before it can act on your behalf.

### openclaw/gog

_Pull urgent emails and check today's calendar — get the full picture of your day without opening Gmail._

- Run `/gog auth` to start the Google OAuth flow
- Grant access to Gmail, Calendar, Drive, and Sheets when prompted
- Auth persists across sessions — re-run if you ever revoke access

### openclaw/weather

_Get the weather for your location so you can plan your day — commute, lunch, travel, whatever._

- No configuration needed — uses public APIs (wttr.in and Open-Meteo)
- Works immediately after install

### openclaw/summarize

_TL;DR a long email thread, article, or doc when you only have 2 minutes to get up to speed._

- No external accounts or API keys needed
- Works immediately after install — paste any URL, file path, or YouTube link

## Step 3: Try it

After setup, say these to your agent to verify everything works:

**openclaw/gog**

- "What's urgent in my inbox today?"
- "What meetings do I have this afternoon?"
- "Any emails from my team since yesterday?"

**openclaw/weather**

- "What's the weather today in my city?"
- "Will it rain this afternoon in London?"
- "5-day forecast for this week"

**openclaw/summarize**

- "TL;DR the last 5 emails in this thread"
- "Summarize this article before my 9am"
- "Give me the key points from this document"

---

*Morning Intel · [clawhub.md/expert/daily-briefing](https://clawhub.md/expert/daily-briefing)*