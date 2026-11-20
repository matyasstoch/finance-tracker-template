# Subscriptions

Currency: USD. Source: `bank-statements/example-statement.csv` (replace with your real export).

| Category | $/month |
| --- | ---: |
| All fixed subscriptions | ~240 + domains (annual) |
| Keeping (4) | ~185 + domains |
| Dropping (2) | ~55 (~$660/yr saved) |
| Usage-based AI APIs (billed separately) | ~100-300 |

Last reviewed: 2026-01-15.

---

## Keeping (ordered by what breaks if payment fails, then by cost)

| # | Status | Service | $/mo | Bills ~day | Notes |
| ---: | :---: | --- | ---: | --- | --- |
| 1 | Active | Domain registrar (Namecheap/Cloudflare) | annual | renewal date | Critical. A failed card takes sites and email offline. |
| 2 | Active | Google Workspace | 15 | 2nd | Core email and Drive. |
| 3 | Active | AI coding plan (Claude/Codex) | 100 | 10th | Daily driver for building. |
| 4 | Active | Supabase | 25 | 24th | Production database (+ usage). |
| 5 | Active | Vercel | 20 | 25th | App hosting. |
| 6 | Active | GitHub | 25 | 12th | Code and private repos. |

---

## Usage-based APIs (check monthly for spend creep)

| Service | Typical $/mo | Billing trigger | Notes |
| --- | ---: | --- | --- |
| OpenRouter / Anthropic / OpenAI API | 100-300 | Auto top-up | Set a hard monthly cap in the provider dashboard. |

---

## Dropping (cancel before next billing day)

| # | Cancelled? | Service | $/mo | Next bill | Why dropping |
| ---: | :---: | --- | ---: | --- | --- |
| 1 | [ ] | Old analytics tool | 35 | 18th | Unused for 3 months. |
| 2 | [ ] | Duplicate note app | 20 | 22nd | Replaced by Git repos. |
