# Contributing to the bank

Entries are added by hand, one at a time, against a fetched source. Quality of attribution beats quantity of entries.

## Entry format

Each entry in `BANK.md` uses exactly these fields:

```markdown
### YYYY-MM-DD — Short descriptive title
Source: https://x.com/karpathy/status/<id>
Summary: Two to four lines, in our words. What he said and why it matters.
Key line: "A brief verified quote, at most ~25 words."   <!-- omit if wording is unverified -->
Tags: theme tags, product tags (e.g. agents, verification, mymilo, codetopo, general)
Product lens: One or two lines, our words — what this datapoint suggests a builder of AI products should consider or do differently.
```

## Verification standard

1. **Canonical URL + date come from a fetched source only** — the post itself, a thread-reader mirror, an aggregator, a web archive, or an article that cites the post. Never from memory.
2. **Key lines** are included only when the exact wording appears in a fetched source. Keep them ≤ ~25 words.
3. **Marks:**
   - Single aggregator / secondary source → append `(via aggregator — secondary source)` to the Summary.
   - Wording not verifiable → no Key line; append `(wording unverified — summary from secondary sources)` to the Summary.
4. **Summaries are always our own words.** Long-form posts (X articles, essays) are summarized, never reproduced.
5. If a candidate post cannot be sourced at all, it is dropped — note it in the PR/commit message so the gap is on record.

## Process

- Add entries under the right theme in `BANK.md` (LLM capability & agents · Software & AI industry · Learning & craft).
- One commit per workstream (scaffold separate from bank entries).
- Update `CHANGELOG.md` when a batch of entries lands.
