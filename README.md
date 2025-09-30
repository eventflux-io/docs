# EventFlux Documentation

Documentation for **EventFlux**, a pattern-first stream processing engine (CEP) in Rust.

- **Live URL:** https://docs.eventflux.io
- **Purpose:** Guides, concepts, operators, patterns (CEP), connectors, deploy, metrics/tuning.
- **Hosting:** GitHub Pages (via GitHub Actions) with custom domain `docs.eventflux.io`.

---

## Structure

- `docs/` — main content in Markdown/MDX
  - `getting-started/`
  - `concepts/` (time, windows, watermarking, state)
  - `operators/` (filter, map, join, enrich, aggregate)
  - `patterns/` (CEP sequences, absence, correlation)
  - `connectors/`
  - `deploy/` (Docker, Kubernetes, on-prem)
  - `metrics-and-tuning/`
- `static/` — images and diagrams
- `src/` — theme overrides and custom pages
- `versioned_docs/` — will appear once versioning is enabled

> Keep terminology aligned with the **Brand & Messaging Reference**.

---

## Publishing

Docs are built and deployed by a GitHub Actions workflow to GitHub Pages.  
The repo’s **Settings → Pages** is configured to:
- **Build and deployment:** Source = “GitHub Actions”
- **Custom domain:** `docs.eventflux.io`
- **Enforce HTTPS:** enabled once DNS is active

DNS (at Namecheap):
- CNAME `docs` → `eventflux-io.github.io`

---

## Contribution guidelines

- **Before you write:** check existing pages to avoid duplication.
- **New pages:** include a one-sentence summary at the top; keep titles concise.
- **Links & images:** use relative links; put assets in `static/` with alt text.
- **Examples:** prefer short, focused examples that illustrate one idea.

### Style & framing

- First paragraph of a topic should answer: **What is it? Why do I need it?**
- Use the core nouns consistently: **filters, joins, enrichment, windows, patterns**.
- Avoid platform language; EventFlux is an **engine**, not a broker.

### Versioning (policy)

- Until 1.0, docs track `main`.
- We’ll enable versioned docs post-1.0 and backfill stable pages as needed.

---

## Licensing

This repository uses **dual licensing**:

- **Documentation content:** CC BY 4.0 — see `LICENSE`
- **Code samples and example snippets:** MIT — see `CODE-LICENSE`

When reusing content under CC BY 4.0, attribute “EventFlux” and link back to the source page.

---

## Feedback

- Docs issues and requests: open an Issue with page URL and proposed change.
- General questions: use Discussions
