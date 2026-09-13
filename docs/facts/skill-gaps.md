---
id: skill-gaps
title: Skill gap detection proposals
type: derived
status: active
date: 2026-09-13
governed-by: TBD
kms-generated: true
tags: [skills, gaps, proposals]
---

## Proposed skill domains from repo signals

| Signal in Repo | Domain to Cover | Likely Review Role | What It Would Own | Hard Constraint | Fitness Function Candidate |
|----------------|-----------------|-------------------|-------------------|-----------------|----------------------------|
| Profile README as primary artifact; decisions about format, branding, audience | **Profile Content Strategy** | Content Strategist | Profile structure, messaging, audience alignment, content freshness | Profile must render correctly on GitHub profile page | Link validity check; content freshness (articles < 6 months) |
| Three public projects (virage, kms, edap_model) referenced as portfolio | **Portfolio Project Curation** | Technical Lead | Project selection, descriptions, tech stack accuracy, link health | All featured projects must be publicly accessible | Automated link checks; version freshness |
| Contact channels for different engagement types (hiring, consulting, academic) | **Engagement Channel Management** | Business Development | Channel relevance, response SLAs, availability accuracy | Calendly link must be functional | Link checks; Calendly API availability |
| Technical writing on DEV and Medium | **Technical Writing Pipeline** | Technical Writer | Article quality, cross-posting strategy, SEO, topic alignment | Articles must align with brand focus (AI Engineering + Backend) | Topic tagging consistency; publication cadence |
| GitHub repo as profile (no separate site) | **GitHub Profile Operations** | DevOps Engineer | Repo settings, branch protection, GitHub Pages (if used), Actions for validation | Profile repo must remain username-matching | Branch protection status; Actions workflow success |
| No CI/CD, no linting, no automated checks | **Profile Quality Assurance** | QA Engineer | Automated validation of all profile assertions | Zero-friction validation on every push | Full validation suite in GitHub Actions |
| Decision records created during bootstrap | **Knowledge Management Operations** | Knowledge Steward | Decision/fact/guardrail lifecycle, capture process, lint integration | All decisions must have track (product|process) | Lint passes; INDEX.md freshness |

## Priority domains (governing irreversible/public commitments)

1. **Profile Content Strategy** - Public-facing profile is the primary artifact; errors directly affect professional reputation
2. **Portfolio Project Curation** - Featured projects are public claims about capabilities; broken links or outdated info damages credibility
3. **GitHub Profile Operations** - Repo configuration affects visibility; misconfiguration hides profile