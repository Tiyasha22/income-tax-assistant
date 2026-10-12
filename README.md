# Income Tax Assistant (India)

A question-answering assistant that explains **Indian income-tax rules** to salaried
people and freelancers in plain language. It answers only from official government
documents, cites the source for every answer, and refuses to answer when no reliable
source matches.

> **This explains the rules. It is not tax advice.**

## Why

Most people don't know the basics of their own income tax, and the law just changed:
the **Income-tax Act, 2025** came into force on **1 April 2026**, replacing the 1961 Act.
Most content online still describes the old law.

## Scope

| | |
|---|---|
| **For** | Salaried individuals; freelancers and independent professionals in India |
| **Law covered** | Income-tax Act, 2025 and Income-tax Rules, 2026 — **Tax Year 2026-27 onwards** |
| **Sources** | `incometaxindia.gov.in` and `incometax.gov.in` only |
| **Out of scope** | Company tax, capital gains, international tax, personal calculations, personal advice |

Income earned before 1 April 2026 falls under the 1961 Act and is **out of scope** — the
assistant explains that boundary rather than guessing. Old-law and new-law documents are
never mixed in the same index.

See [docs/scope.md](docs/scope.md) and [docs/future-scope.md](docs/future-scope.md).

## Status

**Stage 1 of 10 — scope and documents.** No application code yet.

- [x] Scope, users and refusal behaviour defined
- [x] 15 real user questions + 6 must-refuse test cases ([docs/questions.md](docs/questions.md))
- [ ] 10-15 official documents collected and catalogued in `docs/sources.md`
- [ ] Chunking → embeddings → retrieval → answering → API → frontend → evaluation → deploy

## Planned stack

Python (plain scripts) · PostgreSQL + pgvector in Docker · Gemini API for embeddings and
answers · FastAPI · Next.js + TypeScript

## Repository layout

```
docs/          scope, user questions, source document catalogue
documents/     official source PDFs (not committed - see docs/sources.md)
```

The source documents are third-party government publications and are not committed.
`docs/sources.md` records the file name, title, source URL, capture date, which Act and
which tax year for each one, so the corpus can be rebuilt from scratch.
