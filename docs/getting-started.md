---
title: Getting Started
layout: default
---

# Getting Started with LLM Brand Tracker

This guide walks you through installing the app and running your first brand tracking session from scratch.

---

## What You Need

- Windows 10 or 11 (64-bit)
- Google Chrome installed (any version)
- Accounts on the AI platforms you want to track (free accounts work on all of them)
- 5–10 minutes for first-time setup

---

## Step 1 — Download and Install

1. Go to the [latest release](https://github.com/Lsaini-lab/llm-brand-tracker-releases/releases/latest)
2. Download `LLM-Brand-Tracker-Setup-1.1.0.exe`
3. Run the installer

> **Windows SmartScreen warning:** Windows may show "Windows protected your PC." Click **More info → Run anyway.** This appears because the app is open-source and does not have a paid code-signing certificate. It is safe to proceed.

4. Launch **LLM Brand Tracker** from your desktop or Start menu

---

## Step 2 — Setup Wizard (7 Steps)

On first launch, a guided setup wizard opens automatically.

### Step 1 of 7 — Your Brand Name
Enter the brand name you want to track in AI responses. This is the name the app will look for in every AI platform's answer.

Examples: `Notion`, `HubSpot`, `Lenovo`, `Shopify`, `Your Company Name`

This can be changed at any time in Settings → General → Brand Identity.

### Step 2 of 7 — Your Keyword
Enter the search phrase your customers type into AI platforms.

Examples:
- `best laptop for business professionals`
- `top CRM software for small business`
- `best project management tools`
- `which accounting software should I use`

Think about what a potential customer would ask ChatGPT or Gemini when looking for a product in your category.

### Step 3 of 7 — Choose Platforms
Select which of the 6 AI platforms to include in each tracking run. All are enabled by default.

| Platform | Notes |
|---|---|
| ChatGPT | Requires login — free account works |
| Claude | Requires login — free account works |
| Gemini | Requires login — Google account |
| Grok | Requires login — X/Twitter account |
| Google AI Overview | No login needed |
| Perplexity | No login needed |

### Step 4 of 7 — Anthropic API Key (Optional)
Adding an Anthropic API key enables Claude Haiku to extract brands from AI responses, improving detection accuracy from ~80% to ~90%.

Cost: approximately $0.001 per tracking run (1–2k tokens).

If you skip this step, the app uses keyword matching against your brands list instead, which is free and works well for most use cases.

Get a key at [console.anthropic.com/settings/keys](https://console.anthropic.com/settings/keys).

### Step 5 of 7 — Google Sheets (Optional)
Connect a Google Sheet to receive automatic sync after every run. See the [Google Sheets Setup guide](./google-sheets-setup.md) for full instructions.

If you skip this, results are still saved locally and visible in the Dashboard and History pages.

### Step 6 of 7 — Browser Login
The app opens Chrome with tabs for each AI platform that requires login. Log in to each one. Your sessions are saved automatically and last 30–60 days before needing to be refreshed.

This step only needs to be done once. You can re-run it anytime from Settings → Browser Sessions.

### Step 7 of 7 — Done
Click **Finish**. You are taken to the Dashboard.

---

## Step 3 — Run Your First Tracking Session

Click **Run Now** in the sidebar or from the Run Console page.

The app will:
1. Boot Chrome (you will see a terminal/console output)
2. Query each selected AI platform with your keyword
3. Extract every brand mentioned in each response
4. Detect whether your brand was mentioned and at what rank
5. Save a full-page screenshot from each platform
6. Calculate your Share of Voice % across all platforms
7. Sync results to Google Sheets (if connected)

A full run across all 6 platforms takes approximately 2–3 minutes.

---

## Step 4 — Read Your Results

After the run completes, the Dashboard updates with:

- **Brand Visibility Score** — your overall AI visibility (0–100)
- **Total Runs** — how many tracking runs you have done all-time
- **Best SOV% Ever** — your peak share of voice across all runs
- **Best Rank Ever** — the highest rank position your brand has achieved
- **Per-keyword breakdown** — SOV%, rank, and platform count for each keyword

Click into any keyword row to see which platforms mentioned you, your rank on each, and which competitors appeared.

---

## What to Do Next

- **Add competitors to track** — go to the Brands page and add competitor names you want to monitor
- **Set up a schedule** — go to Settings → Advanced → Schedule to run automatically every N hours
- **Add more keywords** — go to Keywords and add different search phrases to track
- **Review the trend chart** — after a few runs, the History page shows whether your visibility is improving

---

## Common First-Run Issues

**"Login expired" on a platform**
You did not log in during Step 6, or the session expired. Go to Settings → Browser Sessions → Re-run Login Setup.

**Chrome window doesn't open**
Kill all `chrome.exe` processes in Task Manager and try again.

**Run finishes but Dashboard shows no data**
Wait 10 seconds and refresh the Dashboard. If still empty, check the Run Console output for error messages.

**Brand not detected**
Your brand may not have been mentioned in the AI responses, or the spelling doesn't match. Go to Brands page and add exact spelling variants.
