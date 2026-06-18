# Changelog

All notable changes to LLM Brand Tracker are documented here.

---

## v1.1.0 — June 2026

### New Features
- **Full brand-agnosticism** — the app now works for any brand name. Set yours in Settings and every metric, label, and report updates dynamically. No longer tied to a single client or product.
- **Brand Visibility Score** — a new 0–100 composite score combining Share of Voice %, mention rate across platforms, and best rank. Single number to track week over week.
- **Keyword Comparison panel** — select 2–3 keywords on the Keywords page to compare their SOV% and rank side by side.
- **Discover Competitors** — the Brands page now detects brands found in your last run that are not yet in your tracked list and lets you add them with one click.

### Fixes
- Dashboard Total Runs counter now shows correct all-time count across all run history files
- Chart animations no longer double-fire on load in React StrictMode
- Keywords page SOV%, rank, and Last Run now populate correctly after each tracking run completes
- Fixed permanent loading state on the Keywords page when network responses are slow
- Removed macOS-only titleBar setting that caused a white gap in the Windows title bar
- App icon regenerated at 16/32/48/256px with the new hexagonal logo design

### Under the Hood
- Renamed all internal `pmaps*` variable names to generic equivalents — codebase is now fully brand-neutral
- Backward-compatible reads of `pmaps_mentioned` field preserved so existing run history loads correctly

---

## v1.0.0 — May 2026

### Initial Release
- Query 6 AI platforms in parallel: ChatGPT, Claude, Gemini, Grok, Google AI Overview, Perplexity
- Brand mention detection and rank extraction from AI responses
- Share of Voice % calculation across all platforms
- Full-page screenshot capture per platform per run
- Google Sheets sync with 5 structured tabs: overview, rankings, sources, trends, competitor_sov
- Run history with SOV% trend chart and rank timeline
- Multi-keyword support with per-keyword stats
- Scheduled automatic runs (set interval in hours)
- Headless mode — Chrome runs invisibly in background
- 7-step guided setup wizard for non-technical users
- Optional Anthropic API key integration for ~90% brand detection accuracy
- Auto-update notifications when new versions are released
- Browser Session Manager — refresh expired AI platform sessions without re-running full setup
