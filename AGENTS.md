# Finance Tracker Agent Rules

Working repo for recurring subscriptions, spend analysis, receipt matching, and financial decisions.

## Security and privacy

- Keep this repository **private**.
- Never commit full card numbers, CVVs, bank passwords, API keys, or session tokens.
- Keep raw bank statement CSVs in `bank-statements/` (gitignored). Commit only clean Markdown summaries and approved receipts/ledgers.

## Subscriptions (`subscriptions.md`)

- Separate fixed monthly/annual subscriptions from usage-based APIs.
- Order active subscriptions by impact if payment fails first (domains, email, hosting), then by descending monthly cost.
- Record the approximate billing day of the month and the source statement date.

## Receipts and accounting (`accounting/`)

- Prefer official invoice PDFs over email receipts when both exist.
- Name every saved receipt consistently: `YYYY-MM-DD-vendor-amount-CCY.pdf` (example: `2026-01-15-vercel-20.00-USD.pdf`).
- Never mark a charge as matched unless both the vendor and amount match (or the exact FX conversion is noted).
- Keep `accounting/missing/open.md` up to date so only truly unmatched charges remain open.

## Finance decisions (`docs/adr/`)

- Use numbered files: `0001-short-slug.md`.
- Never rewrite old decisions. Supersede with a new file if a rule changes.
