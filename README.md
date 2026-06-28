<div align="center">

# LLM Brand Tracker

**Free AI brand monitoring tool — track whether ChatGPT, Gemini, Grok, Claude, Google AI, and Perplexity recommend your brand**

[![Latest Release](https://img.shields.io/github/v/release/Lsaini-lab/llm-brand-tracker-releases?style=for-the-badge&color=7C3AED&label=Latest)](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)
[![Platform](https://img.shields.io/badge/Windows-10%2F11-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)
[![License](https://img.shields.io/badge/License-MIT-10B981?style=for-the-badge)](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)

**[Download for Windows — Free](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)**

</div>

---

![LLM Brand Tracker Dashboard](https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/dashboard.jpg)

---

When someone asks ChatGPT "best CRM for startups" or Gemini "top project management tools," they get a list of specific brands. If yours isn't on that list, you're invisible to that buyer at the exact moment they're deciding.

**LLM Brand Tracker** is a free AI brand monitoring and tracking tool for Windows. It queries ChatGPT, Claude, Gemini, Grok, Google AI Overview, and Perplexity in parallel with your keyword, finds every brand mentioned in each response, and shows you exactly where you rank — automatically, on a schedule, synced to Google Sheets.

This is the measurement layer for **GEO (Generative Engine Optimization) and AEO (Answer Engine Optimization)**. Run it weekly and you'll know whether your content strategy is actually moving the needle in AI-generated answers.

---

## What it does

- Queries all 6 major AI platforms in parallel — one run covers ChatGPT, Claude, Gemini, Grok, Google AI Overview, and Perplexity
- Detects your brand in each response and extracts your rank position (1st, 2nd, 3rd...)
- Identifies every competitor mentioned and calculates your AI Share of Voice %
- Saves a full-page screenshot from each platform after every run
- Syncs results to 5 structured Google Sheets tabs automatically — no manual export
- Runs on a schedule you control; Chrome runs headless in the background
- **Free to use** — no subscription, no SaaS fees, runs entirely on your machine

---

## Screenshots

<table>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/dashboard.jpg" alt="Dashboard — Brand Visibility Score, AI Share of Voice, best rank, run stats" />
      <p align="center"><strong>Dashboard</strong> — Brand Visibility Score, Share of Voice %, all-time stats</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/dashboard-2.jpg" alt="Intelligence Panel — SOV trend chart, competitor leaderboard" />
      <p align="center"><strong>Intelligence Panel</strong> — SOV% trend chart, competitor leaderboard</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/run-console.jpg" alt="Run Console — live output as Chrome queries all 6 AI platforms" />
      <p align="center"><strong>Run Console</strong> — Live output as Chrome queries each platform</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/keywords.jpg" alt="Keywords — AI Share of Voice, rank, last run time per keyword" />
      <p align="center"><strong>Keywords</strong> — Track multiple keywords, compare SOV% and rank</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/history.jpg" alt="History — every AI brand tracking run logged with SOV%, rank and platform count" />
      <p align="center"><strong>History & Trends</strong> — Every run logged, drill into any past session</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/screenshots-page.jpg" alt="Screenshots — full-page captures of ChatGPT, Gemini, Grok and more after every run" />
      <p align="center"><strong>Platform Captures</strong> — Full-page AI response screenshots saved per run</p>
    </td>
  </tr>
</table>

---

## How it works

The app uses Chrome DevTools Protocol (CDP) to drive a real Chrome browser using your saved login sessions — the same way you'd browse manually, but automated. You log in to each platform once; sessions last 30–60 days.

1. Click **Run Now** (or let the scheduler fire automatically)
2. Chrome boots in the background and submits your keyword to each AI platform as a logged-in user
3. Each response is scanned for brand names — against your tracked brands list (~80% accuracy), or via Claude Haiku for ~90% accuracy (~$0.001/run)
4. Results go to the Dashboard and your Google Sheet

A full 6-platform run takes 2–3 minutes.

---

## Download

| File | Notes |
|---|---|
| **LLM-Brand-Tracker-Setup-1.1.0.exe** | Recommended — installer with Start Menu shortcut |
| LLM-Brand-Tracker-1.1.0-win.zip | Portable — extract anywhere, no install required |

**[Go to Latest Release](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)** · Windows 10/11 (64-bit) · Chrome required · Free

> **SmartScreen warning?** Click **More info → Run anyway** — expected for open-source apps without a paid code-signing certificate. It's safe.

---

## Quick start

![Setup wizard — 7 steps, takes about 3 minutes](https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/onboarding.jpg)

1. Download and run the installer
2. Complete the 7-step setup wizard — enter your brand name, keyword, optionally connect Google Sheets (~3 min)
3. Log in to each AI platform when prompted — sessions save automatically and last 30–60 days
4. Click **Run Now**

Full walkthrough: [Getting Started guide](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/getting-started.md)

---

## Supported AI platforms

| Platform | Login |
|---|---|
| ChatGPT (chatgpt.com) | Yes — free account works |
| Claude (claude.ai) | Yes — free account works |
| Gemini (gemini.google.com) | Yes — Google account |
| Grok (grok.com) | Yes — X/Twitter account |
| Google AI Overview | No login needed |
| Perplexity (perplexity.ai) | No login needed |

---

## Google Sheets — 5 auto-populated tabs

Every tracking run syncs to your own Google Sheet automatically:

| Tab | What it tracks |
|---|---|
| overview | Full results per platform — status, brand mentioned, rank, SOV%, response snippet |
| rankings | Ordered competitor list per platform per run |
| sources | Every URL the AI cited in its response |
| trends | SOV%, best rank, visibility score, rank delta over time |
| competitor_sov | Per-competitor share of voice across all platforms |

### What the data looks like

<table>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/gsheet-overview.jpg" alt="Google Sheets overview tab — brand detected, rank, SOV%, citations and response snippet per platform" />
      <p align="center"><strong>overview tab</strong> — brand rank, SOV%, citations and response snippet per platform per run</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/gsheet-sources.jpg" alt="Google Sheets sources tab — every URL cited by ChatGPT, Grok, Perplexity and more" />
      <p align="center"><strong>sources tab</strong> — every URL each AI platform cited in its response</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/gsheet-trends.jpg" alt="Google Sheets trends tab — SOV% over time, visibility score, rank delta across runs" />
      <p align="center"><strong>trends tab</strong> — SOV% per run, visibility score, rank delta over time</p>
    </td>
    <td width="50%"></td>
  </tr>
</table>

See the [Google Sheets setup guide](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/google-sheets-setup.md) for the one-time configuration (~10 min).

---

## FAQ

**How accurate is brand detection?**
~80% without an API key (keyword matching). Add an Anthropic API key in Settings for ~90% via Claude Haiku (~$0.001/run).

**Do I need paid ChatGPT / Claude / Gemini subscriptions?**
No. Free accounts work on all platforms.

**Is my data private?**
All data stays on your machine and in your own Google Sheet. Nothing is sent to any server we control.

**Can I track multiple keywords?**
Yes. Add them on the Keywords page, run all at once with one click.

**Session showing "Login expired"?**
Settings → Browser Sessions → Re-run Login Setup. Grok expires fastest (~2–3 weeks); Google AI and Perplexity need no login.

**What is AI brand monitoring?**
AI brand monitoring is the practice of tracking how often and where AI platforms like ChatGPT, Gemini, and Perplexity mention your brand when users ask about your product category. LLM Brand Tracker automates this across all major platforms and measures your AI Share of Voice over time.

See the [full FAQ](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/faq.md) for more.

---

## Documentation

| Guide | |
|---|---|
| [Getting Started](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/getting-started.md) | Install and run your first AI brand tracking session |
| [Use Cases](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/use-cases.md) | Brand marketers, GEO/AEO agencies, founders, product teams |
| [FAQ](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/faq.md) | Setup, accuracy, platforms, privacy |
| [Google Sheets Setup](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/google-sheets-setup.md) | Step-by-step configuration |
| [vs. Brand24 / Mention / Brandwatch](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/comparison.md) | How AI brand monitoring differs from traditional tools |

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Platform shows "Login expired" | Settings → Browser Sessions → Re-run Login Setup |
| Chrome won't launch | Kill all chrome.exe in Task Manager, then retry |
| tracker.lock error | Settings → Browser Sessions → Clear tracker.lock |
| Google Sheets not syncing | Confirm service account has Editor access to your sheet |
| Brand missing from results | Settings → Brands → add exact spelling variants |
| SmartScreen on install | Click More info → Run anyway |

---

<div align="center">

Built by **[Lucky Saini](https://www.linkedin.com/in/luckysaini1412)**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-luckysaini1412-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/luckysaini1412)

*If this saves you time, a GitHub star helps others find it.*

</div>