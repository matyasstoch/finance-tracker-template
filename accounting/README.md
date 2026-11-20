# Accounting and Receipts

Monthly expense tracking, matched invoice PDFs, and open missing receipts.

No secrets, card PANs, or banking tokens belong here. Prefer official invoice PDFs over plain email receipts.

| Path | What |
| --- | --- |
| `expenses/` | Monthly bank or card expense snapshots and match summaries |
| `receipts/` | Found invoice PDFs named `YYYY-MM-DD-vendor-amount-CCY.pdf` |
| `missing/open.md` | Charges still missing an invoice or receipt |

## Monthly receipt hunt workflow

1. Export the month's business card expenses that are missing receipts into `expenses/YYYY-MM-ledger.csv`.
2. Ask your coding agent to search your billing inbox (Gmail or IMAP) for each vendor + amount + date window (+/- 3 days).
3. Prefer `Invoice-*.pdf` over `Receipt-*.pdf` (for example on Stripe billing emails).
4. Save matched files into `receipts/YYYY-MM-DD-vendor-amount-CCY.pdf`.
5. Write a short summary in `expenses/YYYY-MM-summary.md` and list only the still-unmatched rows in `missing/open.md`.
