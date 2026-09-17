# Figma plugin

The v3 bootstrap plugin reads `version.json`, `design/tokens.json`, and the five `screens/*.json` files from the repository's public `main` branch. The local Figma plugin only needs to be installed once; routine UI/content changes are made in GitHub and pulled with **GitHub 최신 버전 불러오기**.

`manifest.json` allows network access only to `https://raw.githubusercontent.com`.
