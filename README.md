# Michael Gifford

Full-stack engineer building production web platforms and data pipelines —
TypeScript/React/Next.js on the front, Python/FastAPI and LLM-backed data
extraction on the back.

> **A note on what's public here.** My current commercial platform and the
> proprietary data pipeline behind it are maintained in **private repositories**
> for commercial-confidentiality and IP reasons. The public repositories below
> are the genuine pieces I can share — earlier projects, a 1st-place hackathon
> build, reusable tooling, and libraries genericized from real production
> patterns. Happy to walk through the private work in depth in an interview.

## What I work on

- **Full-stack product engineering** — Next.js (App Router, RSC, TypeScript)
  frontends backed by FastAPI / async Python services.
- **Data pipelines** — scraping, normalization, and LLM-based structured
  extraction with deterministic, cache-first, retry-resilient designs.
- **SEO-first public sites** — server-rendered, structured-data-rich pages built
  to scale to thousands of crawlable URLs.

## Selected public repositories

### [`wywaste`](https://github.com/MichaelPGifford/wywaste)
**1st-place hackathon project for the City of Knoxville** (team of three). A
sensor-equipped garbage truck (Raspberry Pi + Arduino) reports GPS position and
logs missed pickups with a photo; residents see why their collection was skipped
on a live map. I built the **Node/Express + MongoDB backend and the
device-to-cloud image pipeline**, plus the map frontend. Credits and scope in the
README.

### [`RealEstateToken`](https://github.com/MichaelPGifford/RealEstateToken)
A proof-of-concept for **tokenizing real estate on Ethereum** — each property is
minted as its own ERC-20 token that can be traded. Go backend with `go-ethereum`,
a Solidity token contract, wallet/transfer handling, and a Bing Maps property
browser. (Solo, 2018–19.)

### [`simple-blockchain`](https://github.com/MichaelPGifford/simple-blockchain)
A blockchain built from scratch in Go (SHA-256 hash-linked blocks) — the
deliberate "learn the primitives first" precursor I used to decide *against*
rolling my own chain and *for* building `RealEstateToken` on Ethereum.

### [`data-helpers`](https://github.com/MichaelPGifford/data-helpers)
Dependency-free TypeScript helpers for cleaning messy data feeds — date
normalization, null/empty pruning, structured logging, resilient async retries.
Genericized from real ingestion work. Fully tested (`vitest`), typed, tree-shakeable.

### [`nextjs-fastapi-template`](https://github.com/MichaelPGifford/nextjs-fastapi-template)
The full-stack monorepo starter I reach for: Next.js + FastAPI, typed API
boundary, single-origin dev proxy, layered backend, CI for both sides.

### [`Smartslides`](https://github.com/MichaelPGifford/Smartslides)
A presentation tool whose slides **follow your voice** — browser mic audio is
streamed over Socket.io into Google Cloud Speech-to-Text, and the transcript
auto-advances your notecards in real time. (Solo, 2019.)

## How I build

- Strict TypeScript and typed Python (`mypy`), linted (`eslint` / `ruff`) and
  tested in CI before anything merges.
- Defensive at the boundaries: coerce and validate untrusted input, never let a
  single bad record take down a batch, fail fast on real bugs.
- Designed for scale from day one, not retrofitted onto sparse data.

## Contact

- GitHub: [@MichaelPGifford](https://github.com/MichaelPGifford)
- Email: mikey.gifford@gmail.com
