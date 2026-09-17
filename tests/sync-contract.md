# v3 sync contract

- `version.json` uses `schemaVersion: 1` and lists the five screen keys.
- `design/tokens.json` may override shared design tokens.
- Each `screens/*.json` file uses `schemaVersion: 1` and an exact `key` matching its file.
- The bootstrap plugin fetches only from `raw.githubusercontent.com/kovemu/ai-video-community-builder/main`.
- If remote sync fails during an ordinary build, the plugin falls back to bundled defaults; explicit GitHub sync reports the error.
