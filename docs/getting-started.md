---
title: Getting Started
layout: default
---

# Getting Started

Install LLM Brand Tracker and run your first brand tracking session from scratch.

**Requirements:** Windows 10/11 (64-bit), Google Chrome, accounts on the AI platforms you want to track (free accounts work on all of them).

---

## Step 1 — Install

1. Go to the [latest release](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)
2. Download `LLM-Brand-Tracker-Setup-1.1.0.exe`
3. Run the installer

> **Windows SmartScreen warning:** Click **More info → Run anyway.** This appears because the app is open-source and unsigned. It's safe to proceed.

4. Launch **LLM Brand Tracker** from your desktop or Start menu

---

## Step 2 — Setup Wizard

On first launch the setup wizard opens automatically. It has 7 steps and takes about 3 minutes.

**Brand name** — the name the app will look for in AI responses. Enter it exactly as the AI would write it (e.g. `Notion`, `HubSpot`, `Shopify`). You can change this later in Settings.

**Keyword** — the search phrase your customers type into AI platforms. Think about what someone would ask ChatGPT when looking for a product in your category:
- `best laptop for business professionals`
- `top CRM for small teams`
- `which accounting software do agencies use`

**Platforms** — all 6 are enabled by default. You can toggle any off.

**Anthropic API key (optional)** — improves brand detection from ~80% to ~90% accuracy. Cost is about $0.001 per run (Claude Haiku). Skip this if you want to start free — the default keyword matching works fine for trend tracking.

**Google Sheets (optional)** — connect a sheet to receive automatic sync after every run. See the [Google Sheets setup guide](./google-sheets-setup.md). Skip for now if you want to try the app first; all results are stored locally regardless.

**Browser login** — the app opens Chrome with tabs for each platform that requires a login. Sign in to each one. Your sessions are saved and last 30–60 days before needing refresh. This step only runs once; you can redo it anytime from Settings → Browser Sessions.

**Done** — click Finish and you land on the Dashboard.

---

## Step 3 — Run

Click **Run Now** in the sidebar or from the Run Console page.

The app boots Chrome in the background, queries each selected platform with your keyword, extracts every brand mentioned in each response, calculates your Share of Voice %, saves a screenshot from each platform, and syncs to Google Sheets if connected. A full 6-platform run takes 2–3 minutes.

---

## Step 4 — Read the results

After the run completes the Dashboard updates with your Brand Visibility Score (0–100), SOV%, best rank, and a per-keyword breakdown. Click any keyword row to see which platforms mentioned you, your rank on each, and which competitors appeared.

The History page shows every past run. After a few runs the Trends chart starts showing whether your visibility is rising or falling.

---

## What to do next

- **Add competitors** — Brands page → add names you want to monitor in AI responses
- **Add keywords** — Keywords page → track different search phrases
- **Set a schedule** — Settings → Advanced → Schedule → run automatically every N hours
- **Refresh sessions when they expire** — Settings → Browser Sessions → Re-run Login Setup (needed every 30–60 days)

---

## Common first-run issues

**"Login expired" on a platform** — you didn't log in during setup, or the session expired. Settings → Browser Sessions → Re-run Login Setup.

**Chrome doesn't open** — kill all `chrome.exe` processes in Task Manager and try again.

**Dashboard shows no data after run** — wait 10 seconds and reload. If still empty, check the Run Console output for error messages.

**Brand not detected** — check the Brands page and confirm the spelling matches how the AI writes it. Add variants if needed.
