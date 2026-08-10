# Subscription Manager

Subscription Manager is a local-first Django app for finding, reviewing, and tracking recurring subscriptions. It combines manual subscription entry, transaction evidence, Gmail receipt scanning, review candidates, renewal alerts, spend analytics, account controls, and multi-currency totals.

## Features

- Custom user accounts with email-token verification, username changes, password changes, account export, session controls, and account deletion flows.
- Subscription dashboard with monthly spend, annual run-rate, upcoming renewals, active/inactive counts, category mix, and trend data.
- Manual subscription tracking with user-isolated data.
- Candidate review queue for transaction, inbox, and receipt-parser evidence.
- Gmail OAuth connection, mailbox status, re-sync, revoke, scan preferences, and per-user mailbox isolation.
- Receipt parsing that extracts suggested merchant, amount, cadence, renewal date, and confidence metadata.
- Review filters, sorting, suppressed lead recovery, bulk actions, HTMX updates, and normal form fallbacks.
- Multi-currency subscription totals with exchange-rate support and user base currency.
- Analytics views, category distribution, monthly trend data, deeper insights, and exportable monthly reports.
- Renewal notification tasks using Huey and Redis.
- Compiled Tailwind CSS served from Django static files.
- Local quality gates for Pytest, Ruff, Mypy, and Tailwind freshness.

## Stack

- Python 3.13
- Django 5.1
- PostgreSQL or SQLite for local development
- Redis and Huey for background work
- HTMX
- Tailwind CSS
- WhiteNoise for static files when `DEBUG=False`
- Pytest, pytest-django, Ruff, Mypy, django-stubs

