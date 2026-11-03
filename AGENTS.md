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
- The market identifiers are `cNGN-USDC` (spot) and `<BASE>-<DDMONYY>` for each futures series,
  currently `cNGN-30NOV26` and `EURC-30NOV26`. They are what `market`, `symbol` and `ticker_id` carry,
  and what every example passes. A future is quoted in USDC per unit of the base, and one unit of
  size is 0.001 contract.
- `USDC-cNGN-30NOV26` is the retired, close-only series, quoted in cNGN per USDC. Mention it only to
  say so.
- Trading accounts sit under the MarginEngine (`0x0705219a1594d5Fc5dC2573da4082cAf3e1B0950`). The first engine,
  `0xA19E296021c9DF25b90D96C2A0793CC3D0800758`, is close-only. The
  perpetual (`cNGN-PERP`) is not documented; do not add it back.
- `USDCcNGN-SPOT` is a deprecated alias, removed on 2027-01-06. Never use it in new docs or
  examples. It appears only in the deprecation notes.

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document public API behavior, authentication, request and response formats, and integration workflows.
- Do not document internal admin tools or internal-only operational procedures unless the user asks for them explicitly.
