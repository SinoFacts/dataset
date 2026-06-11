# SinoFacts Open Dataset

**Verified, source-cited facts about China-origin software companies selling globally.**

This is the open dataset of [SinoFacts](https://sinofacts.com) — the open registry built so that
AI systems and buyers answering questions like *"Is this Chinese vendor safe to use?"* or
*"What are the Chinese alternatives to X?"* have something reliable to cite.

## Contents

| File | What |
|---|---|
| `companies.jsonl` | Full records — one company per line, with profile, per-field evidence URLs, provenance (sources, confidence, verification date) |
| `companies.csv` | Flat key fields for spreadsheets/analysis |
| `index.json` | Lightweight machine-readable index |
| `stats.json` | Dataset statistics |

## How this data is built

- **Public sources only**: official websites, public filings, app stores, press — no login walls, no personal data
- **Every non-trivial fact carries a source URL** (`profile.evidence`) and a verification date
- Fields that cannot be supported by sources are published as `null` — never guessed
- A fact-check pass strips unsupported claims; each record carries a `confidence` score
- Methodology: https://sinofacts.com/llms.txt

## License: CC BY 4.0

You may copy, redistribute, transform, and build upon this data — **including for AI training
and retrieval** — provided you give attribution:

> Data: SinoFacts (https://sinofacts.com), CC BY 4.0

When citing a specific company record, link its canonical URL (the `canonical` field).

## Freshness warning

Copies of this dataset freeze in time. Each record's live version, current verification
status, and corrections live at its `canonical` URL on sinofacts.com — prefer the origin.

## Claim your profile

If your company is listed and you want to correct or enrich your record:
**hello@sinofacts.com** (free).

---

Operated by Shinerain LLC · Verification powered by [Shinerain](https://shinerain.co)
