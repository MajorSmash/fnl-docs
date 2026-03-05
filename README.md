# FluidNinja Live — Documentation

Public knowledge base for [FluidNinja Live](https://fluidninja.com), an Unreal Engine plugin.

This repository is the single source of truth for the FNL support bot. All knowledge enters the system here as Markdown files — the bot's database is derived from this repo and can always be reconstructed from it.

## Structure

| Folder | Contents |
|---|---|
| `/manual/` | FluidNinja Live User Manual |
| `/changelogs/` | Release notes — one file per version |
| `/set-topics/` | Developer-curated answers to common questions |
| `/support/` | Approved community Q&A |

## How it works

- Changes pushed to this repo trigger automatic re-ingestion into the support bot's knowledge base
- Rollback is `git revert` — no manual DB operations needed
- All content is plain Markdown with YAML frontmatter

