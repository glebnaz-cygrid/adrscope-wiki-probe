---
title: Wiki Publishing Probe
description: Throwaway ADR used to verify that the wiki workflow publishes from GitHub Actions
type: adr
category: tooling
tags:
  - probe
status: accepted
created: 2026-09-22
author: Probe
project: probe
technologies:
  - adrscope
audience:
  - developers
related: []
---

## Context

Verifying whether `GITHUB_TOKEN` can push to a repository's own wiki, and whether
the publishing workflow shapes the pages correctly.

## Decision

Publish from GitHub Actions.

## Consequences

If this page appears in the wiki, the workflow works.

## Diagram

```mermaid
flowchart LR
    A[push to main] --> B[adrscope wiki] --> C[(GitHub Wiki)]
```
