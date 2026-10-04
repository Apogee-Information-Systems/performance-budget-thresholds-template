# Performance Budget Thresholds Template

Ready-to-use **Core Web Vitals and performance score budgets** by site type (e-commerce, agency clients, content, SaaS, landing pages). Copy into Sheets/CSV, your monitoring tool, or Lighthouse CI.

**Who it's for:** Developers, agency leads, and PMs who need concrete pass/fail thresholds.

**What you need:** Any CWV tool (PageSpeed Insights, Lighthouse CI, or automated monitoring). Spreadsheet optional.

**Canonical article:** [Performance Budget Thresholds Template](https://apogeewatcher.com/blog/performance-budget-thresholds-template)

**Index:** [core-web-vitals-checklists](https://github.com/Apogee-Information-Systems/core-web-vitals-checklists) · [Apogee on GitHub](https://apogee-information-systems.github.io/)

## How to use this repo
- Start with Google's "Good" baselines in [`templates/universal-thresholds.csv`](templates/universal-thresholds.csv).
- Pick a site-type profile in [`templates/budgets-by-site-type.csv`](templates/budgets-by-site-type.csv).
- Track multiple clients with [`templates/multi-client-tracking.csv`](templates/multi-client-tracking.csv).
- Wire CI with [`templates/lighthouserc.example.json`](templates/lighthouserc.example.json).

## Universal thresholds (Google "Good")

| Metric | Good | Needs Improvement | Poor | Unit |
|:-------|:-----|:------------------|:-----|:-----|
| LCP | ≤2500 | 2500–4000 | >4000 | ms |
| INP | ≤200 | 200–500 | >500 | ms |
| CLS | ≤0.10 | 0.10–0.25 | >0.25 | score |
| Performance Score | ≥90 | 50–89 | ≤49 | 0–100 |

See CSV files for FCP, TBT, Speed Index and per-site-type mobile/desktop budgets.

## Escalation levels

| Level | Condition | Response |
|:------|:----------|:---------|
| Info | Within 10% of budget | Note for next review |
| Warning | Over budget by &lt; 20% | Investigate within 1 week |
| Critical | Over budget by &gt; 20% | Investigate within 48 hours |
| Emergency | Score &lt; 50 or LCP &gt; 5s | Incident within 4 hours |

## Automate your monitoring

Set budgets per site, get alerts when thresholds are exceeded, and track trends with [Apogee Watcher](https://apogeewatcher.com). [Learn more →](https://apogeewatcher.com)
