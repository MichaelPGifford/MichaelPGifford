<h1 align="center">Michael Gifford</h1>

<p align="center">
  <b>Full-Stack &amp; Product Engineer</b> · Nashville, TN · Remote<br>
  I ship revenue-generating web platforms and the data pipelines that feed them —
  Next.js/React on the front, Python/FastAPI and LLM-backed extraction on the back.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white" alt="Next.js">
  <img src="https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB" alt="React">
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/GCP-4285F4?style=flat&logo=googlecloud&logoColor=white" alt="GCP">
</p>

---

Versatile full-stack engineer with a track record of **architecting
revenue-generating platforms**, owning complex data structures, and running
end-to-end system lifecycles. I lean hard on modern AI-assisted engineering
(Cursor, Claude, the OpenAI API) to ship high-quality code fast — from
high-volume ingestion pipelines to server-rendered, SEO-first public sites.

> **A note on what's public here.** My current commercial platform and the
> proprietary pipeline behind it live in **private repositories** for
> confidentiality and IP reasons. The public repos below are the genuine pieces
> I can share — recent tooling, a full financial-data platform, reusable
> libraries genericized from production patterns, and a 1st-place hackathon
> build. Happy to walk through the private work in an interview.

## What I focus on

- **Full-stack product engineering** — Next.js (App Router, RSC, TypeScript)
  frontends backed by Node.js and async Python / FastAPI services.
- **Data pipelines at scale** — scraping, normalization, and LLM-based
  structured extraction with deterministic, cache-first, retry-resilient designs
  (built one processing **9,200+ target sites** in concurrent batches).
- **SEO-first public sites** — server-rendered, structured-data-rich pages
  designed to scale to thousands of crawlable URLs.

## Featured projects

### 🎯 guidedhunts.io — *Founder &amp; Lead Engineer* (private)
A programmatic aggregator platform (Next.js + Python) that ingests and structures
the entire U.S. hunting-outfitter market — packages, pricing, photos, and
reviews. High-volume extraction pipelines (Firecrawl + DataForSEO) run
cost-controlled annual refreshes across 9,200+ sites. Core platform is private;
the tool below is a public artifact from that work.

### [`serp-gap-analyzer`](https://github.com/MichaelPGifford/serp-gap-analyzer) · JavaScript
Mechanical SERP gap analysis for the platform's target keywords: it queries
SerpApi, **classifies who actually ranks** (directory / operator / content),
infers search intent, and emits a static, `noindex` report you can act on. Ships
with an offline demo — no key, no database. Brand-matched static site generator.

### [`AIStocks`](https://github.com/MichaelPGifford/AIStocks) · Python
A full-stack **SEC fundamentals research platform** (FastAPI + Next.js +
Postgres). Point-in-time XBRL pipeline that fetches, parses, and structures raw
10-K/10-Q filings from the SEC EDGAR API, then charts multi-year revenue, gross
margins, and debt-to-equity — with honestly-reported strategy backtests.

### [`nextjs-fastapi-template`](https://github.com/MichaelPGifford/nextjs-fastapi-template) · TypeScript
The full-stack monorepo starter I reach for: Next.js + FastAPI, a typed API
boundary, single-origin dev proxy, layered backend, and CI for both sides.

### [`data-helpers`](https://github.com/MichaelPGifford/data-helpers) · TypeScript
Dependency-free TypeScript helpers for cleaning messy data feeds — date
normalization, null/empty pruning, structured logging, resilient async retries.
Genericized from real ingestion work. Fully tested (`vitest`), typed, tree-shakeable.

### [`wywaste`](https://github.com/MichaelPGifford/wywaste) · 🥇 1st-place hackathon
Smart-city project for the City of Knoxville (team of three). A sensor-equipped
truck (Raspberry Pi + Arduino) reports GPS and logs missed pickups; residents see
why collection was skipped on a live map. I built the **Node/Express + MongoDB
backend and the device-to-cloud pipeline**, plus the map frontend.

### [`Smartslides`](https://github.com/MichaelPGifford/Smartslides) · CSS/JS
A presentation tool whose slides **follow your voice** — browser mic audio streams
over Socket.io into Google Cloud Speech-to-Text, and the transcript auto-advances
your notecards in real time.

<sub>More on my profile: <a href="https://github.com/MichaelPGifford/RealEstateToken"><code>RealEstateToken</code></a> and <a href="https://github.com/MichaelPGifford/simple-blockchain"><code>simple-blockchain</code></a> (Go/Ethereum experiments), <a href="https://github.com/MichaelPGifford?tab=repositories">and more →</a></sub>

