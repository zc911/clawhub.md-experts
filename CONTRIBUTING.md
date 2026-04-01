# Contributing to clawhub/experts

This repo is the community library for [clawhub.md](https://clawhub.md) experts.

An **Expert** is a curated set of skills built around a real workflow.
When someone says "set me up as [Expert Name]" to their agent, it installs everything and configures it — in one step.

## How to add an Expert

1. Fork this repo
2. Create `experts/your-expert-slug.json` (see format below)
3. Open a PR with a short description of the workflow it serves

Your expert goes live on clawhub.md as soon as the PR is merged.

## Expert format

```json
{
  "slug": "your-expert-slug",
  "name": { "en": "Your Expert Name", "zh": "中文名（可选）" },
  "description": {
    "en": "One line — what does this expert help you do?",
    "zh": "中文描述（可选）"
  },
  "goal": { "en": "Short action phrase", "zh": "中文（可选）" },
  "outcome": {
    "en": "After installing, your agent can... (2-3 sentences max)",
    "zh": "中文（可选）"
  },
  "division": "Engineering",
  "skillsWithReason": [
    {
      "slug": "namespace/skill-name",
      "reason": {
        "en": "Why this skill is included in this expert.",
        "zh": "中文（可选）"
      },
      "order": 1,
      "examples": {
        "en": ["Say this to your agent", "Or this"],
        "zh": ["中文示例（可选）"]
      }
    }
  ],
  "installAll": "clawhub install namespace/skill-name",
  "curator": "your-github-username",
  "created": "2026-04-01"
}
```

### `division` options

| Value | Use for |
|-------|---------|
| `Engineering` | Dev tools, coding, infra, open source |
| `Product` | PM, founder, strategy |
| `Content` | Writing, social, creator workflows |
| `Productivity` | Personal tools, research, meetings, daily routines |
| `中文专区` | China-market tools (Feishu, DingTalk, WeCom, etc.) |

### Rules

- **Only reference skills that exist** in the [clawhub skill registry](https://clawhub.md/browse)
- **`outcome` must be concrete** — say what the agent can actually do, not vague aspirations
- **`examples` must be real prompts** you'd actually say to your agent
- **`description` max 80 characters** — it appears in the card on the experts list
- **One workflow per expert** — if it spans 3 unrelated domains, split it

## Questions?

Open an issue or find us on [X](https://x.com/clawhubmd).
