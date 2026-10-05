<div align="center" id="readme-top">

[![][banner-image]](#readme-top)

# Awesome Agent Skills

Hand-picked, verified skill packs for AI coding agents. One short catalog, refreshed every Monday.

Built for Cursor, Claude Code, Codex, and any harness that speaks the open [Agent Skills](https://agentskills.io/specification) format.

[Start here](#start-here) · [Pick your path](#pick-your-path) · [This week](#this-week) · [Catalog](#catalog) · [Archive](weeks/) · [Contribute](#contributing)

<br/>

[![][awesome-shield]][awesome-link]
[![][weekly-shield]](#this-week)
[![][skills-shield]](#catalog)
[![][edition-shield]](weeks/2026-10-05.md)
[![][prs-shield]](#contributing)
[![][license-shield]](#license)

<br/>

**Skills that compound. Agents that level up.**

</div>

<br/>

| `01` Find | `02` Install | `03` Stay current |
| :-- | :-- | :-- |
| Choose a row in [Pick your path](#pick-your-path), or scan the [Catalog](#catalog) by label. | Most GitHub packs install with `npx skills add owner/repo`. Read the `SKILL.md` first. | A new edition lands every Monday. Past editions live in [`weeks/`](weeks/). |

<details>
<summary><kbd>Table of contents</kbd></summary>

#### TOC

- [Start here](#start-here)
  - [Pick your path](#pick-your-path)
  - [Reading an entry](#reading-an-entry)
- [This week](#this-week)
- [Catalog](#catalog)
  - [Standards and discovery](#standards-and-discovery)
  - [Coding workflows](#coding-workflows)
  - [Browser and testing](#browser-and-testing)
  - [Security and platforms](#security-and-platforms)
  - [Writing and design](#writing-and-design)
  - [Catalogs](#catalogs)
- [How it works](#how-it-works)
- [Ecosystem](#ecosystem)
- [Contributing](#contributing)
- [License](#license)

####

</details>

<br/>

---

## Start here

A skill is a folder of instructions, and sometimes scripts or assets, that an agent loads only when a task calls for it. Good skills change how an agent works: how it plans, checks its own output, and uses its tools. This list keeps the short, verified set worth installing, and leaves out prompt pastebins, mirrors, and unmaintained dumps.

> [!IMPORTANT]
> Skills run with your agent's permissions. Read the `SKILL.md` and any bundled scripts before you install, and prefer official org packs. For third-party packs, a scanner such as [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) is worth running.

### Pick your path

| If you are... | Start with | Then browse |
| :-- | :-- | :-- |
| **New to skills** | [agentskills.io Specification](https://agentskills.io/specification), then [anthropics/skills](https://github.com/anthropics/skills) | [Standards and discovery](#standards-and-discovery) |
| **Shipping code every day** | [obra/superpowers](https://github.com/obra/superpowers) for method, [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) for production gates | [Coding workflows](#coding-workflows) |
| **Putting your agent on the web** | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) for automation, [anthropics/webapp-testing](https://officialskills.sh/anthropics/skills/webapp-testing) for local QA | [Browser and testing](#browser-and-testing) |
| **Hardening code or infrastructure** | [trailofbits/skills](https://github.com/trailofbits/skills) for security review, [cloudflare/skills](https://github.com/cloudflare/skills) for the edge | [Security and platforms](#security-and-platforms) |
| **Making documents, UI, or launches** | [Anthropic document skills](https://docs.anthropic.com/en/docs/agents-and-tools/agent-skills/overview), [anthropics/frontend-design](https://officialskills.sh/anthropics/skills/frontend-design) | [Writing and design](#writing-and-design) |
| **Surveying the whole field** | [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) | [Catalogs](#catalogs) |

### Reading an entry

Every entry follows one shape: name and canonical link, one sentence on what it does, then labels.

```md
- **[Name](https://github.com/owner/repo)** - What it does, in one sentence. `label` `label`
```

| Group | Label | Meaning |
| :-- | :-- | :-- |
| Source | `official` | Published by the vendor or foundation that owns the product |
| Harness | `multi` | Works across more than one agent harness |
| Harness | `claude` / `cursor` | Strongest fit for that harness |
| Domain | `browser` | Web navigation, scraping, or UI testing |
| Domain | `security` | Hardening, review, or security research |
| Type | `spec` | Standards and skill-format documentation |
| Type | `catalog` | An index of many skills, not a single pack |

<details>
<summary><kbd>Inclusion bar</kbd></summary>

<br/>

An entry makes the list only if all four hold:

- Public repo or clear install docs
- A real skill pack, plugin, or reusable agent workflow (`SKILL.md` or equivalent)
- Describable in one honest sentence
- Canonical URL only: no mirrors, no invented links

Paid or API-backed tools are allowed when the entry says so.

</details>

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

## This week

<div align="center">

[![][week-badge]](weeks/2026-10-05.md)
[![][date-badge]](weeks/2026-10-05.md)
[![][focus-badge]](weeks/2026-10-05.md)
[![][picks-badge]](#this-week)

<br/>

### Edition 01: Foundations

A first edition has one job: set the floor.

</div>

These seven picks are the packs to install before anything else. Each one changes how an agent works, not just what it knows. Read in order, they trace a single working session: learn the format, find the right skill, plan, challenge the plan, build to a standard, reach the web, and audit what shipped.

| # | Track | The shift | Featured |
| :-: | :-- | :-- | :-- |
| 1 | **Reference** | Learn the format from the team that wrote it | [anthropics/skills](https://github.com/anthropics/skills) |
| 2 | **Discovery** | An agent that finds its own skills stops waiting on you | [find-skills](https://www.skills.sh/vercel-labs/skills/find-skills) |
| 3 | **Method** | Brainstorm, plan, test, verify: structure over improvisation | [obra/superpowers](https://github.com/obra/superpowers) |
| 4 | **Stress-test** | Weak plans fail in conversation, not in production | [mattpocock/skills](https://github.com/mattpocock/skills) · [grill-me](https://www.skills.sh/mattpocock/skills/grill-me) |
| 5 | **Engineering** | Review, API, performance, and shipping gates the agent holds itself to | [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) |
| 6 | **Reach** | The browser becomes a workspace, with no custom glue scripts | [vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser) |
| 7 | **Hardening** | Security review patterns an agent can actually run | [trailofbits/skills](https://github.com/trailofbits/skills) |

> [!TIP]
> Short on time? Install tracks 2 and 3 first. Discovery lets the agent fetch the rest when it needs them, and Method makes everything after it more reliable.

**Full write-up:** [weeks/2026-10-05.md](weeks/2026-10-05.md), with cost notes, sources to watch, and honorable mentions. Edition 02 lands Monday, October 12.

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

## Catalog

21 entries across six shelves, alphabetical within each shelf. Entries stay until they stop meeting the [inclusion bar](#reading-an-entry).

| Shelf | Entries | Reach for it when |
| :-- | :-: | :-- |
| [Standards and discovery](#standards-and-discovery) | 3 | You are learning the format, or want the agent to find skills itself |
| [Coding workflows](#coding-workflows) | 5 | You want method, review gates, or framework-specific guidance |
| [Browser and testing](#browser-and-testing) | 3 | The agent needs to navigate, extract from, or test the web |
| [Security and platforms](#security-and-platforms) | 4 | You are auditing code or building on a specific cloud or database |
| [Writing and design](#writing-and-design) | 4 | The output is a document, an interface, a campaign, or a video |
| [Catalogs](#catalogs) | 2 | You want a wider index than this list keeps |

### Standards and discovery

*The format itself, the reference examples, and the skill that finds other skills.*

- **[agentskills.io Specification](https://agentskills.io/specification)** - Open `SKILL.md` standard for progressive disclosure, scripts, and assets. `spec`
- **[anthropics/skills](https://github.com/anthropics/skills)** - Official Anthropic examples plus `skill-creator`; the reference pattern. `official` `claude`
- **[find-skills](https://www.skills.sh/vercel-labs/skills/find-skills)** - Search and install skills mid-session from the open ecosystem. `cursor`

### Coding workflows

*Engineering method, quality gates, and framework guidance from the teams that maintain the frameworks.*

- **[addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)** - Production workflows with quality gates for review, APIs, performance, and shipping. `multi`
- **[expo/skills](https://github.com/expo/skills)** - Official Expo and EAS skills for native UI, Router, deployment, and upgrades. `official`
- **[mattpocock/skills](https://github.com/mattpocock/skills)** - Practical engineering skills led by relentless plan stress-testing. `multi`
- **[obra/superpowers](https://github.com/obra/superpowers)** - Agentic methodology: brainstorm, plan, TDD, and verify before shipping. `claude`
- **[vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)** - Official React and Next.js best practices, composition, and design guidelines. `official`

### Browser and testing

*Navigate, extract, and test the web.*

- **[anthropics/webapp-testing](https://officialskills.sh/anthropics/skills/webapp-testing)** - Playwright-based local webapp testing from the Anthropic examples. `official` `claude` `browser`
- **[firecrawl/cli](https://github.com/firecrawl/cli)** - Scrape, search, crawl, and interact skills via Firecrawl (API usage may be paid). `browser`
- **[vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser)** - Browser automation CLI and skills to navigate, fill, extract, and screenshot. `official` `browser`

### Security and platforms

*Security research, plus official guidance for the clouds and databases agents deploy to.*

- **[cloudflare/skills](https://github.com/cloudflare/skills)** - Workers, Durable Objects, Wrangler, and Agents SDK best practices. `official`
- **[neondatabase/agent-skills](https://github.com/neondatabase/agent-skills)** - Neon Serverless Postgres patterns for branching, egress, and claimable databases. `official`
- **[supabase/agent-skills](https://github.com/supabase/agent-skills)** - Postgres and Supabase guidance with a focus on RLS and performance. `official`
- **[trailofbits/skills](https://github.com/trailofbits/skills)** - Security research: static analysis, Semgrep, and differential review. `official` `security`

### Writing and design

*Documents, interface craft, marketing, and media.*

- **[Anthropic document skills](https://docs.anthropic.com/en/docs/agents-and-tools/agent-skills/overview)** - Pre-built pptx, xlsx, docx, and pdf creation and editing on Claude. `official` `claude`
- **[anthropics/frontend-design](https://officialskills.sh/anthropics/skills/frontend-design)** - High-signal frontend and UI skill with strong install traction. `official` `claude`
- **[coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)** - SaaS marketing stack: SEO, CRO, copy, launch, pricing, and ads. `multi`
- **[remotion-dev/skills](https://github.com/remotion-dev/skills)** - Programmatic video-with-React skills from the Remotion team. `official`

### Catalogs

*Indexes of many skills. Start here when this list is too narrow.*

- **[heilcheng/awesome-agent-skills](https://github.com/heilcheng/awesome-agent-skills)** - Tutorials, a platform docs map, and discovery pointers. `catalog`
- **[VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)** - Large curated index of official team skills across major vendors. `catalog`

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

## How it works

> [!NOTE]
> The README is the living catalog. Each Monday's edition is archived as a dated file under [`weeks/`](weeks/), so history stays readable and the catalog stays short.

```text
  discover ──► filter ──► publish ──► archive
     │            │           │           │
  skills.sh    installable  README     weeks/
  official     documented   + labels   YYYY-MM-DD.md
  org packs    canonical
```

| Stage | What happens | Output |
| :-- | :-- | :-- |
| **Discover** | Watch skills.sh, official org packs, and trusted indexes | Candidate list |
| **Filter** | Keep installable, documented skills; drop pastebins and mirrors | Curated shortlist |
| **Publish** | Update the catalog and pick the week's featured tracks | This README |
| **Archive** | Ship a dated edition with narrative, sources, and cost notes | [`weeks/`](weeks/) |

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

## Ecosystem

The sources behind each edition, checked every week.

| Source | Role | Link |
| :-- | :-- | :-- |
| skills.sh | Install leaderboard and discovery | [skills.sh](https://www.skills.sh/) |
| agentskills.io | Open skill format specification | [Specification](https://agentskills.io/specification) |
| officialskills.sh | Index of official org skills | [officialskills.sh](https://officialskills.sh/) |
| VoltAgent awesome list | Curated official team packs | [VoltAgent/awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills) |
| Cursor docs | Platform skill APIs and built-ins | [cursor.com/docs/skills](https://cursor.com/docs/skills) |
| Anthropic docs | Agent Skills product overview | [docs.anthropic.com](https://docs.anthropic.com/en/docs/agents-and-tools/agent-skills/overview) |

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

## Contributing

Know a skill that belongs here? Open a pull request that adds **one entry** to the right shelf, in alphabetical order:

```md
- **[Name](https://github.com/owner/repo)** - One precise sentence. `label` `label`
```

Link the canonical source, use labels from [Reading an entry](#reading-an-entry), and say in the PR why it clears the inclusion bar. The full checklist is in [CONTRIBUTING.md](CONTRIBUTING.md).

[![][pr-welcome-shield]](CONTRIBUTING.md)

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

The list is dedicated to the public domain under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). Each linked skill keeps its own license.

---

<div align="center">

**New edition every Monday** · Archive in [weeks/](weeks/) · Inspired by [sindresorhus/awesome](https://github.com/sindresorhus/awesome) · Style nods to [lobehub/lobe-chat](https://github.com/lobehub/lobe-chat)

</div>

<!-- MARKDOWN LINKS & IMAGES -->

[awesome-link]: https://github.com/sindresorhus/awesome
[awesome-shield]: https://cdn.jsdelivr.net/gh/sindresorhus/awesome@d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg
[back-to-top]: https://img.shields.io/badge/-BACK_TO_TOP-3D0B29?style=flat-square
[banner-image]: ./assets/banner-dark.svg
[date-badge]: https://img.shields.io/badge/DATE-2026.10.05-E8A4B8?style=for-the-badge&labelColor=black
[edition-shield]: https://img.shields.io/badge/edition-01_%C2%B7_2026.10.05-7C2547?style=for-the-badge&labelColor=black
[focus-badge]: https://img.shields.io/badge/FOCUS-foundations-BB4E6F?style=for-the-badge&labelColor=black
[license-shield]: https://img.shields.io/badge/license-CC0--1.0-FFF9F4?style=for-the-badge&labelColor=black
[picks-badge]: https://img.shields.io/badge/PICKS-07-FFF9F4?style=for-the-badge&labelColor=black
[pr-welcome-shield]: https://img.shields.io/badge/submit_a_skill-%E2%86%92-BB4E6F?style=for-the-badge&labelColor=black
[prs-shield]: https://img.shields.io/badge/PRs-welcome-BB4E6F?style=for-the-badge&labelColor=black
[skills-shield]: https://img.shields.io/badge/skills-21-E8A4B8?style=for-the-badge&labelColor=black
[week-badge]: https://img.shields.io/badge/WEEK-01-7C2547?style=for-the-badge&labelColor=black
[weekly-shield]: https://img.shields.io/badge/cadence-weekly-BB4E6F?style=for-the-badge&labelColor=black
