# Illegalcord Website instructions

## About this project

- This is a Mintlify documentation site stored in `Illegalcord Website/`.
- Pages are MDX files with YAML frontmatter.
- Site configuration lives in `docs.json`.
- The docs folder is separate from the Illegalcord TypeScript build and is not part of `pnpm-workspace.yaml`.

## Product terminology

- Use `Illegalcord` for the fork documented by this site.
- Use `Equicord` and `Vencord` only when describing upstream source layout, inherited APIs, or credits.
- Use `QuickCSS`, not `Custom CSS`, when referring to the built-in editor exposed by the client.
- Use `Illegalcord Settings`, `Plugins`, `Themes`, `Updater`, `Cloud`, and `Backup & Restore` for settings tabs, matching `src/plugins/_core/settings.tsx`.
- Use `stock plugins` for plugins in `src/plugins`, `Equicord plugins` for `src/equicordplugins`, and `Illegalcord plugins` for `src/userplugins`.

## Writing style

- Use active voice and second person.
- Keep sentences concise.
- Use sentence case for headings.
- Bold UI labels, for example **Plugins**.
- Use code formatting for file names, commands, paths, setting names, and APIs.
- Do not document features that are not visible in the local source tree.
- Prefer source-backed commands such as `pnpm build`, `pnpm buildWeb`, `pnpm inject`, `pnpm uninject`, and `pnpm repair`.
