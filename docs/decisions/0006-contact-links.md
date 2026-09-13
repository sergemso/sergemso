---
id: 0006
title: Contact section includes LinkedIn, GitHub, ORCID, Email, Calendly, DEV, Medium
status: draft
date: 2026-09-12
track: product
tags: [contact, links, availability]
expires: null
---

## Motivation

Provide multiple verified channels for different engagement types: hiring (LinkedIn), code review (GitHub), academic (ORCID), direct contact (Email/Calendly), writing (DEV/Medium).

## Context

The "Open to" line lists: Senior/Staff IC roles, AI Engineering leadership, Technical advisory, Agent-driven development consulting, B2B/Independent Contractor. Each channel serves different paths.

## Tradeoffs

- Pro: Covers all engagement types without friction
- Pro: ORCID adds academic credibility for research-adjacent work
- Pro: Calendly enables zero-friction scheduling for consulting
- Con: Many links can feel cluttered
- Con: Must keep all profiles updated

## Decision

Use shield badges for visual consistency. Order by engagement likelihood: LinkedIn → GitHub → ORCID → Email → Calendly → DEV → Medium. Status badge at top for immediate contractor visibility.