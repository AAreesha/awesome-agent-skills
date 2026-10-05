# Contributing

Thanks for helping keep this list useful. This repo is a **curated** awesome-list of real agent skills — not an exhaust dump of every prompt on the internet.

## How to suggest a skill

1. **Open a PR** that adds one line to the right shelf in [`README.md`](README.md), in alphabetical order:
   ```md
   - **[Name](https://github.com/owner/repo)** - One precise sentence. `label` `label`
   ```
   Use labels from the [Reading an entry](README.md#reading-an-entry) table. Current shelves: Standards and discovery, Coding workflows, Browser and testing, Security and platforms, Writing and design, Catalogs.
2. Optionally mention it in the latest (or next) file under [`weeks/`](weeks/) if it belongs in that week's roundup.
3. In the PR description, include:
   - Why it belongs (what problem it solves for agents)
   - Confirmation the link works and points at a real skill pack / official docs
   - License / cost notes if anything is paid or closed

Issues are fine for discussion, but **PRs with the exact markdown line** are preferred.

## Quality bar

**Include when:**

- There is a real `SKILL.md` (or equivalent Agent Skills pack), or an **official** org/docs page for a skill
- The pack is installable or clearly documented for Cursor / Claude Code / Codex / compatible agents
- Free and open source is strongly preferred; paid/API-backed tools are OK if labeled honestly
- The blurb is accurate and specific (not marketing fluff)

**Do not include:**

- Invented, placeholder, or broken links
- One-off prompt pastebins with no repo / no `SKILL.md`
- Unverified “AI-slop” catalogs that rehost others without adding signal
- Skills you have not at least skimmed (README / SKILL.md / docs)

When in doubt, prefer linking an official org pack over a third-party mirror.

## PR style

- One skill (or one tight cluster) per PR when possible
- Use the exact entry format above: bold linked name, ` - `, one sentence ending in a period, then backticked labels
- Match existing shelf names; propose a new shelf only if nothing fits
- Do not add badges, images, or emojis to entries
- Prefer present-tense, concrete blurbs under ~120 characters
- If you add an entry, bump the `skills` badge, the total in the Catalog intro, and the shelf count in the Catalog table
- Do not rearrange the whole list unless there is a clear reason

## Weekly editions

The living master list lives in `README.md`. Deeper context (sources to watch, honorable mentions) goes in `weeks/YYYY-MM-DD.md`. See [`weeks/README.md`](weeks/README.md).

## License

Contributions are dedicated to the public domain under [CC0 1.0](license).
