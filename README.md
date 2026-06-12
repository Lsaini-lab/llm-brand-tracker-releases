<div align="center">

# LLM Brand Tracker

### Know exactly when and where AI recommends your brand

[![Latest Release](https://img.shields.io/github/v/release/Lsaini-lab/llm-brand-tracker-releases?style=for-the-badge&color=7C3AED&label=Latest)](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)
[![Platform](https://img.shields.io/badge/Windows-10%2F11-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)
[![License](https://img.shields.io/badge/License-MIT-10B981?style=for-the-badge)](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)

**[Download for Windows (.exe)](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)**

</div>

---

![LLM Brand Tracker Dashboard](https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/dashboard.jpg)

---

## What Is LLM Brand Tracker?

When someone asks ChatGPT *"best laptop for business"* or Gemini *"top project management tools"* — they get a list of specific brands. If your brand is not in that list, you are invisible to a fast-growing share of your market.

**LLM Brand Tracker** is a free Windows desktop app that automatically queries 6 major AI platforms with your keywords, detects whether your brand is recommended, measures your rank among competitors, and syncs everything to Google Sheets — on a schedule you control, while you sleep.

This is the measurement tool for **Generative Engine Optimization (GEO)** and **AI Engine Optimization (AEO)** — track where your brand stands in AI-generated responses today, and measure whether your content strategy is working.

---

## Who Is This For

**Brand marketers** — Run weekly tracking sessions to see whether ChatGPT, Gemini, and Perplexity are recommending you or a competitor. Include AI Share of Voice % in your monthly brand reports.

**SEO and GEO agencies** — Track multiple client brands across 6 AI platforms. Show clients week-over-week rank improvements that prove your GEO campaign is working. Export automatically to Google Sheets for client delivery.

**Founders and startups** — Find out if AI recommends your product when buyers ask about your category. Track whether your content and PR investments are improving your position over time.

**Product marketers** — See your exact rank on each platform (ChatGPT vs Gemini vs Perplexity often rank you differently). Monitor competitor positioning changes in real time.

**PR and communications teams** — Measure whether a press campaign, product launch, or new content changed your AI visibility. Compare before and after.

---

## How It Works

LLM Brand Tracker uses **Chrome DevTools Protocol (CDP)** to connect to a real Chrome browser using your saved login sessions — the same way a human would browse the site.

1. You log in to each AI platform once through the app's setup wizard. Sessions are saved and last 30–60 days.
2. When you click Run, the app silently boots Chrome in the background and submits your keyword to each selected AI platform as a logged-in user.
3. Each platform's response is captured as text and a full-page screenshot.
4. The app scans every response for brand names — using pattern matching against your Brands list, and optionally using Claude Haiku AI for ~90% accuracy.
5. Results are compiled into Share of Voice %, brand rank, competitor list, and platform status — then synced to Google Sheets automatically.

No platform API keys are needed. No subscription to ChatGPT Plus, Claude Pro, or Gemini Advanced is required. Free accounts work on all platforms.

---

## Features

### Brand Visibility & Ranking
- **Brand Mention Detection** — instantly knows whether each AI platform mentioned your brand in its response
- **Brand Rank Extraction** — parses numbered lists from AI responses to find your exact position (1st, 2nd, 3rd...)
- **Brand Visibility Score** — a single 0–100 score combining SOV%, mention rate, and rank across all platforms
- **Share of Voice %** — how often your brand appears across all 6 platforms combined vs. every competitor

### Competitor Intelligence
- **Competitor Detection** — every brand mentioned in any AI response is captured automatically
- **Discover Competitors** — identifies new brands from your last run not yet in your tracked list
- **Competitor Leaderboard** — ranked list of which competitors appear most often in AI responses
- **Top Competitors Bar Chart** — frequency chart of the most-mentioned brands across recent runs
- **Competitor SOV % per platform** — see which platforms favour your competitors over you

### Multi-Platform Coverage
- **6 platforms in one run** — ChatGPT, Claude, Gemini, Grok, Google AI Overview, Perplexity queried in parallel
- **Platform Health Indicator** — live status showing which platforms answered, had login issues, or were blocked
- **Per-platform screenshots** — full-page screenshot of every AI response saved automatically after each run
- **Screenshots Gallery** — browse all captured AI responses by platform, keyword, and date

### Tracking & History
- **Run History** — every tracking run stored with timestamp, keyword, platform breakdown, SOV%, and rank
- **Trends Chart** — SOV% and rank plotted over time so you can see whether your brand is rising or falling
- **Rank Timeline** — track your position across platforms week by week
- **30-day, 7-day, and all-time views** — filter history to the time window that matters

### Keywords
- **Multi-keyword support** — add unlimited keywords and track each one independently
- **Run All Keywords** — process every keyword in sequence with one click
- **Keyword Comparison** — view SOV% and rank side by side across keywords
- **Per-keyword stats** — last run time, average SOV%, best rank shown on the keywords list

### Automation & Scheduling
- **Scheduled Runs** — set the app to run automatically every N hours, daily, or on any custom interval
- **Headless mode** — Chrome runs invisibly in the background with no visible windows
- **Auto-updates** — the app notifies you when a new version is available and updates silently

### Google Sheets Integration
- **Automatic sync** after every run — no manual export needed
- **5 structured tabs** auto-created and maintained: overview, rankings, sources, trends, competitor_sov
- **Rank delta** — the trends tab tracks whether your rank improved or declined since the previous run
- **Test Connection** button — verify your Google Sheets setup before running

### Accuracy & Detection
- **Two-layer detection** — brand list scan (~80% accuracy) plus optional Claude Haiku AI extraction (~90% accuracy)
- **Claude AI extraction** — add an Anthropic API key in Settings for smarter brand detection (~$0.001 per run)
- **Citation tracking** — captures every external URL the AI cited in its response (sources tab)

### Setup & Usability
- **7-step setup wizard** — guided onboarding for non-technical users, takes about 3 minutes
- **Works with free accounts** — no paid subscriptions needed for ChatGPT, Claude, Gemini, or Grok
- **Session persistence** — log in once per platform; sessions are saved and last 30–60 days automatically
- **Browser Session Manager** — refresh expired sessions from inside the app without re-running setup
- **Brands management** — add, remove, and bulk-import your tracked competitor list
- **Free to use** — no SaaS subscription, no usage fees, runs entirely on your machine

---

## Screenshots

<table>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/dashboard.jpg" alt="Dashboard showing Brand Visibility Score, SOV%, all-time best rank and run stats" />
      <p align="center"><strong>Dashboard</strong> — Brand Visibility Score, SOV%, all-time stats and per-keyword performance</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/dashboard-2.jpg" alt="Intelligence Panel showing SOV% trend chart, competitor leaderboard and platform health" />
      <p align="center"><strong>Intelligence Panel</strong> — SOV% trend chart, competitor leaderboard, top competitors ranked by frequency</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/run-console.jpg" alt="Run Console showing live CDP log as Chrome boots and queries all 6 platforms" />
      <p align="center"><strong>Run Console</strong> — Live output as the app boots Chrome and queries all 6 platforms in real time</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/keywords.jpg" alt="Keywords page showing 5 keywords each with SOV%, rank, last run time and comparison panel" />
      <p align="center"><strong>Keywords</strong> — Track multiple keywords, see SOV% and rank per keyword, compare side by side</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/history.jpg" alt="History and Trends showing 30 runs listed with timestamp, platforms answered, SOV% and rank" />
      <p align="center"><strong>History & Trends</strong> — Every run logged with SOV%, rank, and platform count — drill into any past run</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/brands.jpg" alt="Brands page showing tracked competitor list and Discover Competitors button" />
      <p align="center"><strong>Brands</strong> — Manage your competitor list; Discover Competitors auto-detects brands from AI responses</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/screenshots-page.jpg" alt="Screenshots gallery showing full AI response screenshots per platform browsable by keyword and date" />
      <p align="center"><strong>Screenshots Gallery</strong> — Browse the exact AI response captured from every platform per run</p>
    </td>
    <td width="50%">
      <img src="https://raw.githubusercontent.com/Lsaini-lab/llm-brand-tracker-releases/main/docs/screenshots/settings.jpg" alt="Settings page showing Brand Identity section, Setup Status checklist and platform tabs" />
      <p align="center"><strong>Settings</strong> — Set your brand name, connect Google Sheets, toggle platforms, manage browser sessions</p>
    </td>
  </tr>
</table>

---

## Download

| File | Notes |
|---|---|
| **LLM-Brand-Tracker-Setup-1.1.0.exe** | Recommended — installer with Start Menu shortcut and silent auto-updates |
| LLM-Brand-Tracker-1.1.0-win.zip | Portable — extract anywhere and run, no installation needed |

**[Go to Latest Release](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)**

**Requirements:** Windows 10/11 (64-bit) · Google Chrome installed

> **Windows SmartScreen warning?** Click **More info → Run anyway** — this is expected for unsigned open-source apps.

---

## Install in 3 Steps

1. Download `LLM-Brand-Tracker-Setup-1.1.0.exe` from the release above
2. Run the installer and launch **LLM Brand Tracker** from your desktop or Start menu
3. Complete the 7-step setup wizard (~3 minutes) — enter your brand name, keyword, and optionally connect Google Sheets

For a full walkthrough, see the [Getting Started guide](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/getting-started.md).

---

## Supported AI Platforms

| Platform | Login required |
|---|---|
| ChatGPT (chatgpt.com) | Yes — free account works |
| Claude (claude.ai) | Yes — free account works |
| Gemini (gemini.google.com) | Yes — Google account |
| Grok (grok.com) | Yes — X/Twitter account |
| Google AI Overview | No login required |
| Perplexity (perplexity.ai) | No login required |

---

## Google Sheets — 5 Auto-Populated Tabs

| Tab | What is tracked |
|---|---|
| overview | Full results per platform per run — status, brand mentioned, rank, SOV%, top competitors |
| rankings | Ordered competitor list per platform — pure competitive intelligence, no noise |
| sources | Every external URL the AI cited in its response |
| trends | SOV%, best rank, rank delta, visibility score over time per keyword |
| competitor_sov | Per-competitor share-of-voice across all platforms |

**One-time setup:** Create a Google Cloud project → enable Sheets API → create a Service Account → share your sheet with it → paste credentials in Settings → Test Connection. See the [full Google Sheets setup guide](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/google-sheets-setup.md).

---

## Frequently Asked Questions

**Does it work with free ChatGPT, Claude, and Gemini accounts?**
Yes. Free accounts work on all platforms.

**How accurate is brand detection?**
Around 80% accuracy with no API key. Add an Anthropic API key in Settings to reach ~90% accuracy (~$0.001 per run via Claude Haiku).

**Is my data private?**
All data stays on your machine and in your own Google Sheet. Nothing is sent to any server we control.

**Sessions show "Login expired"?**
Browser sessions last 30–60 days. Go to Settings → Browser Sessions → Re-run Login Setup to refresh.

**Can I track multiple keywords?**
Yes — add them on the Keywords page and click Run All Keywords to process each in sequence.

**What is GEO / AEO?**
Generative Engine Optimization (GEO) and AI Engine Optimization (AEO) are strategies to improve how often AI platforms recommend your brand when users search for your category. LLM Brand Tracker is the measurement layer — it tells you exactly where you stand today and whether your efforts are working over time.

See the [full FAQ](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/faq.md) for more questions.

---

## Documentation

| Guide | What it covers |
|---|---|
| [Getting Started](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/getting-started.md) | Install the app and run your first session in 10 minutes |
| [Use Cases](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/use-cases.md) | Brand marketers, SEO/GEO agencies, founders, product teams |
| [FAQ](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/faq.md) | Setup, accuracy, platforms, privacy, pricing |
| [Google Sheets Setup](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/google-sheets-setup.md) | Step-by-step Google Cloud and Sheets configuration |
| [Comparison vs. Brand24 / Mention / Brandwatch](https://github.com/Lsaini-lab/llm-brand-tracker-releases/blob/main/docs/comparison.md) | How AI monitoring differs from traditional brand listening |

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Platform shows "Login expired" | Settings → Browser Sessions → Re-run Login Setup |
| Chrome won't launch | Kill all chrome.exe in Task Manager and retry |
| tracker.lock error | Settings → Browser Sessions → Clear tracker.lock |
| Google Sheets not syncing | Verify service account has Editor access to your sheet |
| Brand missing from results | Settings → Brands → add it to your tracked list |
| Windows SmartScreen on install | Click More info → Run anyway |

---

<div align="center">

Built by **[Lucky Saini](https://www.linkedin.com/in/luckysaini1412)**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-luckysaini1412-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/luckysaini1412)

*If this saves you time, please star this repo — it helps others find it.*

</div>
