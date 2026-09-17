# AI Video Community Builder

Figma classic plugin and remote screen-definition source for the AI Video Community platform.

## Architecture

- `plugin/` — locally installed Figma renderer/bootstrap plugin
- `screens/` — remotely editable screen definitions
- `design/` — shared design tokens
- `version.json` — remote schema/version metadata

GitHub is the source of truth for versioning and review. Runtime distribution to the Figma plugin is designed to use a read-only public endpoint rather than embedding GitHub credentials in the plugin.
