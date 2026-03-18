# 📡 Content Research Workflow

> AI-powered research-to-content pipeline — turning trend signals into ready-to-produce YouTube Shorts and TikTok content

[![Live System](https://img.shields.io/badge/System-Live-10b981?style=for-the-badge)](https://roccopaz.github.io)
[![Built with Claude](https://img.shields.io/badge/Built_with-Claude_AI-8b5cf6?style=for-the-badge)](https://anthropic.com)
[![OpenClaw](https://img.shields.io/badge/Orchestrated_by-OpenClaw-3b82f6?style=for-the-badge)](https://roccopaz.github.io)

---

## 🎯 Overview

A production multi-agent AI workflow that automates the full research → content pipeline for a short-form social media channel. Two specialized AI agents collaborate daily — one handling trend intelligence, the other converting research into content concepts.

**The system turns:**
- Trend signals & viral patterns
- Famous speeches & quotes
- Athlete / artist moments
- Cultural topics with high resonance

**Into:**
- Ranked content opportunities
- Ready-to-produce short-form concepts
- Hooks, captions, and edit direction
- A weekly production backlog

---

## 🤖 Agent Architecture

### Robo 🤖 — Research Agent
Responsible for all trend discovery and intelligence gathering.

**Daily output:** Trend Pulse — 3 rising themes, top angles, competitor observations, handoff to Star
**Weekly output:** Trend Memo — pattern analysis, backlog updates, strategic direction

Core question: *What is winning right now that fits the channel?*

### Star ⭐ — Content Agent
Responsible for converting research into production-ready content.

**Daily output:** Content Pack — ranked concepts from Robo's brief
**Weekly output:** Content Slate — 10 prioritized concepts across Immediate / Weekly / Evergreen buckets

Core question: *How do we turn this into content people will actually watch and share?*

---

## 📱 Channel

This workflow powers content for:

[![TikTok](https://img.shields.io/badge/TikTok-@techmotivates-ff0050?style=for-the-badge&logo=tiktok&logoColor=white)](https://www.tiktok.com/@techmotivates)

---

## 🔄 Daily Workflow

```
08:00 AM CST — Robo runs Daily Trend Pulse
    ↓
Robo publishes brief to Discord (trending themes, best angles, handoff)
    ↓
08:15 AM CST — Star picks up brief
    ↓
Star publishes Daily Content Pack (ranked concepts, hooks, captions)
    ↓
Tech reviews → approves concepts for production
```

## 📅 Weekly Workflow

```
Monday — Robo publishes Weekly Trend Memo
    ↓
Star publishes Weekly Content Slate (10 concepts, 3-bucket system)
    ↓
Backlog reviewed → production queue updated
```

---

## 📋 Content Pillars

All content maps to one or more of these pillars:

| Pillar | Examples |
|--------|---------|
| **Athlete Mindset** | Kobe, Jordan, Goggins — training mentality, sacrifice, pain |
| **Rapper / Artist Ambition** | Nipsey, Jay-Z, 50 Cent — hunger, ownership, growth, struggle |
| **Famous Speech Moments** | Denzel, Eric Thomas, Inky Johnson — powerful speech clips |
| **Grind & Hustle** | Anonymous quotes, daily discipline, no excuses mentality |
| **Mindset Shifts** | Reframes, perspective flips, counterintuitive truths |

---

## 🗂️ Files

```
content-research-workflow/
├── README.md                          # This file
├── sop/
│   ├── robo-star-sop.md              # Full SOP — roles, triggers, output formats
│   └── discord-report-format.md      # Standardized Discord output templates
```

---

## 🔧 Tech Stack

- **Claude AI (Sonnet + Opus)** — Powers both Robo and Star agents
- **OpenClaw** — Orchestration platform managing agent scheduling, memory, and handoffs
- **Cron Scheduler** — Triggers daily runs at precise times (8:00 AM + 8:15 AM CST)
- **Discord API** — Delivery channel for all agent outputs
- **Brave Search API** — Powers Robo's live trend discovery and news monitoring
- **Persistent Memory** — Agents retain context across sessions; track backlog and past performance

---

## 💡 What I Built & Learned

- Designed a **multi-agent coordination system** where two specialized LLMs hand off work with structured prompts
- Built **automated cron-based scheduling** so the pipeline runs daily without manual intervention
- Applied **prompt engineering** to create consistent, structured outputs across research and content roles
- Used **Discord as an async delivery layer** for agent-to-human and agent-to-agent communication
- Implemented **persistent agent memory** so Star retains backlog history and Robo tracks trend patterns over time

---

## 🔗 Related Projects

- [OpenClaw VPS AI System](https://roccopaz.github.io) — the infrastructure this workflow runs on
- [Mission Control Dashboard](https://roccopaz.github.io/mission-control/) — monitors this pipeline in the Intel + Content tabs
- [Portfolio](https://roccopaz.github.io) — full project breakdown

---

*AI content automation system — Texas State University CIS Senior · Built with Claude Code + OpenClaw ⚡*
