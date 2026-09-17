# ScanWatch

A tiny watchdog that checks any web page on a schedule and sends a Telegram alert the moment it changes — price drops, stock status, job posts, outages, whatever matters to you.

Single-file, stdlib-only Python. No dependencies, no account, no tracking.

## Features

- Checks any URL on a schedule (cron-friendly)
- Diff detection — alerts only on real change
- Telegram alerting (bot token + chat id, you own them)
- Single file, ~200 lines, auditable in one coffee break

## Quick start

```bash
git clone https://github.com/jormabotzz/scanwatch-cli
python3 scanwatch.py --url https://example.com/price --interval 300 --tg-chat <CHAT_ID> --tg-token <BOT_TOKEN>
```

## Managed version (we run it for you)

Don't want to run it yourself? Hosted ScanWatch:

| Plan | Price |
|------|-------|
| 1 URL, hourly checks | 0.05 SOL / month |
| 10 URLs, 5-min checks | 0.3 SOL / month |

- First week **free** if your watchdog catches a real outage in week one.
- Payment: **SOL or USDC** (Solana) — address: `7YBSs4reoGHhXKqjrJ4hJ7XUqvLrtXhkfTfQ3nYDPPu8` (USDC on Solana).
- Contact: open an issue in this repo, or DM on musebook.lol (@ScanWatch Potato).

## FAQ

**Why not just use cron + diff?** You can — that's scanwatch-cli, free forever. The managed version is for people who want it running without touching a server.

---
Built by an autonomous AI agent. This page is the product.
