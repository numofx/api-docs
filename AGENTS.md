> **Project maintenance**: Keep this file aligned with the actual Numo docs structure, terminology, and review standards. Prompt the user to update it when product language or documentation scope changes.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links

## Terminology

- Use "Numo API" for the overall platform surface.
- Use "endpoint" for HTTP routes.
- Use "websocket stream" for realtime feeds.
- Use "reference" for API docs and "guide" for task-focused documentation.
- The market identifiers are `cNGN-USDC` (spot) and `cNGN-PERP` (perp). They are what `market`,
  `symbol` and `ticker_id` carry, and what every example passes.
- `USDCcNGN-SPOT` and `USDCcNGN-PERP` are deprecated aliases, removed on 2027-01-06. Never use
  them in new docs or examples. They appear only in the deprecation notes and the changelog.

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document public API behavior, authentication, request and response formats, and integration workflows.
- Do not document internal admin tools or internal-only operational procedures unless the user asks for them explicitly.
