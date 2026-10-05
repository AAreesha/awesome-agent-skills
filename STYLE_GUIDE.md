# Awesome Agent Skills — README Style Guide

Reference aesthetic: [lobehub/lobe-chat](https://github.com/lobehub/lobe-chat) (now lobehub/lobehub), adapted for a curated awesome-list.

## Hard rules (Areesha)

- **No emojis** in headings, badges, blurbs, tables, or TOC.
- Professional, warm, editorial tone. No mascot language; every sentence earns its place.
- Self-host brand assets under `assets/`.
- Living categorized catalog + weekly archive under `weeks/`.
- Never invent skills or links. Every URL must resolve to the canonical source.

## Lobe-inspired patterns we keep

1. Full-width **banner graphic** at top (`assets/banner-dark.svg`). The banner carries the mark.
2. Centered hero: title, one-line tagline, harness line, nav links, **for-the-badge** shields with `labelColor=black`.
3. Collapsible TOC: `<details><summary><kbd>Table of contents</kbd></summary>` with a `#### TOC` heading.
4. Section rhythm: `---` dividers + right-aligned **BACK TO TOP** flat-square badge.
5. Clean **tables** for orientation, paths, labels, tracks, shelves, process, and ecosystem.
6. Numbered code-span steps (`` `01` ``, `` `02` ``) as a nod to lobe's `` `A` `` / `` `B` `` headings.
7. Footer link definitions (`[name-shield]: url`), sorted alphabetically.
8. GitHub callouts (`> [!NOTE]`, `[!TIP]`, `[!IMPORTANT]`) sparingly: at most one per section.

## Document order

1. Banner + centered hero + badges (no second logo under shields)
2. Three-step orientation table (`01` Find / `02` Install / `03` Stay current), above the TOC so it lands in the first screenful
3. TOC (details)
4. **Start here**: what a skill is, safety callout, **Pick your path** table (reader need → starter links → shelf anchor), **Reading an entry** (format, grouped labels table, inclusion bar in details)
5. **This week**: edition badges, `### Edition NN: Theme`, editorial paragraph, numbered track table, one TIP, link to `weeks/YYYY-MM-DD.md`, next-edition date
6. **Catalog**: shelf overview table (shelf, count, when to reach for it), then one `###` per shelf with an italic one-line intro
7. **How it works**: pipeline + stage table
8. **Ecosystem**: sources table
9. Contributing + License + centered footer line

## Catalog shelves (stable)

Keep these names and anchors stable week to week; they are linked from Pick your path, the TOC, and CONTRIBUTING.md.

| Shelf | Anchor |
| --- | --- |
| Standards and discovery | `#standards-and-discovery` |
| Coding workflows | `#coding-workflows` |
| Browser and testing | `#browser-and-testing` |
| Security and platforms | `#security-and-platforms` |
| Writing and design | `#writing-and-design` |
| Catalogs | `#catalogs` |

Entries are alphabetical within a shelf (case-insensitive).

## Entry format

```md
- **[Name](url)** - One precise sentence. `label` `label`
```

Labels: `official`, `multi`, `claude`, `cursor`, `browser`, `security`, `spec`, `catalog`. Add a new label only with a row in the labels table.

## Badges

- `style=for-the-badge&labelColor=black`. Cap the hero row at 6.
- Message colours come from the Stobri palette, alternated for rhythm: raspberry `BB4E6F`, pink `E8A4B8`, deep rose `7C2547`, cream `FFF9F4`.
- Plum `3D0B29` is reserved for the BACK TO TOP badge (too dark beside a black label for message text).
- Regenerate counts each Monday.

## Weekly checklist

1. Bump `skills`, `edition`, `WEEK`, `DATE`, `FOCUS`, and `PICKS` badges
2. Update the Catalog intro total and the shelf counts table
3. Rewrite This week: theme heading, editorial paragraph, track table, TIP, next-edition date
4. Revisit Pick your path only if a better starter appears
5. Archive to `weeks/YYYY-MM-DD.md` using the same shelf names, and add a row to `weeks/README.md`
6. Keep shelves stable; no emoji; verify every new URL resolves

## Branding (locked)

- Mark: **B — Stacked modules** (Stobri Studio palette)
- Palette: plum `#3D0B29`, deep rose `#7C2547`, raspberry `#BB4E6F`, pink `#E8A4B8`, cream `#FFF9F4`
- Assets: `assets/logo-mark.png`, `assets/logo.png`, `assets/banner-dark.svg` (default), `assets/banner-light.svg`
- Banner includes the mark — do **not** also place a separate logo under the shields
- Rejected: purple/cyan neural-node; indigo Ink+Signal system
