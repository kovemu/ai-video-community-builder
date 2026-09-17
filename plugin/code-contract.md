# Renderer contract

The installed v3 renderer:

1. fetches `version.json` and `design/tokens.json`,
2. fetches each screen path listed by the version manifest,
3. validates `schemaVersion` and screen keys,
4. applies remote design tokens,
5. regenerates the managed `[AIVC]` frames from the remote data,
6. keeps local bundled defaults as a fallback if the network is unavailable.

Routine design/content edits should therefore target `design/` and `screens/`, not the local installer.
