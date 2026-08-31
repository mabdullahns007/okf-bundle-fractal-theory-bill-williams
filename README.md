# Fractal Theory

An [OKF (Open Knowledge Format v0.2)](../CLAUDE.md) knowledge bundle documenting Bill Williams' chaos-theory / fractal approach to trading, built with the [Karpathy LLM Wiki pattern](../karpathy-llm-wiki.md): a structured, interlinked collection of markdown files maintained by an LLM agent rather than re-derived on every query.

**20 pages** across 6 categories, all sourced from a single ingested talk, with citations, cross-links, and per-page `status` (currently all `draft`, pending human review).

## Karpathy LLM Wiki pattern

Three layers:

- **Raw sources** — the original talk transcript/notes. Recorded at [`sources/practical-fractal-video.md`](sources/practical-fractal-video.md), with the raw record at `raw/sources/practical-fractal-bill-williams.md`.
- **The wiki** — the pages under `people/`, `organizations/`, `books/`, `concepts/`, and `case-studies/`. LLM-maintained.
- **The schema** — [`/CLAUDE.md`](../CLAUDE.md), which defines the OKF page format and conventions for this bundle.

Two index files navigate the wiki:

- [`index.md`](index.md) — content-oriented catalog of every page, organized by category.
- [`log.md`](log.md) — chronological event log of ingestion and query activity.

## What's in here

```
sources/           1 file    the ingested talk: "The Practical Fractal: The Holy Grail to Trading"
people/            1 file    Bill Williams
organizations/     1 file    Profitunity Trading Group
books/             1 file    Trading Chaos (stub — not yet ingested as its own source)
concepts/         13 files   fractal, balance line, oscillators, five dimensions, stop rule, psychology, critiques
case-studies/      3 files   yen fractal trade, Janet's Eurodollar spread, San Juan Investments testimonial
entities/          —         reserved, not yet populated
```

### Concepts

- [Market definition (Fred & Barney)](concepts/market-definition.md) — why consensus and overbought/oversold are meaningless by construction
- [Chaos theory — three principles](concepts/chaos-theory-three-principles.md) — least resistance, unseen structure, changeable structure
- [Fractal (market)](concepts/fractal.md) — the five-bar pattern and its breakout entry rule
- [Balance line](concepts/balance-line.md) — 13-bar MA offset 8 bars forward, the "strange attractor"
- [Momentum oscillator (5/34)](concepts/momentum-oscillator.md) — 5-bar minus 34-bar simple MA histogram
- [Accelerator oscillator](concepts/accelerator-oscillator.md) — 5-bar MA of the momentum oscillator
- [Five dimensions of market structure](concepts/five-dimensions-of-market-structure.md) — the full framework
- [Five magic bullets](concepts/five-magic-bullets.md) — all five dimensions reversing at once
- [Bar classification: squats, greens, fades, fakes](concepts/bar-classification-squats-greens-fades-fakes.md) — named but under-defined in this source
- [Stop-placement rule](concepts/stop-placement-rule.md) — two fractals back, opposite direction
- [Trading psychology: "want what the market wants"](concepts/trading-psychology-holy-grail.md) — the talk's psychological core
- [Technical analysis critique](concepts/technical-analysis-critique.md) — why templates of the past fail
- [Win/loss ratio fallacy](concepts/win-loss-ratio-fallacy.md) — why win rate is the wrong metric

### Case studies

- [Japanese yen fractal trade](case-studies/yen-fractal-trade-case-study.md) — a worked multi-month example
- [Janet's Eurodollar spread trade](case-studies/janet-eurodollar-spread-case-study.md) — small-account student anecdote
- [San Juan Investments testimonial](case-studies/san-juan-investments-testimonial.md) — fund-ranking testimonial

## Scope

This is a **definitional library**, not a trading system. It does not contain:

- Trading algorithms, backtests, or live signal generation
- Live market data feeds or broker integrations
- Independently verified performance results (track-record claims are recorded as *claims*, attributed and cited, not validated)
- Personal opinions on what "works"

Live-data queries applied against this framework (e.g. running the fractal/balance-line/oscillator confluence against a real symbol) are logged in [`log.md`](log.md) but are not filed as new wiki pages unless they produce durable, source-backed synthesis.

## File format

Every page carries YAML frontmatter (`type`, `title`, `description`, `tags`, `sources`, `generated: {by, at}`, `status`) followed by prose body sections, inline `[links](path.md)` to related pages, and footnote-style citations back to the source talk. `status: draft` means the page has not yet had human review.

## Naming convention

Files: `kebab-case.md`. One concept, person, or case study per file.

## How to use this

**As a human reader:** start at [`index.md`](index.md) and follow links into whichever concept or case study you need.

**As an LLM agent:** read [`/CLAUDE.md`](../CLAUDE.md) for the schema and conventions, then read [`index.md`](index.md) to route a query to the right page(s). Cite pages by path. When ingesting a new source, follow the pattern already used for `sources/practical-fractal-video.md`: add a source record, then file or update `concepts/`, `people/`, `organizations/`, `books/`, and `case-studies/` pages as needed, and append an entry to `log.md`.

## Status

Early-stage: one source ingested (2026-08-28), all pages in draft. Several concepts (notably bar classification, and the stop-placement rule's edge cases in choppy markets — see the 2026-08-29 log entry) are flagged as under-defined pending a second source.
