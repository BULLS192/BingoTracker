# BingoTracker

Mobile-first 75-ball bingo card monitor.

## V0.3

- Practical unlimited card count (no 20-card hard cap)
- One-tap called-number entry across all cards
- Timestamped call history
- Round start/end time and duration tracking
- Per-call card progress snapshots
- 1-away and BINGO alerts
- Single line, four corners, X, outside frame, blackout, and custom patterns
- Photo capture/upload with browser-side OCR
- Original card photo retained locally with the round archive
- Session and round history stored locally for offline-first reliability
- JSON session export containing rounds, cards, calls, duration, patterns, near-miss progress, results, and retained photo data
- Direct link to the user's BingoTracker Google Drive archive folder
- Responsive mobile/PWA layout

## Storage model

Live play is local/offline-first. No Supabase dependency is required. The exported session JSON is intended to be archived in Google Drive. The app does not embed Google credentials or automatically upload to Drive from the public static site.

## Live deployment

Render watches `main` and auto-deploys commits to the live site.
