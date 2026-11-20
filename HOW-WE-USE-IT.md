# How We Use Finance Tracker

Software subscriptions and AI API bills creep up quietly. And every month, accountants chase missing PDF receipts for card charges. This repo fixes both with plain Markdown files and a coding agent.

## Our day-to-day workflow

### 1. Run a 15-minute subscription audit from a bank CSV
Export 3 to 6 months of transactions from your bank or business card as CSV and drop it into `bank-statements/` (already in `.gitignore`, so raw statements stay on your machine).

Ask your coding agent to parse the CSV and generate `subscriptions-analysis.md`: a month-by-month spend table grouped by category (AI tools, hosting/dev infra, marketing, productivity). Seeing 6 months side by side makes forgotten subscriptions and usage-based creep obvious in 10 seconds.

### 2. Rank subscriptions by blast radius, not alphabetically
In `subscriptions.md`, list fixed subscriptions in working order: the ones that break your business if a card fails go at the top (domains, email, hosting, database), followed by descending cost. Put the approximate billing day next to each item so you never get surprised when switching cards.

Move every tool you want to cut into the "Dropping" section and check them off as you cancel them. In our own audit, this surfaced over $1,000/month in unused subscriptions immediately.

### 3. Let your agent hunt missing receipts once a month
Every month, drop your list of card expenses missing receipts into `accounting/expenses/`. Point your coding agent at your email inbox (using Gmail or IMAP) to search for matching vendor invoices, save them as `accounting/receipts/YYYY-MM-DD-vendor-amount-CCY.pdf`, and write whatever is still unmatched into `accounting/missing/open.md`.

### 4. Write money rules down as short ADRs
Put recurring financial rules (like setting aside 20% of revenue every month for taxes) in `docs/adr/`. One short file per rule so everyone follows the same math.
