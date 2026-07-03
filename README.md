# Illegalcord Website

This folder contains the Mintlify documentation site for Illegalcord.

The website is intentionally separate from the client build. It has its own `docs.json` and MDX pages, while the Illegalcord source continues to build from the repository root with `pnpm`.

The site links to:

- Illegalcord source code: https://github.com/ImHisako/Illegalcord
- Illegalcord installer: https://github.com/ImHisako/IllegalcordInstaller

## Local preview

From the repository root:

```bash
cd "Illegalcord Website"
npx mintlify dev
```

Mintlify serves the docs at `http://localhost:3000`.

## Structure

- `docs.json` configures the theme, logo, colors, and navigation.
- `index.mdx` is the landing page.
- `source-structure.mdx` maps the docs to the Illegalcord repository layout.
- `customization/` documents settings, plugins, and themes.
- `features/` documents user-facing capabilities backed by the local source.
- `plugin-dev/` documents how to build plugins inside this codebase.
- `troubleshooting/` covers build, inject, update, and uninstall recovery.

## Source alignment

When updating these docs, prefer commands and APIs that exist in the local repository:

- `src/plugins` for stock Vencord plugins.
- `src/equicordplugins` for Equicord-specific plugins.
- `src/userplugins` for Illegalcord-specific bundled plugins.
- `src/api`, `src/components`, `src/utils`, and `src/webpack` for shared plugin APIs.
- `browser` for web extension and userscript entry points.
- `scripts` for build, installer, lint, and plugin metadata generation.
