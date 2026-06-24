---
title: Frequently Asked Questions
layout: default
---

# FAQ

---

## General

**What does LLM Brand Tracker actually do?**
It queries 6 AI platforms — ChatGPT, Claude, Gemini, Grok, Google AI Overview, and Perplexity — with your keyword, extracts every brand mentioned in each response, detects your brand and rank, calculates Share of Voice %, and syncs everything to Google Sheets. Runs on a schedule you set.

**Is it free?**
Yes. MIT licensed, no subscription, no usage limits. The optional Anthropic API key for improved detection costs ~$0.001/run (billed by Anthropic directly). Google Sheets sync uses your own account — also free.

**What is AI Share of Voice?**
The percentage of AI platform responses that mention your brand for a given keyword. If 4 out of 6 platforms mention you, your SOV% is ~67%. Tracking this weekly shows whether your AI visibility is improving or declining.

**What is GEO / AEO / LLM SEO?**
All the same thing: optimizing your brand's presence in AI-generated answers. As ChatGPT, Claude, and Gemini become primary research tools, appearing in their responses matters — not unlike ranking on page 1 of Google. LLM Brand Tracker measures your GEO performance so you know whether your content strategy is working.

---

## Setup

**What do I need to install it?**
Windows 10 or 11 (64-bit) and Google Chrome. 4 GB RAM recommended. About 500 MB disk space. Free accounts on the AI platforms you want to track.

**Do I need paid ChatGPT, Claude, or Gemini subscriptions?**
No. Free accounts work fine on all platforms.

**How long does setup take?**
The wizard takes about 3 minutes. Logging into AI platforms adds another 2–5 minutes.

**Can I install without admin rights?**
Yes — use the portable ZIP version. Extract anywhere and run the exe.

**Does it work on Mac or Linux?**
Windows only for now.

---

## Tracking

**How accurate is brand detection?**
Two layers run simultaneously:

- **With Anthropic API key:** ~90% — Claude Haiku reads each response and extracts brand names
- **Without API key:** ~80% — keyword matching against your tracked brands list

For trend tracking, 80% is good enough. The API key is recommended if you're running client reports and need higher confidence per run.

**Why wasn't my brand detected even though the AI mentioned it?**
Three common reasons: (1) the spelling in your brands list doesn't match how the AI wrote it — add variants; (2) LLM responses vary run to run, so a brand that appeared last time may not appear this time; (3) the platform session expired and returned a login page instead of a real response.

**How often do AI responses change?**
Frequently. LLMs don't return identical responses every time, especially for competitive categories. This is why the trend chart over many runs is more meaningful than any single result.

**What is "Brand Rank"?**
When AI platforms return numbered lists, the app parses your position — rank 1 means you're the top recommendation. When there's no numbered list, it falls back to your position by character offset in the response.

---

## Platforms

**Why does it need my login sessions?**
The app uses Chrome DevTools Protocol (CDP) to connect to real Chrome with your saved login sessions. This lets it query platforms as a logged-in user — no platform API key, no subscription. Sessions last 30–60 days.

**What happens when a session expires?**
The platform shows "Login expired" in the Dashboard. Settings → Browser Sessions → Re-run Login Setup. Grok expires fastest (~2–3 weeks). Google AI Overview and Perplexity don't require login.

**Can I track fewer than 6 platforms?**
Yes. Settings → Platforms → toggle any on or off.

---

## Google Sheets

**Is Google Sheets required?**
No. All results are saved locally and visible inside the app regardless. Google Sheets adds automatic delivery to a spreadsheet you own.

**What does it cost?**
Nothing. You use your own Google account. Setup requires a free Google Cloud Service Account — the process takes about 10 minutes and is covered in the [setup guide](./google-sheets-setup.md).

**What tabs does it create?**
Five, auto-created on the first sync: `overview`, `rankings`, `sources`, `trends`, `competitor_sov`. New rows are appended after every run — existing data is never overwritten.

---

## Privacy

**Is my data sent anywhere?**
No. Everything stays on your machine and in your own Google Sheet. We have no server receiving your brand data, keywords, or results.

**Does it store my passwords?**
No. It saves browser session cookies — the same thing your browser does when you stay logged in. Your passwords are never seen by the app.
