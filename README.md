# Groww Mutual Fund FAQs — Facts-Only RAG Prototype

## Scope
- Product: Groww
- AMC corpus: Groww Mutual Fund / Groww Asset Management Limited
- Schemes: Groww Large Cap Fund Direct Growth; Groww Value Fund Direct Growth; Groww ELSS Tax Saver Fund Direct Growth
- Sources: 19 public URLs from Groww/Groww Mutual Fund, AMFI and SEBI. No third-party blogs are used.

## What it answers
Expense ratio, exit load, minimum SIP/lump sum, ELSS lock-in, riskometer, benchmark, and how to download a Groww capital-gains statement.

## What it refuses
Buy/sell decisions, portfolio recommendations, return predictions/comparisons, and other opinionated questions. It redirects to an official educational or scheme document.

## Privacy
The prototype does not request or store PAN, Aadhaar, account numbers, OTPs, email addresses, phone numbers, or other PII.

## Retrieval approach
This prototype uses a small embedded corpus of verified scheme facts and official source metadata. A lightweight keyword/entity matcher retrieves the most relevant fact record and returns its source URL. It deliberately does not calculate returns or synthesize investment advice.

## Run locally
Open `app.html` in a modern browser. No server, API key, database, or external runtime dependency is required.

## Files
- `app.html` — working prototype
- `source_list.csv` — 19 official source URLs
- `sample_qa.md` — sample queries and answers
- `README.md` — setup, scope and limits

## Known limits
- The corpus is intentionally small and limited to three schemes.
- Facts can change; users should open the linked official source for the latest document.
- The assistant is not a financial adviser and does not make recommendations.
- Historical performance/returns are excluded from answer generation.

## UI disclaimer
**Facts-only. No investment advice.**
