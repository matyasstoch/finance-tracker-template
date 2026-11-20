# Finance Tracker

Working repo for your personal or company finances: recurring subscriptions, monthly spend analysis, receipt matching, and simple finance rules.

Keep this repository **private**. Never commit card numbers, bank logins, or API keys.

## Quick setup prompt

Paste this into your coding agent inside this folder:

```text
Read README.md, HOW-WE-USE-IT.md, and AGENTS.md. I am going to drop a CSV export of my last 3 to 6 months of bank or card statements into bank-statements/ (which is gitignored). Ask me my main currency and whether this is for personal or business finances. Then parse the CSV, fill out subscriptions-analysis.md with a clean month-by-month spend table grouped by category, populate subscriptions.md ranked by what hurts most if a card fails, and list every recurring charge I might want to cancel.
```

## Map

- [subscriptions.md](subscriptions.md) - Every recurring card/subscription, sorted by what breaks if a payment fails, then by cost. Also tracks what you are cancelling.
- [subscriptions-analysis.md](subscriptions-analysis.md) - Month-by-month spend table built from your bank CSV, grouped by category so spend creep jumps out.
- [accounting/](accounting/README.md) - Monthly expense ledgers, receipt PDFs, and the open missing-receipts list.
- [docs/adr/](docs/adr/0001-monthly-tax-reserve.md) - Short numbered finance decisions (such as your monthly tax reserve rule).
- [HOW-WE-USE-IT.md](HOW-WE-USE-IT.md) - How we actually run subscription audits and monthly receipt hunts with coding agents.