## Experience

- **guidedhunts.io** — Founder &amp; Lead Engineer *(2026–present)* — architected and
  deployed a programmatic aggregator; built extraction pipelines across 9,200+ sites.
- **USCC, LLC** — Founder &amp; Lead Developer *(2020–present)* — production full-stack
  e-commerce (Node.js/JS/SQL) driving **$100k+ annual revenue**; third-party API and
  payment-gateway integrations with 99.9% uptime.
- **Takl** — Technical Support Intern — end-to-end ticket lifecycle in Zendesk;
  replicated database/integration bugs in staging for DevOps hotfixes.
- **Transformation Media** — Web Dev Intern — interactive JS layout tool; production
  Stripe / Square / PayPal payment integrations.

## Tech stack

**Languages** JavaScript · TypeScript · Python · PHP · C++ · SQL
**Frontend** Next.js · React · Tailwind CSS · HTML5 · CSS3
**Backend** Node.js · FastAPI · REST · Webhooks · PostgreSQL · MySQL
**Data &amp; APIs** Firecrawl · DataForSEO · SerpApi · SEC EDGAR · Google APIs · Stripe · Square
**AI-assisted** Cursor · Claude · OpenAI API · prompt engineering
**Infra &amp; tooling** Git · GitHub · Google Cloud Platform · Postman · automated cron jobs

## How I build

- Strict TypeScript and typed Python (`mypy`), linted (`eslint` / `ruff`) and
  tested in CI before anything merges.
- Defensive at the boundaries: coerce and validate untrusted input, never let a
  single bad record take down a batch, fail fast on real bugs.
- Designed for scale from day one, not retrofitted onto sparse data.

## 📈 Recent activity

<!--START_SECTION:activity-->
- `2026-07-05` 📦 Pushed 1 commit to [`MichaelPGifford/MichaelPGifford`](https://github.com/MichaelPGifford/MichaelPGifford)
- `2026-07-05` 📦 Pushed 1 commit to [`MichaelPGifford/MichaelPGifford`](https://github.com/MichaelPGifford/MichaelPGifford)
- `2026-07-05` 📦 Pushed 1 commit to [`MichaelPGifford/MichaelPGifford`](https://github.com/MichaelPGifford/MichaelPGifford)
- `2026-07-05` 📦 Pushed 1 commit to [`MichaelPGifford/serp-gap-analyzer`](https://github.com/MichaelPGifford/serp-gap-analyzer)
- `2026-07-05` 📦 Pushed 1 commit to [`MichaelPGifford/serp-gap-analyzer`](https://github.com/MichaelPGifford/serp-gap-analyzer)
- `2026-07-05` 📦 Pushed 1 commit to [`MichaelPGifford/serp-gap-analyzer`](https://github.com/MichaelPGifford/serp-gap-analyzer)
- `2026-07-05` 📦 Pushed 1 commit to [`MichaelPGifford/serp-gap-analyzer`](https://github.com/MichaelPGifford/serp-gap-analyzer)
- `2026-07-05` 🌱 Created branch in [`MichaelPGifford/serp-gap-analyzer`](https://github.com/MichaelPGifford/serp-gap-analyzer)
- `2026-07-03` 🌱 Created branch in [`MichaelPGifford/AIStocks`](https://github.com/MichaelPGifford/AIStocks)
- `2026-07-03` 🌱 Created branch in [`MichaelPGifford/livrey`](https://github.com/MichaelPGifford/livrey)
- `2026-07-03` 📦 Pushed 1 commit to [`MichaelPGifford/capitalcitycomputer`](https://github.com/MichaelPGifford/capitalcitycomputer)
- `2026-07-03` 🌱 Created branch in [`MichaelPGifford/capitalcitycomputer`](https://github.com/MichaelPGifford/capitalcitycomputer)
<!--END_SECTION:activity-->

## 📊 GitHub at a glance

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=MichaelPGifford&show_icons=true&hide_border=true&count_private=true&include_all_commits=true&theme=vue" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MichaelPGifford&layout=compact&hide_border=true&langs_count=8&theme=vue" alt="Top languages">
</p>

## Education

**B.S. in Computer Science** — University of Tennessee, Knoxville

## Contact

- Email: [mikeygifford@gmail.com](mailto:mikeygifford@gmail.com)
- LinkedIn: [linkedin.com/in/michgif](https://linkedin.com/in/michgif)
- GitHub: [@MichaelPGifford](https://github.com/MichaelPGifford)
