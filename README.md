# sintel-report

Morning-scan handoff for the Daily Intel Report (evening briefing).

## Lanes

- `grok-scans/YYYY-MM-DD.md` — Grok's morning X-native scan (breaking items,
  founder/builder announcements, insider chatter). Date = US Eastern scan date.
- `gemini-scans/YYYY-MM-DD.md` — Gemini's morning Google-web scan (official
  announcements, tech press, analyst/engineering writeups).

## Contract

- One file per lane per day. If a scan is re-run the same day, overwrite.
- The evening compiler (Pip) pulls both lanes, verifies every claim against
  real sources, and folds the solid ones into the edition. Scan items are
  leads, not facts.
- If a lane misses a day, the edition ships anyway — the gap gets one line.
