---
title: Frequently Asked Questions
layout: default
---

# Frequently Asked Questions

---

## General Questions

**What is LLM Brand Tracker?**
LLM Brand Tracker is a free Windows desktop app that automatically queries 6 AI platforms — ChatGPT, Claude, Gemini, Grok, Google AI Overview, and Perplexity — with your keywords, detects whether your brand appears in each response, measures your rank among competitors, and syncs results to Google Sheets. It is the measurement tool for Generative Engine Optimization (GEO) and AI brand monitoring.

**Does AI mention my brand?**
The only way to find out is to ask. LLM Brand Tracker asks all 6 major AI platforms your category keyword and reports back which ones mentioned you, at what rank position, and which competitors appeared instead. Download the app and run your first session in under 10 minutes.

**How do I know if ChatGPT recommends my brand?**
Install LLM Brand Tracker, enter your brand name and the keyword your customers use (e.g. "best CRM for startups"), and click Run. The app queries ChatGPT automatically and shows whether your brand was mentioned and at what rank.

**Is this free?**
Yes. The app is free. There are no subscription fees or usage limits. The optional Anthropic API key (for improved detection accuracy) costs approximately $0.001 per run. Google Sheets sync uses your own Google account — also free.

**What is AI Share of Voice?**
AI Share of Voice (SOV%) is the percentage of AI platform responses that mention your brand when queried with a given keyword. If you track 6 platforms and 4 of them mention your brand, your SOV% is approximately 67%. Tracking this over time shows whether your AI visibility is improving.

**What is GEO / AEO / LLM SEO?**
These terms all describe the same discipline: optimizing your brand's presence in AI-generated answers.
- **GEO** — Generative Engine Optimization
- **AEO** — Answer Engine Optimization
- **LLM SEO** — SEO for large language model platforms

As ChatGPT, Claude, and Gemini become primary research tools, appearing in their responses is as important as ranking on Google. LLM Brand Tracker measures your GEO performance.

**Why does AI brand visibility matter?**
Research shows a growing share of purchase decisions are now AI-influenced. When a buyer asks ChatGPT "what is the best tool for X" before visiting any website, the brands mentioned in that response have a significant advantage. If your brand is not mentioned, you are missing a channel that is growing faster than traditional search.

---

## Setup and Installation

**What are the system requirements?**
Windows 10 or 11 (64-bit) and Google Chrome. 4 GB RAM recommended. Approximately 500 MB disk space.

**Do I need to pay for ChatGPT, Claude, or Gemini?**
No. Free accounts on all platforms work fine. The app logs in with your saved browser session, so it sees the same responses a free user would see.

**How long does setup take?**
The 7-step setup wizard takes approximately 3 minutes. Logging in to AI platforms (Step 6) takes another 2–5 minutes depending on how many platforms you use.

**Can I install it without admin rights?**
Yes, if you use the portable ZIP version. Extract it anywhere and run the exe — no installation required.

**Does it work on Mac or Linux?**
Currently Windows only. Mac and Linux support may come in a future release.

---

## Tracking and Accuracy

**How accurate is brand detection?**
Two-layer detection:
- **With Anthropic API key:** ~90% accuracy using Claude Haiku to extract brands from AI responses
- **Without API key:** ~80% accuracy using keyword matching against your brands list

For most use cases, 80% accuracy without an API key is sufficient for trend tracking. The Claude API key is recommended for agencies running client reports.

**Why doesn't a platform show my brand even when I know it mentions it?**
Possible reasons:
1. Your brand spelling in the app does not exactly match how the AI writes it. Add variants to your Brands page.
2. The AI gave a different response this time — LLM responses vary run to run, especially for competitive categories.
3. The platform session expired and returned a login page instead of a real response.

**How often do AI responses change?**
Frequently. LLMs do not return identical responses every time. A brand that appears in one run may not appear in the next. This is why trend data (running the same keyword repeatedly over time) is more meaningful than any single run.

**What is Brand Rank?**
When AI platforms return numbered lists ("1. Brand A  2. Brand B  3. Your Brand"), LLM Brand Tracker extracts your position from that list. This is your brand rank. Rank 1 means you are the top recommendation. When the AI does not use a numbered list, rank falls back to character position in the response.

---

## AI Platforms

**Why does the app need me to log in to AI platforms?**
The app uses Chrome DevTools Protocol (CDP) to connect to a real Chrome browser with your saved login sessions. This lets it query the platforms exactly as a logged-in user would — seeing the same personalized responses, without any platform API key or subscription. Sessions last 30–60 days before needing refresh.

**What happens when a platform session expires?**
The platform shows "Login expired" status in the Dashboard. Go to Settings → Browser Sessions → Re-run Login Setup to refresh. Grok sessions typically expire fastest (2–4 weeks). Google and Perplexity do not require login.

**Can I track just some platforms and not all 6?**
Yes. Go to Settings → Platforms and toggle individual platforms on or off. You can also choose platforms per-run from the Run Console page.

**Does it work with paid ChatGPT / Claude subscriptions?**
Yes. The app logs in with your account regardless of subscription tier. If you have a paid account, it will see responses through that account.

---

## Google Sheets

**Is Google Sheets required?**
No. It is optional. Without it, all results are saved locally and visible in the Dashboard, Keywords, and History pages inside the app. Google Sheets sync adds automatic report delivery to a spreadsheet you own.

**What does the Google Sheets integration cost?**
Nothing. You use your own Google account and Google Drive. The only setup required is creating a Service Account in Google Cloud (free tier) and sharing your sheet with it.

**How many tabs does it create?**
Five tabs, created automatically:
- **overview** — full results per platform per run
- **rankings** — competitor list per platform
- **sources** — URLs cited by AI in responses
- **trends** — SOV%, rank, and delta over time
- **competitor_sov** — per-competitor share of voice across all platforms

**Does it overwrite existing data?**
No. It appends new rows after each run. Your historical data is never overwritten.

---

## Privacy and Security

**Is my brand data sent anywhere?**
No. All tracking data stays on your machine and in your own Google Sheet. The app does not transmit your brand name, keywords, or results to any server we control.

**Does the app store my AI platform passwords?**
No. The app saves your browser session cookies (same as any browser does), not your passwords. Your credentials are never visible to the app.

**Can I use this for competitor research without them knowing?**
Yes. The app queries AI platforms as a regular logged-in user. There is no way for a competitor to know you are running queries about their brand.

---

## Pricing and Business Model

**Is it really free forever?**
Yes. The app is MIT licensed, free to download and use with no usage limits. The optional Anthropic API key is pay-per-use at ~$0.001 per run, billed by Anthropic directly — we receive nothing from it.

**Is there a paid or Pro version?**
Not currently. All features are available in the free version.
