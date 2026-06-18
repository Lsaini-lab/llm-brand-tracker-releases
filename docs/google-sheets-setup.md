---
title: Google Sheets Setup
layout: default
---

# Google Sheets Setup Guide

LLM Brand Tracker can automatically sync tracking results to a Google Sheet you own after every run. This gives you a permanent, shareable record of your AI brand visibility data across 5 structured tabs.

---

## What Gets Synced

| Tab | What it contains |
|---|---|
| **overview** | Full results per platform per run — date, keyword, platform, status, brand mentioned, rank, SOV%, top competitors, citation count |
| **rankings** | Ordered competitor list per platform — date, keyword, platform, rank, brand name |
| **sources** | Every external URL the AI cited in its response — date, keyword, platform, domain, URL |
| **trends** | SOV%, best rank, rank delta, platforms answered, visibility score — one row per keyword per run |
| **competitor_sov** | Per-competitor share-of-voice across all platforms — date, keyword, brand, mention count, platform count, SOV% |

All tabs are created automatically on the first sync. New rows are appended after each run — existing data is never overwritten.

---

## One-Time Setup (10 Minutes)

### Part 1 — Google Cloud Project and Service Account

1. Go to [console.cloud.google.com](https://console.cloud.google.com)
2. Click **Select a project** → **New Project** → name it anything (e.g. "LLM Tracker") → **Create**
3. In the search bar, search for **Google Sheets API** → click it → click **Enable**
4. In the left menu, go to **IAM & Admin → Service Accounts**
5. Click **Create Service Account**
   - Name: anything (e.g. "llm-tracker")
   - Click **Create and Continue** → skip the optional steps → **Done**
6. Click on the service account you just created
7. Go to the **Keys** tab → **Add Key → Create new key → JSON** → **Create**
8. A JSON file downloads automatically. Keep this file — you will need it in Step 3.

### Part 2 — Create and Share the Google Sheet

1. Go to [sheets.google.com](https://sheets.google.com) and create a new blank spreadsheet
2. Name it anything (e.g. "LLM Brand Tracker")
3. Click **Share** (top right)
4. Open the JSON file you downloaded in Part 1 and find the `client_email` field. It looks like: `llm-tracker@your-project.iam.gserviceaccount.com`
5. Paste that email into the Share dialog
6. Set permission to **Editor**
7. Click **Send** (ignore the warning about sharing with a service account)
8. Copy the URL of your sheet from the browser address bar — you will need it in Step 3

### Part 3 — Connect in the App

1. Open **LLM Brand Tracker**
2. Go to **Settings → Integrations**
3. Under **Google Sheets**:
   - Click **Upload Service Account JSON** and select the JSON file from Part 1
   - Paste your Google Sheet URL into the **Sheet URL** field
4. Click **Test Connection**
5. You should see a green success message. If not, check that the service account email has Editor access to the sheet.

That is all. The next time you run a tracking session, results will appear in your sheet automatically.

---

## Troubleshooting

**"Invalid credentials" error**
The JSON file path may have changed or the file was moved. Re-upload it in Settings → Integrations.

**"Permission denied" error**
The service account does not have access to the sheet. Go to your Google Sheet → Share → verify the service account email is listed with Editor permission.

**Columns appearing in wrong sheet / wrong tab**
Do not rename or reorder the 5 tabs (overview, rankings, sources, trends, competitor_sov). The app writes to these tabs by name. You can add additional tabs freely.

**Data not appearing after a run**
Check that Google Sheets sync is enabled: Settings → Advanced → Sync to Google Sheets must be toggled on.

---

## Reading Your Data

### Overview Tab
Each row is one platform from one run. Status values:
- `✓ Answered` — real response captured, data is reliable
- `✗ Login expired` — session needs refreshing
- `✗ Captcha` — platform blocked the request, retry later
- `✗ No response` — platform loaded but no answer was extracted

### Trends Tab
The most useful tab for measuring progress over time. Key columns:
- `sov_pct` — your Share of Voice % that run (brand mentions / total platforms)
- `best_rank` — your highest rank position across all platforms that run
- `rank_delta` — how your best rank changed since the previous run (negative = improved)
- `platforms_answered` — how many platforms gave a real response

### Competitor SOV Tab
Shows which competitors appear most often in AI responses for your keyword. Sort by `mention_count` descending to see your top AI competitors. This updates after every run.
