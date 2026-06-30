# Michael Gifford

Full-stack engineer building production web platforms and data pipelines —
TypeScript/React/Next.js on the front, Python/FastAPI and LLM-backed data
extraction on the back.

> **A note on what's public here.** My commercial platforms and the proprietary
> data pipelines behind them are maintained in **private repositories** for
> commercial-confidentiality and IP reasons. The public repositories below are
> the genuine, sanitized pieces I can share: reusable architecture templates,
> dependency-free utility libraries, and tooling — the same patterns I run in
> production, with the business domain stripped out. Happy to walk through the
> private work in depth in a technical interview.

## What I work on

- **Full-stack product engineering** — Next.js (App Router, RSC, TypeScript)
  frontends backed by FastAPI / async Python services.
- **Data pipelines** — scraping, normalization, and LLM-based structured
  extraction with deterministic, cache-first, retry-resilient designs.
- **SEO-first public sites** — server-rendered, structured-data-rich pages built
  to scale to thousands of crawlable URLs.

## Selected public repositories

### [`nextjs-fastapi-template`](https://github.com/MichaelPGifford/nextjs-fastapi-template)
The full-stack monorepo starter I reach for: Next.js + FastAPI in one repo,
typed API boundary, single-origin dev proxy, layered backend, and CI for both
sides out of the box. A runnable, empty shell of the architecture I ship to
production.

### [`data-helpers`](https://github.com/MichaelPGifford/data-helpers)
Small, dependency-free TypeScript helpers for cleaning messy data feeds — date
normalization, null/empty pruning, structured logging, and resilient async
retries with backoff. Extracted and genericized from real ingestion work. Fully
tested (`vitest`), typed, and tree-shakeable.

## How I build

- Strict TypeScript and typed Python (`mypy`), linted (`eslint` / `ruff`) and
  tested in CI before anything merges.
- Defensive at the boundaries: coerce and validate untrusted input, never let a
  single bad record take down a batch, fail fast on real bugs.
- Designed for scale from day one, not retrofitted onto sparse data.

## Contact

- GitHub: [@MichaelPGifford](https://github.com/MichaelPGifford)
- Email: mikey.gifford@gmail.com
