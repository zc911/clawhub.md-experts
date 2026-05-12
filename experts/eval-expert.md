# AI Eval Engineer

> **Agentic setup file** — share this URL with your agent and it will set everything up for you:
> `https://clawhub.md/expert/eval-expert.md`

**Goal:** Measure and improve AI quality

**What you'll have:** Build eval suites that catch regressions before users do. Write LLM-as-judge evaluators, create golden datasets, run CI evals on every model change, and track quality metrics over time. Turn 'it feels worse' into a reproducible test.

---

## Step 1: Install

```bash
clawhub install anthropics/claude-api openclaw/coding-agent openclaw/github
```

## Step 2: Try it

After setup, say these to your agent:

**anthropics/claude-api**

- "Write a Claude-as-judge evaluator for my chatbot"
- "Compare my current prompt vs a new version on 50 test cases"
- "Build an eval that detects hallucinations in my RAG pipeline"

**openclaw/coding-agent**

- "Scaffold a pytest eval suite for my LLM app"
- "Generate 100 diverse test cases from my production logs"
- "Wire evals into my GitHub Actions CI"

**openclaw/github**

- "Post eval score diff as a PR comment"
- "Block merge if eval score drops below threshold"
- "List all eval regressions since the last release"

---

*AI Eval Engineer · [clawhub.md/expert/eval-expert](https://clawhub.md/expert/eval-expert)*