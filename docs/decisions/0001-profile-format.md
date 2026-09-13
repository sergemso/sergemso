---
id: 0001
title: Profile format is GitHub profile README
status: draft
date: 2026-09-12
track: product
tags: [profile, github, format]
expires: null
---

## Motivation

Use the special `sergemso/sergemso` repo as GitHub profile README (shows on profile page) rather than a separate personal website or GitHub Pages site.

## Context

GitHub automatically renders the README of a repo matching the username as the profile page. This is the standard convention for developer profiles.

## Tradeoffs

- Pro: Zero hosting/maintenance, native GitHub integration, version controlled
- Pro: Shows commit activity, contributions graph automatically
- Con: Limited to Markdown, no custom domain or advanced styling
- Con: Cannot use client-side JS for interactive elements

## Decision

Use the profile README approach. Keep it as a single Markdown file in the root of `sergemso/sergemso`.