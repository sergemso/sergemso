---
id: fitness-inventory
title: Fitness function inventory
type: derived
status: active
date: 2026-09-13
governed-by: TBD
kms-generated: true
tags: [fitness, ci, automation, debt]
---

## Enforced checks (currently automated)

| Rule | Automation | Governing Decision | Notes |
|------|------------|-------------------|-------|
| README.md exists | GitHub Pages/profile rendering | 0001 | GitHub auto-renders username-matching repo |
| Branch protection | GitHub settings (not configured) | TBD | No branch protection rules set |
| Markdown linting | Not configured | TBD | No markdownlint or similar in CI |

## Candidate fitness functions (not yet automated)

| Rule | Why Not Automated | Governing Decision | Fitness Function Candidate |
|------|-------------------|-------------------|----------------------------|
| All project links (virage, kms, edap_model) return 200 | No CI pipeline | 0002 | Scheduled link check via GitHub Actions |
| All contact links (LinkedIn, ORCID, Calendly, DEV, Medium) return 200 | No CI pipeline | 0006 | Scheduled link check via GitHub Actions |
| Tech stack categories match decision 0002 domains | Manual review only | 0002, 0004 | Lint rule: categories must include AI Engineering, Backend/Platform |
| Experience highlights contain no company names | Manual review only | 0005 | Regex check: no known employer names in README |
| All article links have valid HTTPS URLs | Manual review only | 0006 | Markdown link validator |
| ORCID format valid (0000-0000-0000-0000) | Manual review only | 0010 | Regex check on ORCID badge URL |
| Status badge matches "Open to" line | Manual review only | 0011 | Consistency check between badge text and footer |

## Debt log

- No CI/CD pipeline exists for this repo
- No markdown linting
- No link checking
- No branch protection
- No automated validation of profile content against decisions