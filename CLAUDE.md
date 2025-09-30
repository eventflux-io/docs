# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the documentation repository for **EventFlux**, a pattern-first stream processing engine (CEP) in Rust. The documentation will be hosted at `docs.eventflux.io` via GitHub Pages.

## Repository Structure

The repository follows a standard documentation site structure:
- `docs/` — main content in Markdown/MDX, organized by topic:
  - `getting-started/`
  - `concepts/` (time, windows, watermarking, state)
  - `operators/` (filter, map, join, enrich, aggregate)
  - `patterns/` (CEP sequences, absence, correlation)
  - `connectors/`
  - `deploy/` (Docker, Kubernetes, on-prem)
  - `metrics-and-tuning/`
- `static/` — images, diagrams, and static assets
- `src/` — theme overrides and custom pages
- `versioned_docs/` — versioned documentation (appears after versioning is enabled post-1.0)
- `assets/brand/` — brand materials and messaging reference

## Documentation Standards

### Terminology & Naming
- Always refer to EventFlux as a "pattern-first stream processing engine (CEP) in Rust" on first mention
- Core operator nouns: **filters, joins, enrichment, windows, patterns**
- EventFlux is an **engine**, not a broker or platform
- Refer to `/Users/grainier/Github/docs/assets/brand/BRAND_REFERENCE.md:1` for complete brand guidelines

### Writing Style
- First paragraph should answer: "What is it? Why do I need it?"
- Use concrete terms over vague buzzwords
- Keep examples short and focused on illustrating one concept
- Include one-sentence summaries at the top of new pages
- Use relative links for internal references
- Place assets in `static/` with descriptive alt text

### Avoid
- Platform language (EventFlux is not a broker)
- Generic development practices
- Duplicating content that exists elsewhere

## Publishing

Documentation is deployed via GitHub Actions to GitHub Pages with custom domain `docs.eventflux.io`. DNS is configured with CNAME `docs` → `eventflux-io.github.io`.

## Licensing

- **Documentation content:** CC BY 4.0 (see LICENSE)
- **Code samples/snippets:** MIT (see CODE-LICENSE)

## Versioning Policy

- Pre-1.0: docs track `main` branch
- Post-1.0: versioned docs will be enabled and stable pages backfilled as needed