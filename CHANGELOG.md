# Changelog

## 3.0.1

- Fix Figma auto-layout error during Home generation: `layoutSizingHorizontal = FILL` is now applied only after `Home Composer` is attached to its auto-layout parent.
- Add regression coverage that reproduces Figma's `FILL can only be set on children of auto-layout frames` rule.

## 3.0.0

- GitHub-backed remote screen definitions
- Remote design token overrides
- One-click `GitHub 최신 버전 불러오기`
- Automatic remote sync before screen generation
- Local bundled defaults when GitHub is temporarily unavailable
