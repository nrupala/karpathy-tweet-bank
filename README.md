# karpathy-tweet-bank

A wisdom bank of Andrej Karpathy's tweets — links, dates, summaries and key lines, banked for reference.

This is **not an archive**. It is a curated set of data points: short public posts by one of the clearest thinkers in AI, kept because they keep proving useful when building software in the LLM era.

## What this is

- An **attribution-first reference bank** of Andrej Karpathy's public posts on X.
- Every entry links the **canonical post**, gives its **date**, a **summary in our own words**, and — where the wording is verified — a **brief key line**.
- The tweets themselves are © Andrej Karpathy. Nothing here replaces the originals; follow the link and read the source.

## Banking policy

1. **Link, don't copy.** Entries carry the canonical `x.com` URL and date. Long posts are summarized, never reproduced wholesale.
2. **Brief quotes only.** A *Key line* is at most ~25 words, quoted only when the wording was verified against a fetched source.
3. **Verify or mark.** Entries sourced from a single aggregator or secondary source are marked `(via aggregator — secondary source)`. Entries whose wording could not be verified are summary-only — no Key line — and marked `(wording unverified — summary from secondary sources)`.
4. **No fabrication.** No tweet ID, date, or quote is ever entered from memory. If it can't be sourced, it doesn't get banked.

## How this bank is used

The entries are **data points for product work**, consulted during product builds and reviews as advisory input:

- Each entry carries **Tags** (themes + product relevance) so it can be pulled into a build or review by topic.
- Each entry carries a **Product lens** — one or two lines on what the datapoint suggests a builder of AI products should consider or do differently.
- The bank may itself become a product one day: an advisory feed of field-tested judgment for people building with LLMs ("product advice" as a service).

## Layout

- [`BANK.md`](BANK.md) — the bank itself, grouped by theme.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — how entries get added and verified.
- [`CHANGELOG.md`](CHANGELOG.md) — what changed, per release.
- [`NOTICE`](NOTICE) — ownership and third-party attribution.

## License

The bank's own text (summaries, lenses, structure) is licensed under the [Apache License 2.0](LICENSE). Quoted lines remain © Andrej Karpathy and are included briefly for reference and commentary.

---

Owned by Nrupal Akolkar · Built with Muse by Meta
