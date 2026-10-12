# Source documents

Corpus for the Income Tax Assistant. Every document here must be **official**
(`incometaxindia.gov.in` or `incometax.gov.in`) and must describe the **Income-tax Act,
2025 / Income-tax Rules, 2026** for **Tax Year 2026-27 onwards**. Old-law documents are
never mixed in — see [scope.md](scope.md).

All files live in `documents/` and are **not committed** (large third-party PDFs). This
table is the reproducible record: anyone can rebuild the corpus from it.

Captured: 12 Oct 2026.

## Corpus

| # | File | Title | Source URL | Act | Tax year | Pages | Capture | Verified |
|---|---|---|---|---|---|---|---|---|
| 1 | `2026-27_transition-faqs-1961-to-2025_cbdt.pdf` | FAQs on Interplay and Transition from the Income-tax Act, 1961 to the Income-tax Act, 2025 (Directorate of Income Tax, CBDT) | ⚠️ TO FILL | 2025 (incl. 1961 interplay) | 2026-27 onwards + transition | 99 | pdf-download | ✅ text layer is OCR (Acrobat Paper Capture); sampled p.12, clean |
| 2 | `2026-27_form-168-ais_cbdt.pdf` | Form 168 — Annual Information Statement (AIS), notified under Rule 245 of the Income-tax Rules, 2026 | ⚠️ TO FILL | 2025 | 2026-27 | 4 | pdf-download | ✅ |
| 3 | `2026-27_tds-certificates-form-130-133_cbdt.pdf` | Comprehensive Note on TDS Certificates — Form No. 130/131/132/133 (earlier Form 16/16A/16B/16C/16D/16E/27D), s.395(4) of the Income-tax Act, 2025 | ⚠️ TO FILL | 2025 | 2026-27 | 4 | pdf-download | ✅ |
| 4 | `2026-27_budget-2026-faqs-updated_cbdt.pdf` | FAQs on Budget 2026-27 (updated 23 Feb 2026) | ⚠️ TO FILL | 2025 (as amended by Finance Act, 2026) | 2026-27 | 67 | pdf-download | ✅ updated version — the 1 Feb original has a different rate, see `_rejected/` |
| 5 | `2026-27_income-tax-act-2025_cbdt.pdf` | Income-tax Act, 2025 [30 of 2025], as amended by Finance Act, 2026 | ⚠️ TO FILL | 2025 | 2026-27 | 674 | pdf-download | ✅ reference only — do not index whole, see note below |
| 6 | `2026-27_income-tax-rules-2026_cbdt.pdf` | Income-tax Rules, 2026 [G.S.R. 198(E), dated 20-3-2026] | ⚠️ TO FILL | 2025 (Rules 2026) | 2026-27 | 423 | pdf-download | ✅ reference only — do not index whole, see note below |

**⚠️ Source URLs still to fill in.** Provenance is half the value of a citation — an
answer that says "per the transition FAQs" with no link can't be checked by the user.
Paste each from browser history.

### Note on documents 5 and 6

The Act (674 pages) and Rules (423 pages) are authoritative but should **not** be chunked
into the v1 index wholesale. Together they are ~2.9 million characters — thousands of
chunks, of which maybe twenty answer the 15 user questions. Statutory language is dense
and repetitive, so the rest would match every query weakly and drag precision down.

Keep them as reference. If the coverage check leaves a gap, extract the **specific
chapter** that closes it.

## Rejected

Moved to `documents/_rejected/` rather than deleted, so the decisions stay auditable.

| File | Why rejected |
|---|---|
| `FAQs on New Tax vs Old Tax Regime*.html` | **Old law.** Says "Finance Act 2023 … Section 115BAC w.e.f AY 2024-25", Form 10-IEA, s.139(1). Live page on the official portal, but 1961-Act content |
| `Employees - Benefits allowable*.html` | **Old law.** 115BAC, "previous year"; zero occurrences of "tax year" |
| `Treatment of income from different sources*.html` | **Old law.** "previous year" × 50, 115BAC; zero "tax year" |
| `File ITR-1 (Sahaj) Online - FAQs*.html` | **Old law.** Assessment-year framing, zero "tax year" |
| `View Tax Credit Mismatch User Manual*.html` | Borderline — portal procedure, law-neutral, but assessment-year vocabulary. Rejected for consistency; re-capture if Q4 proves uncovered |
| `FAQs-Budget-2026.pdf` | **Superseded.** The 1 Feb 2026 original; the 23 Feb "Updated" version corrects a rate from 2% to 1%. Two conflicting rates in one corpus is worse than one document |
| `FN-137.pdf` | Form 137 (earlier 24G) — TDS/TCS Book Adjustment Statement for **government deductors**. Correct law, serves none of the 15 questions |
| `Tax-Tutorials-as-per-Income-tax-Act-2025*.pdf` | **No content** — a single page of links to 44 tutorials. Useless to ingest, valuable as a download list (below) |

**Format note:** the HTML pages were saved as "complete web page", which produces 3-17%
text to 83-97% navigation, scripts and an asset folder of up to 203 files. Even with the
right law, that needs a boilerplate stripper before chunking. Capture pages as
**print-to-PDF with headers/footers on** instead — the URL and date get stamped into the
file itself.

## Coverage against the 15 user questions

| Q | Topic | Status | Covered by |
|---|---|---|---|
| 1 | why was ₹8,000 TDS deducted | 🟡 partial | #2 (where to check), but not *why* — needs salary-TDS guidance |
| 2 | Form 16 vs bank salary | 🟡 partial | #3 (the form), not gross-vs-net salary computation |
| 3 | changed jobs, report both salaries | 🔴 gap | — |
| 4 | TDS not showing in Form 26AS | 🟢 covered | #2 |
| 5 | HRA exemption rules | 🔴 gap | — (statute only) |
| 6 | standard deduction in the new regime | 🟡 partial | #4 |
| 7 | what changed between the regimes | 🟢 covered | #1, #4 |
| 8 | income earned before April 2026 | 🟢 **strong** | #1 — the refusal-with-citation case |
| 9 | Upwork income: salary or professional | 🔴 gap | — (statute only) |
| 10 | Form 16A vs Form 16 | 🟢 **strong** | #3 |
| 11 | TDS credit from three clients | 🟡 partial | #2 |
| 12 | presumptive taxation | 🔴 gap | — |
| 13 | records for freelance income | 🔴 gap | — |
| 14 | advance tax, when to pay | 🔴 gap | — |
| 15 | freelance plus a full-time job | 🔴 gap | — |

**3 strong · 4 partial · 8 gaps.** Salaried questions are reasonably served; the
freelancer half is almost entirely uncovered.

## Still to download

The rejected `Tax-Tutorials` index listed 44 per-topic tutorials written under the
Income-tax Act, 2025 — the right law in the right register. These close most gaps:

| Tutorial / document | Closes |
|---|---|
| Deductions/Allowances allowed to a salaried employee | Q5, Q6 |
| Tax on Presumptive Basis in case of Certain Eligible Businesses or Professions | Q12 |
| Maintenance of Books of Accounts | Q13 |
| Tax Rates | Q6, Q7 |
| Refund of excess tax paid by the taxpayer | Q11 |
| E-Payment of Direct Taxes | Q14 (partial) |
| CBDT circular on TDS from salaries, Tax Year 2026-27 | Q1, Q2 |
| Advance tax — instalments, due dates, interest | Q14 |
| Which ITR form applies + filing instructions (new law) | Q3, Q15 |
| Business and professional income guidance (new law) | Q9, Q15 |
