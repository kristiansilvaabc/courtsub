# CourtSub 📰

A fact-checking tool for court reporters working across Melbourne's Magistrates Court, County Court, Supreme Court, and Federal Court.

Paste your draft article, source documents, and shorthand notes — CourtSub checks every factual claim paragraph by paragraph and flags anything that needs attention before you file.

---

## Features

- **Paragraph-by-paragraph fact-checking** — works through your draft in order, top to bottom
- **Shorthand decoder** — understands common court reporting abbreviations (Pros, Def, NPP, PSD, MMC, COA, LSC and more)
- **Quote verification** — compares direct quotes against your notes word-for-word, ignoring capitalisation and punctuation differences
- **Name consistency checker** — flags any name spelled differently across your draft
- **Flag for follow-up** — mark individual findings to come back to, with a sticky footer counter
- **File upload** — accepts .pdf and .docx source documents and notes
- **URL fetching** — pull in content from public URLs as a source
- **Word counter** — live word count on your draft
- **Five-category report** — Verified, Check These, Not in Sources, Ambiguous Notes, Check Quotes

---

## Setup

CourtSub uses the [Anthropic API](https://console.anthropic.com). You need an Anthropic account with API access.

1. Open the tool in your browser
2. When prompted, enter your Anthropic API key (starts with `sk-ant-`)
3. Your key is saved in your browser's local storage — it never leaves your device

**Cost:** approximately $0.04 per fact-check run on a typical court story.

---

## Shorthand key

| Abbreviation | Meaning |
|---|---|
| Pros | Prosecution / Prosecutor |
| Def | Defendant / Defence lawyer |
| DOB | Date of birth |
| Chg | Charge / Charged |
| Mag | Magistrate |
| Melb | Melbourne |
| Sent | Sentence / Sentenced |
| NG | Not Guilty |
| Obj | Objection |
| Pol | Police |
| NPP | Non-parole period |
| PSD | Pre-sentence detention |
| w/o | Without |
| maxpen | Maximum penalty |
| Incl | Including / Inclusive / Includes |
| 1.4 but | 1,4-Butanediol |
| dec | Deceased or December (context dependent) |
| u/c | Undercover |
| MMC | Melbourne Magistrates' Court |
| COA | Court of Appeal |
| Det | Detective (context dependent) |
| LSC | Leading Senior Constable |
| PG | Plead guilty (context dependent) |

---

## How to use

1. Paste source documents (court lists, police statements, press releases) or upload .pdf/.docx files
2. Add public URLs if needed — CourtSub will fetch the content
3. Paste or upload your shorthand notes
4. Paste your draft article
5. Click **Run Fact Check**
6. Review the report paragraph by paragraph alongside your draft
7. Flag anything to come back to using the ⚑ button on each finding
8. Clear all fields between stories

---

## Status categories

| Status | Meaning |
|---|---|
| ✓ Verified | Confirmed by sources or notes |
| ✕ Check These | Contradicts sources — check both versions |
| ? Not in Sources | Not found in any provided source or notes |
| ~ Ambiguous Notes | Unclear note or missing detail |
| ❝ Check Quotes | Quote wording differs from notes — verify before publishing |

---

## Privacy

- Your API key is stored in browser local storage only and is never sent to or stored by this repository
- Content you paste is sent to the Anthropic API for processing — subject to [Anthropic's privacy policy](https://www.anthropic.com/legal/privacy)
- No data is stored by this application itself

---

## Built with

- [Anthropic Claude API](https://www.anthropic.com)
- [PDF.js](https://mozilla.github.io/pdf.js/)
- [Mammoth.js](https://github.com/mwilliamson/mammoth.js)
