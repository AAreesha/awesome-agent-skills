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
[![][edition-shield]](weeks/2026-10-26.md)
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
> Skills run with your agent's permissions. Read the `SKILL.md` and any bundled scripts before you install, and prefer official org packs. `gh skill preview owner/repo skill` shows a skill's files without installing it, and for third-party packs a scanner such as [NVIDIA/SkillSpector](https://github.com/NVIDIA/SkillSpector) is worth running.

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

[![][week-badge]](weeks/2026-10-26.md)
[![][date-badge]](weeks/2026-10-26.md)
[![][focus-badge]](weeks/2026-10-26.md)
[![][picks-badge]](#this-week)

<br/>

### Edition 04: Checks and balances

The standard got a neutral home this week. The best new skills make agents prove their work.

</div>

On October 22, Anthropic [donated Agent Skills](https://www.anthropic.com/news/donating-agent-skills-to-the-agentic-ai-foundation) to the Agentic AI Foundation under the Linux Foundation, the same home as MCP. The format didn't change that day, but the proposed roadmap puts versioning and security guidance for skill authors and installers first. This edition follows the same idea at the level of a single skill: inspect what you install, have more than one model review the change, and check the output against something real before calling it done.

| # | Track | The shift | Featured |
| :-: | :-- | :-- | :-- |
| 1 | **Inspection** | Preview a skill's files before installing, pin a version, and update on purpose | [GitHub CLI: gh skill](https://cli.github.com/manual/gh_skill) |
| 2 | **Review** | Three models from three providers review a change, and the loop runs until they agree | [t3dotgg/tstack](https://github.com/t3dotgg/tstack) |
| 3 | **Idiom** | Write, review, and port idiomatic Rust, with a clippy config that enforces the rules in CI | [morganlinton/BeautifulRust](https://github.com/morganlinton/BeautifulRust) |
| 4 | **Migrations** | The agent edits the schema, and Atlas plans, lints, and tests the migration before it reports done | [ariga/atlas](https://github.com/ariga/atlas) |
| 5 | **Science** | 177 validated skills and 100+ scientific databases for biology, chemistry, medicine, and drug discovery | [K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills) |
| 6 | **Motion** | Rebuild a motion design clip as SVG and GSAP, checked frame by frame against the source | [lovisdotio/motion2code](https://github.com/lovisdotio/motion2code) |
| 7 | **Launch films** | A product film with its own score, where you click a frame to change it | [alchaincyf/huashu-motion](https://github.com/alchaincyf/huashu-motion) |

Also new to the catalog: [squirrelscan/skills](https://github.com/squirrelscan/skills), a website audit loop that checks 300+ rules, fixes in batches, and re-audits until the site scores well.

> [!TIP]
> Run `gh skill preview` on any pack in this edition before you install it. tstack, huashu-motion, and Motion2Code all run code on your machine.

**Full write-up:** [weeks/2026-10-26.md](weeks/2026-10-26.md), with cost and safety notes, the week's platform news, and honorable mentions. Edition 05 lands Monday, November 2.

<div align="right">

[![][back-to-top]](#readme-top)

</div>

---

## Catalog

50 entries across six shelves, alphabetical within each shelf. Entries stay until they stop meeting the [inclusion bar](#reading-an-entry).

| Shelf | Entries | Reach for it when |
| :-- | :-: | :-- |
| [Standards and discovery](#standards-and-discovery) | 5 | You are learning the format, or want the agent to find skills itself |
| [Coding workflows](#coding-workflows) | 12 | You want method, review gates, or framework-specific guidance |
| [Browser and testing](#browser-and-testing) | 4 | The agent needs to navigate, extract from, or test the web |
| [Security and platforms](#security-and-platforms) | 13 | You are auditing or reverse-engineering software, or building on a specific cloud, database, or commerce platform |
| [Writing and design](#writing-and-design) | 14 | The output is a document, an interface, a diagram, a video, a 3D scene, or prose |
| [Catalogs](#catalogs) | 2 | You want a wider index than this list keeps |

### Standards and discovery

*The format itself, the reference examples, the skill that finds other skills, the CLI that previews them, and the linter that checks them.*

- **[agent-sh/agnix](https://github.com/agent-sh/agnix)** - Linter and language server that validates `SKILL.md`, `AGENTS.md`, `CLAUDE.md`, hooks, and MCP configs, with auto-fix. `multi`
- **[agentskills.io Specification](https://agentskills.io/specification)** - Open `SKILL.md` standard for progressive disclosure, scripts, and assets. `spec`
- **[anthropics/skills](https://github.com/anthropics/skills)** - Official Anthropic examples plus `skill-creator`; the reference pattern. `official` `claude`
- **[find-skills](https://www.skills.sh/vercel-labs/skills/find-skills)** - Search and install skills mid-session from the open ecosystem. `cursor`
- **[GitHub CLI: gh skill](https://cli.github.com/manual/gh_skill)** - Search, preview, install, pin, and update skills from any GitHub repo for Copilot, Claude Code, Cursor, Codex, and more (public preview). `official` `multi`

### Coding workflows

*Engineering method, quality gates, evals, and framework guidance from the teams that maintain the frameworks.*

- **[addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)** - Production workflows with quality gates for review, APIs, performance, and shipping. `multi`
- **[confident-ai/eval-skills](https://github.com/confident-ai/eval-skills)** - Eval workflow from first inspectable trace to calibrated graders, repeatable runs, and regression gates. `multi`
- **[cursor/plugins: pstack](https://github.com/cursor/plugins/tree/main/pstack)** - Lauren Tan's daily engineering skills at Cursor: restate, plan, dig in, and verify, run through `poteto-mode`. `official` `cursor`
- **[expo/skills](https://github.com/expo/skills)** - Official Expo and EAS skills for native UI, Router, deployment, and upgrades. `official`
- **[K-Dense-AI/scientific-agent-skills](https://github.com/K-Dense-AI/scientific-agent-skills)** - 177 validated skills and 100+ scientific databases for biology, chemistry, medicine, and drug discovery. `multi`
- **[mattpocock/skills](https://github.com/mattpocock/skills)** - Practical engineering skills led by relentless plan stress-testing. `multi`
- **[morganlinton/BeautifulRust](https://github.com/morganlinton/BeautifulRust)** - Write, review, and port idiomatic Rust, distilled from five style guides, with a tested clippy config for CI. `multi`
- **[obra/superpowers](https://github.com/obra/superpowers)** - Agentic methodology: brainstorm, plan, TDD, and verify before shipping. `claude`
- **[robonuggets/be-ambitious](https://github.com/robonuggets/be-ambitious)** - Rewrites a task at a higher altitude, depth, or range, following Felix Rieseberg's framework, and ends with an outside check. `claude`
- **[t3dotgg/tstack](https://github.com/t3dotgg/tstack)** - PR skills that prove, review, file, babysit, and merge a change, with a three-provider `council` review. `multi`
- **[twostraws/SwiftUI-Agent-Skill](https://github.com/twostraws/SwiftUI-Agent-Skill)** - Modern SwiftUI guidance on APIs, performance, and accessibility, aimed at the mistakes LLMs actually make. `multi`
- **[vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)** - Official React and Next.js best practices, composition, and design guidelines. `official`

### Browser and testing

*Navigate, extract, and test the web.*

- **[anthropics/webapp-testing](https://officialskills.sh/anthropics/skills/webapp-testing)** - Playwright-based local webapp testing from the Anthropic examples. `official` `claude` `browser`
- **[firecrawl/cli](https://github.com/firecrawl/cli)** - Scrape, search, crawl, and interact skills via Firecrawl (API usage may be paid). `browser`
- **[squirrelscan/skills](https://github.com/squirrelscan/skills)** - Website audit loop over 300+ SEO, performance, security, and accessibility rules: fix in batches, re-audit until it passes (needs the squirrel CLI). `browser`
- **[vercel-labs/agent-browser](https://github.com/vercel-labs/agent-browser)** - Browser automation CLI and skills to navigate, fill, extract, and screenshot. `official` `browser`

### Security and platforms

*Security research and reverse engineering, plus official guidance for the clouds, databases, and commerce platforms agents build on.*

- **[ariga/atlas](https://github.com/ariga/atlas)** - Official Atlas skills: the agent edits the desired schema, and Atlas plans, lints, and tests the migration across 10+ databases. `official` `multi`
- **[aws/agent-toolkit-for-aws](https://github.com/aws/agent-toolkit-for-aws)** - Official AWS skills, plugins, and MCP servers for building, deploying, and running on AWS, including SageMaker AI and Airflow. `official` `multi`
- **[cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill)** - Six-phase security audit where isolated agents hunt, then fresh verifiers try to disprove every finding. `official` `security`
- **[cloudflare/skills](https://github.com/cloudflare/skills)** - Workers, Durable Objects, Wrangler, and Agents SDK best practices. `official`
- **[google/skills](https://github.com/google/skills)** - Official skills and plugins for Google Cloud, BigQuery, the gcloud CLI, and other Google developer products. `official` `multi`
- **[microsoft/azure-skills](https://github.com/microsoft/azure-skills)** - Official Azure plugin pairing deploy, diagnostics, and cost skills with the Azure MCP Server. `official` `multi`
- **[morluto/rea](https://github.com/morluto/rea)** - Reverse Engineer Anything: an MCP server and skill for analyzing apps, runtime behavior, and native binaries. `security` `multi`
- **[neondatabase/agent-skills](https://github.com/neondatabase/agent-skills)** - Neon Serverless Postgres patterns for branching, egress, and claimable databases. `official`
- **[NVIDIA/skills](https://github.com/NVIDIA/skills)** - Verified NVIDIA catalog for CUDA-X, robotics, simulation, and RAG workflows, synced daily from product repos. `official` `multi`
- **[prisma/skills](https://github.com/prisma/skills)** - Prisma ORM 7 CLI reference, v6-to-v7 upgrade path, and client API guidance. `official`
- **[Shopify/shop](https://github.com/Shopify/shop)** - Official Shop skill and MCP for catalog search, carts, Shop Pay checkout after shopper approval, and order tracking. `official` `multi`
- **[supabase/agent-skills](https://github.com/supabase/agent-skills)** - Postgres and Supabase guidance with a focus on RLS and performance. `official`
- **[trailofbits/skills](https://github.com/trailofbits/skills)** - Security research: static analysis, Semgrep, and differential review. `official` `security`

### Writing and design

*Documents, interface craft, diagrams, motion, marketing, video, 3D, and prose.*

- **[alchaincyf/huashu-motion](https://github.com/alchaincyf/huashu-motion)** - Product launch films with a locally generated score and a browser editor where you click a frame to change it. `multi`
- **[Anthropic document skills](https://docs.anthropic.com/en/docs/agents-and-tools/agent-skills/overview)** - Pre-built pptx, xlsx, docx, and pdf creation and editing on Claude. `official` `claude`
- **[anthropics/frontend-design](https://officialskills.sh/anthropics/skills/frontend-design)** - High-signal frontend and UI skill with strong install traction. `official` `claude`
- **[coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)** - SaaS marketing stack: SEO, CRO, copy, launch, pricing, and ads. `multi`
- **[EL4CTEO/blender-skills](https://github.com/EL4CTEO/blender-skills)** - 22 Blender 5.2 skills covering modeling, UVs, PBR, rigging, animation, export, and QA, each script tested in real Blender. `multi`
- **[emilkowalski/skills](https://github.com/emilkowalski/skills)** - Animation and interface craft from a design engineer, listing the small mistakes agents make and how to fix them. `multi`
- **[heygen-com/hyperframes](https://github.com/heygen-com/hyperframes)** - HTML-to-MP4 video framework with 21 skills covering planning, animation, media, and rendering. `official` `multi`
- **[juliobsz/skills](https://github.com/juliobsz/skills)** - `/awwwards` builds a site from one line and checks it in a real browser; `/jury` scores any site like an awards jury. `multi`
- **[Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill)** - Anti-slop frontend skills that push agents past generic layouts toward premium interfaces. `multi`
- **[lovisdotio/motion2code](https://github.com/lovisdotio/motion2code)** - Rebuilds a motion design video as looping SVG and GSAP code, checked frame by frame against the source. `multi`
- **[pbakaus/impeccable](https://github.com/pbakaus/impeccable)** - One design skill with 24 commands and 59 deterministic detector rules for AI-generated frontends. `multi`
- **[petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop)** - Removes 20+ AI writing patterns while keeping your voice, and lists every change. `multi`
- **[remotion-dev/skills](https://github.com/remotion-dev/skills)** - Programmatic video-with-React skills from the Remotion team. `official`
- **[tt-a1i/archify](https://github.com/tt-a1i/archify)** - Turns an idea, plan, or codebase into an interactive, source-linked HTML diagram you can refine and share. `multi`

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
| agentskills.io | Open skill format specification, now under the Agentic AI Foundation | [Specification](https://agentskills.io/specification) |
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
[date-badge]: https://img.shields.io/badge/DATE-2026.10.26-E8A4B8?style=for-the-badge&labelColor=black
[edition-shield]: https://img.shields.io/badge/edition-04_%C2%B7_2026.10.26-7C2547?style=for-the-badge&labelColor=black
[focus-badge]: https://img.shields.io/badge/FOCUS-checks_and_balances-BB4E6F?style=for-the-badge&labelColor=black
[license-shield]: https://img.shields.io/badge/license-CC0--1.0-FFF9F4?style=for-the-badge&labelColor=black
[picks-badge]: https://img.shields.io/badge/PICKS-07-FFF9F4?style=for-the-badge&labelColor=black
[pr-welcome-shield]: https://img.shields.io/badge/submit_a_skill-%E2%86%92-BB4E6F?style=for-the-badge&labelColor=black
[prs-shield]: https://img.shields.io/badge/PRs-welcome-BB4E6F?style=for-the-badge&labelColor=black
[skills-shield]: https://img.shields.io/badge/skills-50-E8A4B8?style=for-the-badge&labelColor=black
[week-badge]: https://img.shields.io/badge/WEEK-04-7C2547?style=for-the-badge&labelColor=black
[weekly-shield]: https://img.shields.io/badge/cadence-weekly-BB4E6F?style=for-the-badge&labelColor=black
