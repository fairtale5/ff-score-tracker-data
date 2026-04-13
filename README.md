# ff-score-tracker-data

This repository holds **offline backups** of FastFox ScoreTracker lap data: dated snapshots pulled from the VPS (`/opt/redline/score-tracker/`), plus any other snapshot folders we add here.

Each top-level folder named like `YYYY-MM-DD` is one **full tree** (per-server subfolders, `laptimes/`, `records.json`, etc.) as written by [ScoreTrackerPlugin](https://github.com/fairtale5/ScoreTrackerPlugin).

The main FastFox game/config monorepo **does not track** these bytes anymore; it keeps this path on disk for local dev and points `SCORE_TRACKER_ROOT` (or the backup script) at `servers/score-tracker-history/<date>/`.
