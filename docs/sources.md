# Source documents

Corpus for the Income Tax Assistant. Every document must be **official**
(`incometaxindia.gov.in` / `incometax.gov.in`) and must describe the **Income-tax Act,
2025 / Income-tax Rules, 2026** for **Tax Year 2026-27 onwards**. Old-law documents are
never mixed in — see [scope.md](scope.md).

Files live in `documents/` and are **not committed** (large third-party publications).
This table is the reproducible record: the corpus can be rebuilt from it.

**Captured:** 12 Oct 2026. **24 documents.**

## How law era was verified

Every file was checked for vocabulary, not trusted by title. The 2025 Act replaced
"previous year"/"assessment year" with **"tax year"**, and section 115BAC (the old Act's
new-regime provision) no longer exists. So:

- ✅ contains "tax year", no "assessment year", no "115BAC" → new law
- ❌ contains "115BAC" or "previous year", zero "tax year" → old law, reject

Most CBDT tutorials also carry an explicit stamp: *"This document contains the provisions
of the Income-tax Act, 2025, as amended by the Finance Act, 2026."*

## Corpus

### Core — transition, forms, rates

| File | Title | Source | Pages/size | Serves |
|---|---|---|---|---|
| `2026-27_transition-faqs-1961-to-2025_cbdt.pdf` | FAQs on Interplay and Transition from the Income-tax Act, 1961 to the Income-tax Act, 2025 | [link](https://www.incometaxindia.gov.in/documents/20117/43120/Updated-FQAs-on-Interplay%26Transitions.pdf/dda21cfd-28be-d931-ad5c-6459ecbd2ea7?version=2.0) (v2.0) | 99 pp | Q7, Q8 |
| `2026-27_tds-certificates-form-130-133_cbdt.pdf` | Comprehensive Note on TDS Certificates — Form 130/131/132/133 (earlier 16/16A/16B/16C/16D/16E/27D), s.395(4) | forms hub ⚠️ | 4 pp | Q2, Q10 |
| `2026-27_form-168-ais_cbdt.pdf` | Form 168 — Annual Information Statement (AIS), Rule 245 | forms hub ⚠️ | 4 pp | Q1, Q4, Q11 |
| `2026-27_budget-2026-faqs-updated_cbdt.pdf` | FAQs on Budget 2026-27 (updated 23 Feb 2026) | articleKey 15773815 ⚠️ | 67 pp | Q6, Q7 |
| `2026-27_tax-rates_tutorial.html` | Tax Rates (Tax Tutorial) | [articleKey 20753090](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20753090) | 37 k chars | Q6, Q7 |
| `2026-27_tds-rates_reftable.html` | TDS Rates (Tax Reference Table) | [articleKey 20863623](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20863623) | 25 k chars | Q1, Q11 |

### Salaried employees

| File | Title | Source | Size | Serves |
|---|---|---|---|---|
| `2026-27_salary-deductions-allowances_tutorial.html` | Deductions/Allowances allowed to a salaried employee | [articleKey 20296315](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20296315) | 24 k chars | Q5, Q6 |
| `2026-27_employees-benefits-allowable_reftable.html` | Employees — Benefits allowable | [articleKey 19644329](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/19644329) | 39 k chars | Q1, Q2, Q3, Q5 |
| `2026-27_allowances-allowable_reftable.html` | Allowances allowable to tax payer | [articleKey 20828899](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20828899) | 18 k chars | Q5 |
| `2026-27_deductions-allowable_reftable.html` | Deductions allowable to tax payer | [articleKey 20863470](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20863470) | 55 k chars | Q5, Q6 |

### Freelancers and professionals

| File | Title | Source | Size | Serves |
|---|---|---|---|---|
| `2026-27_presumptive-taxation_tutorial.html` | Tax on Presumptive Basis in case of Certain Eligible Businesses or Professions | [articleKey 20292967](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20292967) | 36 k chars | Q12 |
| `2026-27_faqs-presumptive-taxation_cbdt.pdf` | FAQs on Tax on Presumptive Taxation Scheme | [link](https://www.incometaxindia.gov.in/documents/d/guest/faqs-on-tax-on-presumptive-taxation-scheme) | 14 pp | Q12 |
| `2026-27_books-of-accounts_tutorial.html` | Maintenance of Books of Accounts | [articleKey 20296243](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20296243) | 13 k chars | Q13 |
| `2026-27_small-businessmen-benefits_reftable.html` | Small Businessmen — Benefits allowable | [articleKey 19644264](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/19644264) | 27 k chars | Q9, Q12, Q13 |
| `2026-27_faqs-tax-audit_cbdt.pdf` | FAQs on Tax audit | [link](https://www.incometaxindia.gov.in/documents/d/guest/faqs-on-tax-audit-1) | 5 pp | Q13 |

### TDS, advance tax, payments and refunds

| File | Title | Source | Size | Serves |
|---|---|---|---|---|
| `2026-27_faqs-tds_cbdt.pdf` | FAQs on Tax Deducted at Source (TDS) | [link](https://www.incometaxindia.gov.in/documents/d/guest/faqs-on-tax-deducted-source) | 30 pp | Q1, Q2, Q11 |
| `2026-27_faqs-advance-tax_cbdt.pdf` | FAQs on Advance Tax (ss. 404-409) | [link](https://www.incometaxindia.gov.in/documents/d/guest/faq-on-advance-tax) | 12 pp | Q14 |
| `2026-27_e-payment-direct-taxes_tutorial.html` | E-Payment of Direct Taxes | [articleKey 20332769](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20332769) | 11 k chars | Q14 |
| `2026-27_faqs-ais-tis_cbdt.pdf` | FAQs on AIS and TIS | [link](https://www.incometaxindia.gov.in/documents/d/guest/faqs-on-annual-information-system) | 2 pp ⚠️ thin | Q4, Q11 |
| `2026-27_refund-of-excess-tax_tutorial.html` | Refund of excess tax paid by the taxpayer | [articleKey 20833431](https://www.incometaxindia.gov.in/o/headless-delivery/v1.0/sites/20117/structured-contents/by-key/20833431) | 20 k chars | Q11 |

### General and statutory reference

| File | Title | Source | Size | Note |
|---|---|---|---|---|
| `2026-27_faqs-general_cbdt.pdf` | General FAQs as per Income-tax Act, 2025 | [link](https://www.incometaxindia.gov.in/documents/d/guest/general-faqs) | 9 pp | fallback |
| `2026-27_faqs-computation-of-tax_cbdt.pdf` | FAQs on Computation of Tax | [link](https://www.incometaxindia.gov.in/documents/d/guest/faqs-on-computation-of-tax) | 12 pp | Q6, Q7, Q15 |
| `2026-27_income-tax-act-2025_cbdt.pdf` | Income-tax Act, 2025 [30 of 2025], as amended by Finance Act, 2026 | act/rules page ⚠️ | 674 pp | **do not index whole** |
| `2026-27_income-tax-rules-2026_cbdt.pdf` | Income-tax Rules, 2026 [G.S.R. 198(E), 20-3-2026] | act/rules page ⚠️ | 423 pp | **do not index whole** |

⚠️ **Five direct URLs still to fill** (the files downloaded by hand before the catalogue
existed). Their hub pages:
`/faqs-and-guidance-notes-on-forms-as-per-income-tax-rules-2026` (the two form notes) and
`/income-tax-act-202511` (Budget FAQs, Act, Rules).

### Note on the Act and Rules

Authoritative, but **do not chunk them into the v1 index**. Together ~2.9 M characters →
thousands of chunks, of which maybe twenty answer the 15 questions. Statutory language is
dense and repetitive, so the rest matches every query weakly and drags precision down.
Keep as reference; if a gap appears, extract the specific chapter.

## Capture method

| Format | Count | How |
|---|---|---|
| PDF | 10 | downloaded from `/documents/d/guest/<slug>` |
| HTML (content-only) | 12 | Liferay headless-delivery API, `documentContent` field |
| PDF (manual) | 2 | Act and Rules, downloaded by hand |

`incometaxindia.gov.in` sits behind a WAF that fingerprints the TLS handshake — `curl`
gets 403 with any user-agent or cookie, and headless browsers are detected too. These
were captured by driving a real windowed browser and fetching from the page context.

**The HTML files are content-only** — a single `documentContent` field, 65-70% text, no
navigation, scripts or asset folders. Each carries a comment header with its source URL,
article key, site `dateModified` and capture date. That is a far better ingestion input
than "save page as HTML", which yielded 3-17% text (see rejected).

## Rejected

In `documents/_rejected/`, not deleted, so the decisions stay auditable.

| File | Why |
|---|---|
| `FAQs on New Tax vs Old Tax Regime*.html` | **Old law** — "Finance Act 2023 … s.115BAC w.e.f AY 2024-25", Form 10-IEA. Live on the official portal, three years stale |
| `Employees - Benefits allowable*.html` | **Old law** — 115BAC, "previous year", zero "tax year". Replaced by the new-law reference table above |
| `Treatment of income from different sources*.html` | **Old law** — "previous year" ×50 |
| `File ITR-1 (Sahaj) Online - FAQs*.html` | **Old law** — assessment-year framing |
| `View Tax Credit Mismatch User Manual*.html` | Borderline: portal procedure, assessment-year vocabulary. Superseded by the AIS and TDS FAQs |
| `FAQs-Budget-2026.pdf` | **Superseded** — the 1 Feb original; the 23 Feb update corrects a rate from 2% to 1% |
| `FN-137.pdf` | Form 137 (ex-24G), TDS/TCS Book Adjustment for **government deductors**. Right law, irrelevant to the users |
| `Tax-Tutorials-*.pdf` | Link index, no content — but it named the 42 tutorials, 6 of which are now in the corpus |
| `index-only--faqs-act-2025-hub.html` | Link index — named the 30 FAQ documents, 7 now in the corpus |
| `index-only--tax-reference-tables-hub.html` | Link index — named 25 reference tables, 4 now in the corpus |
| `duplicate--Updated-FQAs-*.pdf` | Byte-identical duplicate of the renamed transition FAQ |

## Coverage against the 15 user questions

Scanned by keyword across the whole corpus (statutes excluded).

| Q | Topic | Status |
|---|---|---|
| 1 | why ₹8,000 TDS deducted | 🟢 TDS FAQs, TDS rates, employees-benefits |
| 2 | Form 16 vs bank salary | 🟢 form-130-133 note, salary deductions |
| 3 | changed jobs, two employers | 🟡 **weak** — one mention only |
| 4 | TDS not in Form 26AS | 🟢 Form 168 AIS |
| 5 | HRA exemption | 🟢 allowances, salary deductions |
| 6 | standard deduction, new regime | 🟢 salary deductions, budget FAQs |
| 7 | what changed between regimes | 🟢 budget FAQs, tax rates, transition |
| 8 | income before April 2026 | 🟢 **strong** — transition FAQs, 183 hits |
| 9 | Upwork: salary or professional | 🟢 small-businessmen, presumptive |
| 10 | Form 16A vs Form 16 | 🟢 form-130-133 note |
| 11 | TDS credit, three clients | 🟢 TDS FAQs, AIS, refunds |
| 12 | presumptive taxation | 🟢 **strong** — tutorial + FAQ, 200 hits |
| 13 | records for freelance income | 🟢 books of accounts, tax audit |
| 14 | advance tax | 🟢 **strong** — advance tax FAQs, 81 hits |
| 15 | freelance plus a full-time job | 🟡 **weak** — two mentions |

**13 covered, 2 weak, 0 uncovered** (was 3 / 4 / 8).

Keyword presence is not proof a question is answerable — it only proves the topic is in
the corpus. Real verification happens in Stage 4-5, when retrieval returns actual
passages. Q3 and Q15 are the two to watch.

## Still worth adding

| Need | Closes |
|---|---|
| Salary from two employers / mid-year job change (CBDT salary-TDS circular for TY 2026-27) | Q3 |
| Combining salary with professional income; which ITR form applies | Q15 |
